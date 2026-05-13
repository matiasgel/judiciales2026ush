# Encuentro 1 — "Entender para no equivocarse"
### Propuesta de diseño pedagógico · Para revisión y aprobación

---

**Materia:** Inteligencia Artificial en el Poder Judicial de la Nación  
**Institución:** Poder Judicial de la Nación  
**Público:** Personal del PJN sin experiencia previa en IA (administrativos, empleados judiciales, auxiliares)  
**Perfil del participante:** Maneja navegador web y correo electrónico. No se asume ningún conocimiento técnico.  
**Perfil docente:** Licenciado en Informática, investigador en IA

---

## ¿Qué se busca lograr?

Al terminar el encuentro, cada participante debe poder:

1. Explicar con sus propias palabras qué es la inteligencia artificial y en qué se diferencia de un buscador o una base de datos.
2. Reconocer al menos dos tareas concretas del Poder Judicial en las que la IA ya puede ser útil hoy.
3. Nombrar los principales riesgos de usar IA en el trabajo judicial: alucinaciones y confidencialidad.
4. Entender qué es la ventana de contexto y por qué el modelo no recuerda información entre sesiones.
5. Formular un prompt básico usando la estructura: **Rol + Tarea + Contexto + Restricciones**.

---

## Estructura del encuentro

| Bloque | Contenido | Modalidad |
|--------|-----------|-----------|
| 0 | Apertura y presentación | Encuadre |
| 1 | ¿Qué es la inteligencia artificial? | Conceptual |
| 2 | IA en el Poder Judicial hoy | Aplicado — demo |
| 3 | Riesgos que hay que conocer primero | Caso real |
| 4 | Ventana de contexto | Conceptual |
| 5 | Cómo formular un prompt | Práctico — demos en vivo |
| 5b | Demo completa: sentencia en lenguaje claro | Demo en vivo |
| 6 | Cierre y síntesis | Síntesis |

---

## Descripción de cada bloque

### Bloque 0 — Apertura

Presentación del docente y del programa del día.

Pregunta disparadora al grupo: *"¿Alguien ya usó ChatGPT o alguna IA? ¿Para qué?"*

Objetivo: activar saberes previos y romper el hielo antes de la parte conceptual.

---

### Bloque 1 — ¿Qué es la inteligencia artificial?

**Temas:**
- Definición operativa de IA, sin tecnicismos.
- Qué es un modelo de lenguaje: la metáfora del "predictor de palabras".
- Diferencia entre buscador (índice de páginas), base de datos (hechos fijos) y modelo generativo (texto probable).

**Mensaje clave del bloque:**
> La IA genera texto probable, no verdad verificada.

**Cómo se desarrolla:** Exposición directa con dos analogías accesibles: el autocomplete del celular y el adivino de palabras. Sin historia de la IA ni detalles técnicos. Las preguntas del público se reservan para el cierre.

---

### Bloque 2 — IA en el Poder Judicial hoy

**Tareas en las que la IA ya puede colaborar:**
- Redacción de oficios
- Resumen de expedientes
- Mejora de textos jurídicos
- **Búsqueda y síntesis de jurisprudencia:** pedirle a la IA que identifique y organice los criterios jurisprudenciales relevantes sobre un tema específico, con postura predominante, fallos de referencia y postura en tensión — todo en un formato estructurado y verificable

**Cómo se desarrolla:** Demo en vivo proyectada. El docente escribe un prompt frente al grupo y muestra el resultado en pantalla. Los participantes observan y comentan.

---

### Bloque 3 — Riesgos que hay que conocer primero

**Temas:**
- **Alucinaciones:** la IA inventa información. Caso real: *Mata vs. Avianca* — un abogado presentó jurisprudencia citada por ChatGPT que no existía. El tribunal lo sancionó.
- **Confidencialidad:** qué pasa cuando se pega el texto de un expediente en un chat público.
- **Confianza excesiva:** el riesgo de asumir que si lo dijo la IA, es correcto.
- Marco normativo: confidencialidad, secreto de sumario, datos personales.

**Regla concreta para el participante:**
> Nunca pegues el texto de un expediente real en un chat público.

**Cómo se desarrolla:** El caso Mata vs. Avianca se presenta con alto impacto visual. El bloque termina con la regla anterior, pronunciada en voz alta por el docente.

---

### Bloque 4 — Ventana de contexto

**Temas:**
- Qué es el contexto: "la memoria de trabajo de la IA".
- Cómo afecta la respuesta: el mismo prompt con contexto diferente produce resultados distintos.
- Por qué el modelo parece olvidar el principio en documentos muy largos.

**Cómo se desarrolla:** Metáfora del pizarrón que se borra entre sesiones. Sin demo técnica. Funciona como puente hacia el bloque siguiente: *"por eso el prompt tiene que tener todo el contexto necesario".*

---

### Bloque 5 — Cómo formular un prompt

Este es el bloque central y práctico del encuentro. Se desarrolla íntegramente como demo en vivo proyectada. El docente opera — los participantes observan, diagnostican y proponen mejoras en voz alta. No se requiere ningún dispositivo individual.

**Secuencia del bloque:**

**1. Por qué importa la forma de pedir**
La calidad de la respuesta depende directamente de cómo está redactado el pedido.

**2. La estructura básica**
Plantilla canónica: **Rol + Tarea + Contexto + Restricciones**
Esta plantilla queda visible en pantalla durante todas las demos que siguen.

**3. Ejemplos malos vs. buenos**
Tres pares de prompts para tareas típicas del PJN. El grupo compara los resultados en pantalla.

**4. Plantillas de salida**
Cómo incluir en el prompt el formato esperado de la respuesta.
Concepto clave: *"Si no le decís cómo responder, la IA inventa el formato."*
Ejemplo de plantilla de oficio con campos fijos:

```
OFICIO N°: {{numero}}
Destinatario: {{destinatario}}
Asunto: {{asunto}}
Cuerpo: {{cuerpo}}
Firma: {{firma}}
```

**5. Demo 1 — Prompt sin estructura**
El docente escribe un prompt vago en vivo. El grupo diagnostica qué le falta.

**6. Demo 2 — Prompt mejorado**
El docente reescribe el mismo prompt con la estructura completa. El grupo compara los dos resultados lado a lado.

**7. Demo 3 — Prompt con restricción de confidencialidad**
El docente agrega *"responde solo con la información que te proveo"* y muestra cómo cambia el comportamiento.
Discusión: por qué esto es importante en el PJN.

**8. Demo 4 — De la respuesta al documento**
El docente obtiene de ChatGPT una respuesta con campos de oficio estructurados y genera un archivo `.docx` listo para usar en segundos. Objetivo: mostrar que la IA puede ser el primer eslabón de un flujo de trabajo real.

**9. Demo 5 — Búsqueda de jurisprudencia con prompt estructurado**
El docente muestra la diferencia entre pedirle a ChatGPT *"buscá jurisprudencia sobre responsabilidad del Estado"* y usar un prompt estructurado con rol, restricciones explícitas y plantilla de salida definida.

Plantilla de prompt utilizada en la demo:

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
ADVERTENCIA: Esta síntesis debe verificarse en Saij, Infojus o la base del tribunal
antes de ser utilizada en actuaciones.
```

**Advertencia clave que el docente pronuncia en este momento:**
> La IA puede inventar fallos que no existen. Este resultado siempre debe verificarse en Saij, Infojus o la base del tribunal antes de usarse en una actuación.

**10. Construcción colectiva**
El docente proyecta una situación nueva (redactar un oficio). El grupo dicta el prompt en voz alta, incluyendo la plantilla de salida. El docente lo escribe, ejecuta y genera el documento en tiempo real.

---

### Bloque 5b — Demo completa: sentencia en lenguaje claro

> Cierra el encuentro con un caso de uso real e impactante para el ámbito judicial.

**El problema que resuelve:**
Las sentencias judiciales suelen ser largas, técnicas y difíciles de entender para las partes. El lenguaje claro es una práctica ya adoptada en varios tribunales argentinos y avalada por normativa nacional y provincial.

**Estructura de la demo:**

**1. El documento de referencia**
El docente muestra una guía de principios de lenguaje claro basada en normativa oficial argentina (Ministerio de Justicia de la Nación). Este documento se pega como contexto dentro del prompt.
*Concepto a transmitir: "el contexto es el poder del prompt".*

**2. El prompt reutilizable**
El docente abre un prompt ya armado con: rol del asistente, instrucciones de lenguaje claro, y plantilla de salida con campos fijos. Solo hay que cambiar los datos del caso para reutilizarlo en cualquier sentencia.

**3. Flujo completo con protección de privacidad**
La demo muestra cuatro pasos encadenados:

| Paso | Qué sucede | Resultado visible |
|------|-----------|-------------------|
| 1 | El docente tiene un texto con datos de un caso ficticio | Texto con nombres, fechas y datos del expediente |
| 2 | El texto se anonimiza automáticamente | Nombres y datos reemplazados por marcadores como `{{PERSONA_1}}`. El mapeo real → marcador queda guardado **solo en la computadora del docente** |
| 3 | El texto anonimizado va a ChatGPT con el prompt | ChatGPT responde con la sentencia estructurada, conservando los marcadores sin ver los datos reales |
| 4 | Se genera el documento `.docx` final | El sistema restituye los nombres reales desde el mapeo local. El documento queda con los datos correctos |

**Principio que queda demostrado:**
> El dato real nunca sale al exterior. Se protege antes de ir a ChatGPT y se restituye localmente al generar el documento.

**4. Reflexión final**
Diferencia entre "usar IA para tomar la decisión judicial" y "usar IA como asistente de redacción". El contenido jurídico lo decide el magistrado — la IA da forma, no criterio.

---

### Bloque 6 — Cierre

- Síntesis de los conceptos clave del día en pantalla.
- Pregunta final al grupo: *"¿En qué tarea de su trabajo le daría un primer uso a la IA?"*
- Respuesta a preguntas del público.
- Mensaje final del encuentro: **"La IA no garantiza verdad: genera respuestas plausibles."**
- Anuncio del Encuentro 2: trabajo con documentos judiciales.

---

## Materiales del encuentro

| Material | Descripción |
|----------|-------------|
| Presentación | Apoyo visual para todos los bloques |
| Guía de lenguaje claro | Principios basados en normativa oficial argentina para usar como contexto en el prompt |
| Prompt de jurisprudencia | Plantilla reutilizable para búsqueda de criterios jurisprudenciales por tema y fuero |
| Prompt de sentencia | Plantilla reutilizable para redacción de sentencias en lenguaje claro |

Todos los materiales se proyectan en pantalla. **No se distribuye ningún material en papel ni se requiere ningún dispositivo individual de los participantes.**

---

## Cobertura del programa oficial

| Tópico del programa | Cubierto en |
|---------------------|-------------|
| Introducción a la IA | Bloque 1 |
| Uso de IA en el Poder Judicial | Bloque 2 |
| Riesgos del uso de IA | Bloque 3 |
| Ventana de contexto | Bloque 4 |
| Introducción al prompting | Bloque 5 |

---

## Fuera del alcance de este encuentro

Los siguientes temas no se abordan aquí y se reservan para encuentros posteriores:

- Herramientas especializadas para documentos (Encuentro 2)
- Futuro de la IA en el derecho (Encuentro 3)
- Arquitectura técnica de modelos o código fuente
- Comparativas entre herramientas de IA
- Historia detallada de la IA

---

## Concepto central del encuentro

> **"La IA no garantiza verdad: genera respuestas plausibles."**

Este es el mensaje que el encuentro debe dejar grabado en el participante antes de que use cualquier herramienta de IA en su trabajo judicial.

---

## Checklist de aprobación

Para aprobar este diseño, se solicita verificar que:

- [ ] Los 5 tópicos del programa del Día 1 están cubiertos con profundidad suficiente
- [ ] El encuentro es accesible para personal sin formación técnica
- [ ] El enfoque de demo proyectada por el docente es adecuado para el perfil del público
- [ ] El tratamiento de riesgos y confidencialidad es apropiado para el contexto judicial
- [ ] La inclusión de búsqueda de jurisprudencia como caso de uso es pertinente
- [ ] La advertencia sobre verificación de fallos es suficientemente enfática
- [ ] El Bloque 5b (flujo de privacidad en la demo de sentencia) es pertinente y el nivel de complejidad es apropiado
- [ ] El mensaje central del encuentro es correcto y completo

---

*Documento para revisión interna · versión preliminar · sujeto a ajustes según feedback*
