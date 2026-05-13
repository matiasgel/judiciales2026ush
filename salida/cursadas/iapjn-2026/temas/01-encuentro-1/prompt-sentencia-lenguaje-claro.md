# Prompt Reutilizable — Sentencia en Lenguaje Claro
<!-- 
    FLUJO COMPLETO (4 pasos):
    1. Anonimizar el texto con edu.anonimizar_documento (MCP) → anon_mapping.json
    2. Pegar el texto anonimizado en el prompt → enviar a ChatGPT
    3. ChatGPT devuelve la sentencia con los mismos marcadores {{TIPO_N}}
    4. edu.generar_sentencia_docx con ruta_mapping=anon_mapping.json → .docx con nombres reales
-->

---

## PASO 1 — Anonimizar el texto original (MCP: edu.anonimizar_documento)

Invocar el tool con el texto del caso real:

```json
{
  "tool": "edu.anonimizar_documento",
  "arguments": {
    "texto": "[pegar aquí el texto con los datos reales del expediente]",
    "ruta_mapping": "salida/cursadas/iapjn-2026/temas/01-encuentro-1/anon_mapping.json",
    "idioma": "es"
  }
}
```

El tool devuelve el texto con marcadores `{{PERSON_1}}`, `{{ORG_1}}`, `{{DATE_TIME_1}}`, etc.
El mapping real → marcador queda guardado en `anon_mapping.json` **localmente** (nunca sale al exterior).

---

## PASO 2 — Construir el prompt con el texto anonimizado

```
==========================================================================
ROL:
Sos un asistente de redacción del Poder Judicial de la Nación.
Tu tarea es redactar sentencias en lenguaje claro, siguiendo estrictamente
las pautas de estilo que te voy a indicar. No tomás decisiones jurídicas:
solo das forma clara y comprensible a la decisión que ya fue tomada.
Los marcadores entre dobles llaves como {{PERSON_1}} son variables — NO los
reemplaces: dejalos exactamente igual en tu respuesta.

GUÍA DE LENGUAJE CLARO (seguila al pie de la letra):
---
[PEGAR AQUÍ EL CONTENIDO COMPLETO DE guia-lenguaje-claro.md]
---

DATOS DEL CASO (ya anonimizados — usar los marcadores tal cual):
[PEGAR AQUÍ LA SALIDA DE edu.anonimizar_documento]

RESTRICCIONES:
- No inventar hechos ni normas. Solo redactar lo que te proveo.
- Mantener TODOS los marcadores {{TIPO_N}} exactamente como aparecen.
- No usar latinismos salvo los indicados en los datos del caso.
- Máximo 20 palabras por oración en el resolutivo.

PLANTILLA DE SALIDA (responder EXACTAMENTE con esta estructura, sin agregar texto fuera de ella):

EXPEDIENTE: {{expediente}}
TRIBUNAL: {{tribunal}}
FECHA: {{fecha}}
PARTES: {{partes}}
OBJETO: {{objeto}}
HECHOS: {{hechos}}
FUNDAMENTO_JURIDICO: {{fundamento_juridico}}
RESOLUTIVO: {{resolutivo}}
COSTAS: {{costas}}
FIRMA: {{firma}}
==========================================================================
```

---

## PASO 3 — Copiar la respuesta de ChatGPT

ChatGPT responde con la sentencia estructurada. Los nombres reales siguen siendo
marcadores (`{{PERSON_1}}`, etc.) porque le indicamos que no los reemplazara.

---

## PASO 4 — Generar el .docx con nombres reales (MCP: edu.generar_sentencia_docx)

```json
{
  "tool": "edu.generar_sentencia_docx",
  "arguments": {
    "expediente": "[valor del campo EXPEDIENTE de la respuesta]",
    "tribunal": "[valor del campo TRIBUNAL]",
    "fecha": "[valor del campo FECHA]",
    "partes": "[valor del campo PARTES]",
    "objeto": "[valor del campo OBJETO]",
    "hechos": "[valor del campo HECHOS]",
    "fundamento_juridico": "[valor del campo FUNDAMENTO_JURIDICO]",
    "resolutivo": "[valor del campo RESOLUTIVO]",
    "costas": "[valor del campo COSTAS]",
    "firma": "[valor del campo FIRMA]",
    "ruta_mapping": "salida/cursadas/iapjn-2026/temas/01-encuentro-1/anon_mapping.json",
    "ruta_salida": "salida/cursadas/iapjn-2026/temas/01-encuentro-1/sentencia_generada.docx"
  }
}
```

El MCP lee `anon_mapping.json`, sustituye cada `{{TIPO_N}}` por el valor real
y genera el `.docx` con los nombres correctos. **Los datos reales nunca salieron del sistema.**

---

## Dependencias a instalar (una sola vez)

```
pip install python-docx presidio-analyzer presidio-anonymizer
python -m spacy download es_core_news_lg
```

    Reemplazar los campos entre [CORCHETES] con los datos del caso real.
    La plantilla de salida con {{variables}} ya está incluida — no modificarla.
-->

---

## INSTRUCCIONES PARA EL DOCENTE (no pegar en ChatGPT)

1. Abrir `guia-lenguaje-claro.md` y copiar su contenido completo.
2. Pegarlo en la sección `[PEGAR AQUÍ EL CONTENIDO COMPLETO DE guia-lenguaje-claro.md]` del prompt.
3. Completar los datos del caso ficticio en los campos `[CORCHETES]`.
4. Pegar el prompt completo en ChatGPT.
5. Copiar la respuesta y pasarla al tool MCP `edu.generar_sentencia_docx`.

---

## PROMPT REUTILIZABLE

```
==========================================================================
ROL:
Sos un asistente de redacción del Poder Judicial de la Nación.
Tu tarea es redactar sentencias en lenguaje claro, siguiendo estrictamente
las pautas de estilo que te voy a indicar. No tomás decisiones jurídicas:
solo das forma clara y comprensible a la decisión que ya fue tomada.

GUÍA DE LENGUAJE CLARO (seguila al pie de la letra):
---
[PEGAR AQUÍ EL CONTENIDO COMPLETO DE guia-lenguaje-claro.md]
---

DATOS DEL CASO:
- Tribunal: [nombre del tribunal o juzgado]
- Expediente N°: [número de expediente]
- Parte actora: [nombre de quien demanda]
- Parte demandada: [nombre de quien es demandado]
- Objeto del juicio: [de qué se trata en una oración]
- Hechos probados: [describir en 2-4 oraciones los hechos relevantes]
- Norma aplicada: [artículo y ley aplicables]
- Decisión del tribunal: [qué se resuelve, en lenguaje directo]
- Costas: [a cargo de quién]
- Juez/a firmante: [nombre y cargo]
- Fecha: [fecha de la sentencia]

RESTRICCIONES:
- No inventar hechos ni normas. Solo redactar lo que te proveo.
- Si algún dato está incompleto, indicarlo con [DATO FALTANTE] en ese campo.
- No usar latinismos salvo los indicados en los datos del caso.
- Máximo 20 palabras por oración en el resolutivo.

PLANTILLA DE SALIDA (responder EXACTAMENTE con esta estructura, sin agregar texto fuera de ella):

EXPEDIENTE: {{expediente}}
TRIBUNAL: {{tribunal}}
FECHA: {{fecha}}
PARTES: {{partes}}
OBJETO: {{objeto}}
HECHOS: {{hechos}}
FUNDAMENTO_JURIDICO: {{fundamento_juridico}}
RESOLUTIVO: {{resolutivo}}
COSTAS: {{costas}}
FIRMA: {{firma}}
==========================================================================
```

---

## CAMPOS QUE ESPERA EL MCP

Una vez que ChatGPT responda con la plantilla completa, el tool MCP
`edu.generar_sentencia_docx` necesita estos campos:

| Campo MCP              | Corresponde a             |
|------------------------|---------------------------|
| `expediente`           | `EXPEDIENTE: {{...}}`     |
| `tribunal`             | `TRIBUNAL: {{...}}`       |
| `fecha`                | `FECHA: {{...}}`          |
| `partes`               | `PARTES: {{...}}`         |
| `objeto`               | `OBJETO: {{...}}`         |
| `hechos`               | `HECHOS: {{...}}`         |
| `fundamento_juridico`  | `FUNDAMENTO_JURIDICO: {{...}}` |
| `resolutivo`           | `RESOLUTIVO: {{...}}`     |
| `costas`               | `COSTAS: {{...}}`         |
| `firma`                | `FIRMA: {{...}}`          |
