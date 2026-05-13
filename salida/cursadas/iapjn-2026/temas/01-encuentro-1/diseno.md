# Diseño: Encuentro 1 — Entender para no equivocarse
<!-- STATUS: BORRADOR -->

## Metadatos
- **Tema:** 01 — encuentro-1
- **Título completo:** Encuentro 1 — Entender para no equivocarse
- **Materia:** Inteligencia Artificial en el Poder Judicial de la Nación
- **Institución:** Poder Judicial de la Nación
- **Duración estimada:** 90 minutos ← _referencia orientativa; el docente suele completar el contenido en menos tiempo — no usarla como constraint rígido de generación_
- **Público:** Usuarios sin experiencia previa o con bajo nivel técnico
- **Perfil docente:** Licenciado en Informática, investigador docente en IA
- **Fecha de diseño:** 2026-04-27

---

## Objetivo general del encuentro

Brindar a los participantes una comprensión básica y operativa de la inteligencia artificial y sus riesgos, para que puedan tomar decisiones informadas sobre su uso en el entorno judicial.

---

## Objetivos específicos de aprendizaje

Al finalizar el encuentro, el participante podrá:

1. Explicar con sus propias palabras qué es la inteligencia artificial y qué la diferencia de un buscador o base de datos.
2. Identificar al menos dos casos de uso concreto de IA en tareas del Poder Judicial de la Nación.
3. Nombrar los principales riesgos del uso de IA en contextos legales (alucinaciones, confidencialidad).
4. Describir qué es la ventana de contexto y cómo afecta la calidad de la respuesta.
5. Formular un prompt básico con estructura: rol + tarea + contexto + restricciones.

---

## Público objetivo

- Personal del PJN sin experiencia previa en IA
- Perfiles: administrativos, empleados judiciales, auxiliares
- Supuesto: saben usar un navegador web y correo electrónico; no se asume conocimiento técnico

---

## Tópicos del plan mínimo asignados

| N° | Tópico | Fuente (plan-minimo.md) |
|----|--------|-------------------------|
| 1 | Introducción a la IA | §1 Día 1 |
| 2 | Uso de IA en el Poder Judicial | §2 Día 1 |
| 3 | Riesgos del uso de IA | §3 Día 1 |
| 4 | Ventana de contexto | §4 Día 1 |
| 5 | Introducción al prompting | §5 Día 1 |

---

## Distribución de tiempo (90 min)

| Bloque | Nombre | Duración | Tipo |
|--------|--------|----------|------|
| 0 | Apertura y presentación del día | 5 min | Encuadre |
| 1 | Introducción a la IA | 15 min | Conceptual |
| 2 | Uso de IA en el Poder Judicial | 8 min | Aplicado |
| 3 | Riesgos del uso de IA | 12 min | Crítico / Preventivo |
| 4 | Ventana de contexto | 8 min | Conceptual |
| 5 | Introducción al prompting | 32 min | Práctico |
| 6 | Cierre, preguntas y mensaje clave | 10 min | Síntesis |
| **Total** | | **90 min** | |

> **Perfil docente:** Ritmo de exposición ágil — los bloques teóricos están dimensionados para exposición fluida sin detenerse en detalles técnicos. El tiempo ganado en teoría se vuelca íntegro en el ejercicio práctico de prompting.

> **Regla de scope:** Cualquier contenido no listado en la tabla anterior está fuera de scope de este encuentro.

---

## Descripción por bloque

### Bloque 0 — Apertura (5 min)
- Presentación del docente y del programa del encuentro
- Pregunta inicial al público: "¿Alguien ya usó ChatGPT o una IA? ¿Para qué?"
- Objetivo: romper el hielo y activar conocimientos previos

### Bloque 1 — Introducción a la IA (15 min)
**Subtemas:**
- Qué es la inteligencia artificial (definición operativa, sin tecnicismos)
- Qué es un modelo generador / LLM: la metáfora del "predictor de palabras"
- Diferencias fundamentales entre buscador (índice), base de datos (hechos fijos) y modelo probabilístico (generación)

**Objetivo de bloque:** Que el participante entienda que la IA genera texto probable, no verdad verificada.

**Estrategia pedagógica:** Exposición directa con 2 analogías clave (autocomplete del celular + adivino de palabras). Mínima discusión — el docente avanza rápido y rescata preguntas para el cierre.

**Nota de ritmo:** Sin profundizar en historia ni arquitectura técnica — solo lo necesario para entender el riesgo de alucinación.

**Filminas estimadas:** 4

### Bloque 2 — Uso de IA en el Poder Judicial (8 min)
**Subtemas:**
- Redacción de oficios (ejemplo real con IA)
- Resumen de expedientes
- Mejora de textos jurídicos
- **Búsqueda y síntesis de jurisprudencia:** pedir a la IA que organice y resuma criterios jurisprudenciales sobre un tema específico, con plantilla de salida estructurada por posición jurídica

**Objetivo de bloque:** Mostrar que la IA ya es aplicable hoy en tareas concretas del PJN.

**Estrategia pedagógica:** Demo en vivo por el docente: escribir el prompt frente al grupo y mostrar el resultado en pantalla proyectada. Los participantes observan y comentan.

**Filminas estimadas:** 2–3

### Bloque 3 — Riesgos del uso de IA (12 min)
**Subtemas:**
- Invención de información (alucinación): ejemplos con citas legales inexistentes
- Uso indebido de datos sensibles: qué pasa cuando se pega un expediente en ChatGPT
- Problemas legales: confidencialidad, secreto de sumario, GDPR/marco argentino
- Confianza excesiva: el riesgo de "si lo dijo la IA, es verdad"

**Objetivo de bloque:** Que el participante sepa _cuándo NO usar IA_ antes de aprender a usarla.

**Estrategia pedagógica:** Un caso real contundente (Mata vs Avianca — abogado citó casos inexistentes generados por IA) presentado en 2 slides. El impacto reemplaza la discusión extendida — el docente cierra con la regla concreta: "nunca pegues un expediente real en un chat público".

**Filminas estimadas:** 3–4

### Bloque 4 — Ventana de contexto (8 min)
**Subtemas:**
- Qué es el contexto: "la memoria de trabajo de la IA"
- Cómo afecta la respuesta: mismo prompt con contexto diferente → respuestas distintas
- Limitaciones en textos largos: por qué el modelo "se olvida" del principio en documentos extensos

**Objetivo de bloque:** Que el participante sepa que la IA no recuerda nada entre sesiones y que el contexto debe proveerse explícitamente.

**Estrategia pedagógica:** Metáfora del "pizarrón que se borra entre sesiones" — exposición directa sin demo técnica. Este bloque sirve de puente hacia el Bloque 5: "por eso el prompt tiene que tener todo el contexto necesario".

**Filminas estimadas:** 2–3

### Bloque 5 — Introducción al prompting (32 min)
**Subtemas:**
- Por qué la forma de pedir afecta el resultado (2 min — concepto disparador)
- Estructura básica: **Rol + Tarea + Contexto + Restricciones** (5 min — explicación con plantilla visual)
- Ejemplos malos vs. buenos para tareas del PJN (5 min — 3 pares de prompts en pantalla)
- **Plantillas de salida:** cómo incluir en el prompt el formato esperado de la respuesta — tabla, listado, borrador de oficio con secciones fijas. Concepto clave: "si no le decís cómo responder, la IA inventa el formato" (3 min)
- **Demo 1 — Prompt sin estructura** (5 min): el docente escribe un prompt vago en vivo y muestra el resultado pobre; el grupo diagnostica qué le falta
- **Demo 2 — Prompt mejorado** (7 min): el docente reescribe el mismo prompt con la estructura completa; el grupo compara los dos resultados en pantalla
- **Demo 3 — Prompt con restricción de confidencialidad** (5 min): el docente agrega "responde solo con la información que te proveo" y muestra cómo cambia el comportamiento; discusión sobre por qué importa en el PJN
- **Plantillas de salida con variables** (5 min): cómo pedirle a ChatGPT que responda usando una plantilla con marcadores `{{variable}}` — el modelo rellena los campos, la estructura queda fija. Ejemplo de plantilla de oficio genérico:
  ```
  OFICIO N°: {{numero}}
  Destinatario: {{destinatario}}
  Asunto: {{asunto}}
  Cuerpo: {{cuerpo}}
  Firma: {{firma}}
  ```
  El docente muestra el antes (respuesta libre) y el después (respuesta con variables completadas) en vivo.
- **Demo 4 — De la respuesta al .docx vía MCP** (5 min): el docente copia los campos de la respuesta estructurada de ChatGPT y los pasa al tool `edu.generar_oficio_docx` del MCP server EDU. Se genera un `.docx` listo para usar sin abrir la terminal. Objetivo: mostrar que la IA puede ser el primer eslabón de un flujo de trabajo real, con el MCP como puente entre el chat y los documentos institucionales.
- **Demo 5 — Búsqueda de jurisprudencia** (5 min): el docente usa el prompt estructurado de búsqueda de jurisprudencia — la IA sintetiza posiciones jurídicas y lista fallos relevantes. El docente muestra la plantilla de salida antes de ejecutar el prompt para que el grupo vea la diferencia entre "buscá jurisprudencia sobre X" y un pedido con roles, restricciones y formato definido. **Advertencia clave que el docente pronuncia en este momento:** la IA puede inventar fallos que no existen — el resultado siempre debe verificarse en Saij, Infojus o la base del tribunal.

**Plantilla de prompt reutilizable — búsqueda de jurisprudencia:**
```
Actuás como asistente de investigación jurídica.
Tu tarea es identificar y sintetizar los principales criterios jurisprudenciales
sobre el siguiente tema: [TEMA JURÍDICO].
Trabajás para un/a [ROL: juez/a | secretario/a | defensor/a | fiscal] del fuero [FUERO].

RESTRICCIONES:
- Limitá la respuesta a los criterios más relevantes y consolidados.
- No inventes fallos. Si no tenés certeza de un fallo específico, indicalo explícitamente.
- No incluyas opinión doctrinaria, solo posiciones jurisprudenciales.
- Si hay posiciones encontradas, identificalas como Postura A y Postura B.

USÁ EXACTAMENTE ESTA PLANTILLA DE SALIDA, sin agregar texto fuera de ella:

TEMA: {{tema}}
FUERO / JURISDICCIÓN: {{fuero}}
POSTURA PREDOMINANTE: {{postura_predominante}}
FUNDAMENTO CENTRAL: {{fundamento_central}}
FALLOS DE REFERENCIA:
  - {{fallo_1}}
  - {{fallo_2}}
  - {{fallo_3}}
POSTURA MINORITARIA O EN TENSIÓN (si existe): {{postura_minoritaria}}
OBSERVACIONES: {{observaciones}}
ADVERTENCIA: Esta síntesis debe verificarse en Saij, Infojus o la base del tribunal antes de ser utilizada en actuaciones.
```

- **Construcción colectiva** (8 min): el docente proyecta una situación nueva (ej: redactar un oficio) y el grupo dicta en voz alta el prompt + la plantilla de salida con variables; el docente lo escribe, ejecuta y genera el .docx en tiempo real

**Objetivo de bloque:** Que el participante comprenda la estructura del prompt, sepa incluir una plantilla de salida para obtener respuestas estructuradas y predecibles, y pueda dictar o corregir un prompt oralmente verificando el resultado en pantalla.

**Estrategia pedagógica:** Todas las interacciones son demos en vivo proyectadas — el docente opera la herramienta, los participantes observan, diagnostican y proponen mejoras oralmente. No se requiere ningún dispositivo individual.

**Material de apoyo:** Slide fija con la plantilla `[Rol] + [Tarea] + [Contexto] + [Restricciones] + [Plantilla de salida]` visible durante todo el bloque. Roberto debe incluir una filmina de ejemplo de plantilla de salida (tabla de oficio, listado numerado) como slide de referencia.

**Filminas estimadas:** 10–12

### Bloque 5b — Demo avanzada: sentencia en lenguaje claro → .docx (20 min)

> **Nota de scope:** Este bloque es la culminación práctica del encuentro. Muestra el flujo completo: documento de referencia como contexto → prompt reutilizable → salida estructurada → .docx generado por MCP. Está pensado para cerrar la sesión con un caso de uso real e impactante.

**Subtemas:**
- **El problema:** las sentencias judiciales son largas, técnicas y difíciles de entender para las partes. El lenguaje claro es una solución ya adoptada en varios tribunales.
- **El documento de referencia** (2 min): el docente muestra `guia-lenguaje-claro.md` — contiene los principios clave (oraciones cortas, voz activa, evitar latinismos, estructura lógica). Este documento se **pega como contexto en el prompt**, no se adjunta como archivo. Concepto a transmitir: "el contexto es el poder del prompt".
- **El prompt reutilizable** (5 min): el docente abre `prompt-sentencia-lenguaje-claro.md` — un prompt completo que ya tiene: rol del asistente, instrucciones de lenguaje claro, y la plantilla de salida con campos `{{variable}}` embebidos. El docente explica por qué este prompt es reutilizable: solo hay que cambiar los datos del caso.
- **Demo en vivo** (8 min): flujo completo en 4 pasos:
  1. El docente tiene un texto con datos reales de un caso ficticio.
  2. Invoca `edu.anonimizar_documento` via MCP → Presidio (Microsoft) detecta nombres, organizaciones, fechas y los reemplaza con marcadores `{{PERSON_1}}`, `{{ORG_1}}`, etc. El mapping real→marcador se guarda en `anon_mapping.json` localmente. **Nunca sale ningún dato real hacia ChatGPT.**
  3. El texto anonimizado se pega en el prompt reutilizable y se envía a ChatGPT → responde con la sentencia estructurada con los mismos marcadores.
  4. Se invoca `edu.generar_sentencia_docx` con la respuesta + la ruta del `anon_mapping.json` → el MCP sustituye los marcadores por los valores reales y genera el `.docx` final con nombres reales, sin que hayan salido del sistema.
- **Reflexión final** (5 min): diferencia entre "usar IA para hacer el trabajo del juez" vs "usar IA como asistente de redacción con el criterio del juez". Regla: el contenido jurídico lo decide el magistrado — la IA da forma, no criterio.

**Objetivo de bloque:** Que el participante vea en acción un flujo completo y real: documento de referencia + prompt reutilizable + plantilla de salida + generación de .docx. Que entienda que la IA no reemplaza el juicio jurídico sino que acelera la redacción.

**Archivos de demo en la carpeta del tema:**
- `guia-lenguaje-claro.md` — principios de lenguaje claro para sentencias (fuentes: lenguajeclaroargentina.gob.ar)
- `prompt-sentencia-lenguaje-claro.md` — prompt reutilizable con plantilla de sentencia embebida
- Tool MCP: `edu.anonimizar_documento` (Microsoft Presidio) → genera `anon_mapping.json`
- Tool MCP: `edu.generar_sentencia_docx` → acepta `ruta_mapping` para revertir anonimización en el .docx

**Mensaje clave sobre privacidad:**
> "El dato real nunca sale al exterior: se anonimiza antes de ir a ChatGPT y se restituye localmente al generar el documento."

**Estrategia pedagógica:** Demo completamente en pantalla proyectada. El docente opera — los participantes observan. El impacto está en ver que un documento institucional formal sale en 30 segundos con formato correcto.

**Filminas estimadas:** 4–5

### Bloque 6 — Cierre (10 min)
- Síntesis de los 5 conceptos clave del día
- Mensaje central: **"La IA no garantiza verdad: genera respuestas plausibles."**
- Respuesta a preguntas del público
- Anuncio del Encuentro 2: trabajo con documentos judiciales

---

## Filminas estimadas: 28–34 filminas

> Distribución orientativa (ajustable por Roberto en la redacción):
> - 1 portada
> - 1 agenda
> - 4 bloque 1 (teoría condensada)
> - 2–3 bloque 2
> - 3–4 bloque 3
> - 2–3 bloque 4
> - 8–9 bloque 5 (práctico expandido — incluye plantilla de prompt, ejemplos de plantillas de salida, demos ronda a ronda)
> - 1 cierre

> **Nota de producción:** En el Bloque 5, la filmina de plantilla `[Rol] + [Tarea] + [Contexto] + [Restricciones] + [Plantilla de salida]` debe permanecer visible durante todas las demos. Roberto debe incluir además una filmina con 2–3 ejemplos de plantillas de salida típicas del PJN (tabla de campos de oficio, listado numerado de observaciones, borrador con secciones fijas).

---

## Concepto no negociable del encuentro

> **"La IA no garantiza verdad: genera respuestas plausibles."**
> Debe quedar grabado en el participante antes de que use cualquier herramienta de IA en su trabajo.

---

## Restricciones de scope

Los siguientes temas están **fuera de scope** de este encuentro:
- Herramientas específicas de documentos (NotebookLM, Presidio) → Encuentro 2
- Futuro de la IA en el derecho → Encuentro 3
- Algoritmos o código fuente
- Historia de la IA (más allá de lo mínimo orientativo)
- Comparativas técnicas de modelos

---

## Instrucciones de producción para Roberto (class-writer)

> **Leer antes de generar `minuta.md` y `filminas.md`**

### Material de demo incluido en la carpeta del tema

| Archivo | Propósito |
|---------|-----------|
| `oficio_desde_template.py` | Fallback de línea de comandos — misma lógica que el MCP, útil si el server no está corriendo. |

**Tool MCP para la Demo 4:** `edu.generar_oficio_docx`
- Servidor: `edu-mcp-server/server.py`
- Input: campos `numero`, `destinatario`, `asunto`, `cuerpo`, `firma` (salida directa de ChatGPT)
- Output: `.docx` generado en la ruta indicada (default: `oficio_generado.docx`)
- Requiere: `pip install python-docx` en el entorno del MCP server

**Prompt de demo para el docente** (copiar tal cual en ChatGPT):
```
Sos un asistente del Poder Judicial de la Nación. Redactá un oficio formal
respondiendo con EXACTAMENTE esta plantilla, sin agregar nada fuera de ella:

OFICIO N°: {{numero}}
Destinatario: {{destinatario}}
Asunto: {{asunto}}
Cuerpo: {{cuerpo}}
Firma: {{firma}}

Situación: [el docente completa aquí con lo que dicte el grupo]
```

Luego copiar la respuesta de ChatGPT a un archivo `respuesta.txt` y ejecutar:
```
python oficio_desde_template.py respuesta.txt
```

---

### Templates obligatorios

| Artefacto | Template canónico | Ubicación |
|-----------|------------------|-----------|
| `minuta.md` | Estructura canónica de minuta | `_edu/templates/class-template.md` |
| `filminas.md` | Plantilla canónica de filminas | `_edu/templates/filminas-template.md` |
| Directivas y enums | Schema de filminas | `_edu/templates/filminas-schema.yaml` |
| Validación JSON | Contrato del plan | `_edu/schemas/plan-filminas.schema.json` |
| Schema por filmina | Contrato individual | `_edu/schemas/filmina-slide.schema.json` |
| Tipos y layouts | Fuente de verdad pipeline | `_edu/schemas/schema-registry.json` |

### Reglas de uso

1. **`filminas.md`** debe seguir exactamente el esqueleto de `filminas-template.md`: cada slide con `### [F-XX] Título corto`, directivas `@tipo:`, `@layout:` y `@imagen:` donde corresponda.
2. **`minuta.md`** debe seguir la estructura canónica de `class-template.md`: sección por filmina `[F-XX]`, con `Qué decir`, `Conceptos clave`, `Preguntas anticipadas` y `Transición`.
3. Las filminas del Bloque 5 que contengan demos deben usar `@tipo: demo`.
4. La filmina de plantilla de prompt (`[Rol] + [Tarea] + [Contexto] + [Restricciones]`) debe llevar `@tipo: concepto-abstracto` y permanecer como slide de referencia visible durante todo el bloque de prompting.
5. **Duración:** No usar los 90 min como límite estricto — el docente avanza más rápido. Generar el contenido completo sin recortar bloques para ajustar al tiempo estimado.

---

## Criterios de aprobación del diseño

- [ ] Duración total ≤ 90 minutos con los bloques propuestos
- [ ] Los 5 tópicos del plan-mínimo (Día 1) están cubiertos
- [ ] El diseño es ejecutable por un docente con perfil investigador
- [ ] El público objetivo (no técnico) puede seguir el hilo sin perderse
- [ ] El bloque de prompting es enteramente en vivo (demo proyectada por el docente — sin dispositivos individuales)
