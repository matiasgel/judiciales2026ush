# Filminas: Encuentro 1 — Entender para no equivocarse

**Materia:** Inteligencia Artificial en el Poder Judicial de la Nación
**Duración:** 120 min
**Total de filminas:** 46

## PORTADA

---

### [F-00] Portada

@tipo: portada
@imagen: background
@prompt-imagen: Two abstract circular shapes overlapping on white background. Left circle dark bordo color with soft gradient. Right circle dark gray color with soft gradient. Subtle radial light from center. Flat minimalist style. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# Inteligencia Artificial en el Poder Judicial de la Nación

Encuentro 1 — Entender para no equivocarse

---

## BLOQUE 0 — Apertura

---

### [F-01] Agenda del día

@tipo: concepto-abstracto
@imagen: content
@prompt-imagen: Ten small horizontal rectangles arranged vertically as a checklist on the right side. Each rectangle dark bordo on white background. To the left of each, a small dark gray circle. Flat icon style. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# Lo que vamos a ver hoy

- Qué es la IA y dónde están ChatGPT, Claude y Gemini
- Herramientas y casos de uso en el Poder Judicial
- Primera mirada a ChatGPT
- Riesgos — caso real argentino (Rosario, 2025)
- Ventana de contexto
- Cómo escribir un buen prompt
- Configuraciones avanzadas y privacidad
- Sentencia en lenguaje claro y anonimización
- Cierre y mensaje clave

> La clase es enteramente proyectada vía Google Meet. No necesitás computadora ni celular.

---

## BLOQUE 1 — ¿Qué es la IA? Dónde están los LLMs

---

### [F-02] ¿Qué es la inteligencia artificial?

@tipo: concepto-abstracto
@imagen: content
@prompt-imagen: Four small flat icons arranged in a horizontal sequence on the right half of a white background. First icon: envelope dark bordo. Second icon: play triangle dark gray. Third icon: arrow turning dark bordo. Fourth icon: keyboard rectangle dark gray. All icons flat minimal style. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# Programas que aprenden a hacer tareas humanas

- Definición operativa: imitan capacidades que antes requerían inteligencia humana
- Ejemplos que ya usamos sin saberlo:
  - Filtro de spam del correo
  - Recomendaciones de Netflix
  - Autocomplete del teclado
  - Asistentes de voz del celular

---

### [F-03] El mapa de la IA — dónde están los LLMs

@tipo: diagrama
@imagen: content
@prompt-imagen: Four concentric circles centered on the right half of a white background. Outermost circle largest dark bordo thin outline. Second circle dark gray thin outline. Third circle bordo medium thickness. Innermost small filled bordo solid disk. All circles share the same center point. Clean geometric flat style. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# Círculos concéntricos: del universo más amplio al más específico

- **IA** — el universo entero: cualquier sistema que imita capacidades humanas
- **Machine Learning** — IA que aprende de ejemplos (filtro de spam, scoring crediticio)
- **Deep Learning** — ML con redes neuronales grandes (reconocimiento facial, traducción)
- **LLMs** — Deep Learning especializado en lenguaje: ChatGPT, Claude, Gemini, Copilot

> Cuando hoy alguien dice "IA", en el 90% de los casos habla de un LLM. Pero IA es mucho más grande.

---

### [F-04] Cómo funciona un LLM en una sola idea

@tipo: concepto-abstracto
@imagen: content
@prompt-imagen: Five small horizontal rectangles in a row on the right half of a white background. The first three rectangles dark bordo. The fourth rectangle dark gray with a thin dotted outline. The fifth rectangle white with bordo outline only. A small arrow connects each rectangle to the next, dark gray. Flat geometric minimalist. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# Un predictor de la palabra siguiente

- El modelo lee un texto y predice cuál palabra sigue, una y otra vez
- Lo hizo millones de veces sobre millones de textos durante el entrenamiento
- Por eso parece que entiende — pero está calculando probabilidades, no comprendiendo

> Ejemplo en vivo: "El acusado se presenta ante el..." → juez / tribunal / fiscal

---

### [F-05] Qué NO es un LLM

@tipo: tabla-comparativa

# La diferencia con un buscador o una base de datos

| | Buscador (Google) | Base de datos (SAIJ, Lex Doctor) | LLM (ChatGPT) |
|---|---|---|---|
| **Qué hace** | Encuentra | Almacena hechos verificados | Genera texto probable |
| **Garantiza verdad** | Sigue la fuente | Sí (lo que está cargado) | **No — puede inventar** |
| **Cita la fuente** | Sí (link) | Sí (registro) | A veces — y puede mentir sobre ella |
| **Necesita conexión** | Sí | Depende | Sí |

---

### [F-06] Glosario de bolsillo

@tipo: concepto-abstracto
@imagen: content
@prompt-imagen: Three small flat icons stacked vertically on the right side of a white background. First icon: a small filled square bordo. Second icon: a chat bubble outline dark gray. Third icon: a starburst shape bordo. All flat minimal style. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# Tres palabras que vamos a usar toda la clase

- **LLM** — Modelo de Lenguaje Grande. ChatGPT, Claude, Gemini y similares
- **Prompt** — lo que vos le escribís al modelo
- **Alucinación** — cuando el modelo inventa algo que suena creíble pero es falso

---

## BLOQUE 2 — Herramientas de IA y usos en el Poder Judicial

---

### [F-07] Panorama actual de herramientas

@tipo: tabla

# Las cinco más relevantes para trabajo administrativo y judicial

| Herramienta | Quién la hace | Para qué sirve | Navegador |
|---|---|---|---|
| **ChatGPT** | OpenAI | Conversación, redacción, análisis de texto | chatgpt.com |
| **Claude** | Anthropic | Textos largos, raciocinio jurídico | claude.ai |
| **Gemini** | Google | Conversación integrada con servicios Google | gemini.google.com |
| **NotebookLM** | Google | "Cuaderno" con documentos propios cargados | notebooklm.google.com |
| **Copilot** | Microsoft | Integrado en Word, Outlook, Edge | Microsoft 365 |

> Usamos ChatGPT como ejemplo principal. Lo que aprendan se aplica casi igual al resto.

---

### [F-08] Casos de uso concretos en el PJN

@tipo: concepto-abstracto
@imagen: content
@prompt-imagen: Six small flat icons arranged in two columns of three on the right half of a white background. Each icon a different abstract shape: a rectangle, a folded page corner, a horizontal arrow, a magnifying loop, a globe outline, an open mouth bubble. Three icons dark bordo, three icons dark gray, alternating. Clean flat minimalist style. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# Seis usos que ya hacen otros compañeros

1. **Redacción de oficios** — borrador inicial a partir de datos básicos
2. **Resumen de expedientes** — síntesis por tema (atención: datos sensibles → Bloque 3)
3. **Mejora de redacción** — lenguaje más claro, formal o accesible
4. **Búsqueda de jurisprudencia** — organizar criterios (verificar siempre en SAIJ/InfoJus)
5. **Traducción** de documentos extranjeros
6. **Explicar tecnicismos** a partes no profesionales (lo vemos en Bloque 5b)

---

### [F-09] Encuadre human-first

@tipo: concepto-abstracto
@imagen: background
@prompt-imagen: A large soft circle filling most of the slide, dark bordo with subtle radial gradient on white background. In the center a small filled bordo dot. Around the dot a thin dark gray circular ring. Flat minimalist. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# La IA produce borradores. La firma es humana.

- En todos estos casos la IA propone — no decide
- La firma, el criterio jurídico y la decisión son siempre humanos
- Si una IA decide en el Poder Judicial, dejamos de tener Poder Judicial

---

## BLOQUE 2b — Primera mirada a ChatGPT

---

### [F-10] Acceso — chatgpt.com

@tipo: demo
@imagen: none

# No se instala nada. Una cuenta gratuita alcanza.

## Cómo entrar

- Abrir cualquier navegador (Chrome, Firefox, Edge)
- Ir a **chatgpt.com**
- Crear cuenta gratuita con correo o cuenta Google
- La interfaz cambia cada pocos meses — los elementos clave siempre están

> El docente lo muestra vía Google Meet (compartir pantalla desde la laptop).

---

### [F-11] Mapa de la interfaz de ChatGPT

@tipo: diagrama
@imagen: content
@prompt-imagen: Stylized rectangle representing a browser window on the right half of a white background. Inside it: a narrow vertical strip on the left dark gray representing a sidebar. A large central rectangle white representing the conversation area. A long horizontal rounded rectangle at the bottom bordo representing an input box. A small circle in the top right corner dark gray representing a profile icon. Five small thin arrows in dark bordo pointing to each element from outside. Flat minimalist diagram style. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# Cinco lugares que conviene ubicar

- **Barra lateral izquierda** — historial de conversaciones
- **Área central** — la conversación en curso
- **Caja de texto inferior** — donde se escribe el prompt
- **Selector de modelo (arriba)** — GPT-4o, GPT-4o mini. Dejar el que viene por defecto
- **Botón "New chat"** — abre una conversación nueva, memoria en blanco
- **Ícono de perfil (arriba a la derecha)** — Settings, controles de privacidad (Bloque 4b)

---

### [F-12] Tres reglas básicas antes de usar ChatGPT

@tipo: concepto-abstracto
@imagen: content
@prompt-imagen: Three numbered shapes stacked vertically on the right half of a white background. First shape: a shield outline bordo. Second shape: a pencil mark dark gray. Third shape: a small gear outline bordo. Each shape isolated. Flat minimalist icon style. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# Lo que conviene tener claro desde el primer prompt

1. **No pegar información sensible de expedientes** (Bloque 3)
2. Lo que genera es un **borrador** — siempre revisar
3. **Revisar los controles de privacidad** antes de usar con tareas del PJN (Bloque 4b)

---

## BLOQUE 3 — Riesgos: el humano decide primero

---

### [F-13] Principio rector del bloque y del encuentro

@tipo: socratica
@imagen: background
@prompt-imagen: A large central irregular blob shape dark bordo with soft edges on white background. Around it three small dark gray dots arranged at varying distances. Subtle radial gradient. Flat minimalist abstract. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# El humano decide primero

La IA propone. La persona valida, decide y firma.

---

### [F-14] Riesgo 1 — Alucinaciones

@tipo: concepto-abstracto
@imagen: content
@prompt-imagen: A small page outline dark gray on the right side of a white background. From inside the page three small irregular blobs emerge dark bordo, increasing in size from bottom to top. Flat minimalist icon style. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# El modelo inventa información que suena creíble

- Especialmente peligroso con fallos, artículos legales, números de expediente
- La IA escribe con la misma seguridad cuando dice verdad y cuando inventa
- No avisa cuándo está alucinando

> El modelo escribe con la confianza de quien sabe — aunque no sepa.

---

### [F-15] Caso argentino real — Cámara Civil de Rosario, agosto 2025

@tipo: socratica
@imagen: background
@prompt-imagen: A central rectangular shape dark bordo with subtle texture on white background, suggesting a closed page or document. Around it, soft empty space. A thin dark gray line frames it on the right side only. Flat minimalist. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# Juez Oscar Puccinelli — cita textual

> "Es sumamente riesgoso y hasta temerario delegar la labor de búsqueda de jurisprudencia de soporte y luego volcarla sin cotejar la fuente."

## Qué pasó

- Un abogado presentó apelación con jurisprudencia **inexistente** generada por ChatGPT
- Reconoció que no verificó las citas
- **Resultado:** apelación rechazada, reprensión, notificación al Tribunal de Ética

---

### [F-16] El caso no fue único — Argentina ya tiene jurisprudencia propia

@tipo: timeline
@imagen: none

# Casos similares replicados en distintos fueros

| Caso | Fuero / Provincia | Año | Sanción |
|---|---|---|---|
| Cámara Civil Rosario (Puccinelli) | Civil — Santa Fe | 2025 | Reprensión + Tribunal de Ética |
| Cipolletti (Río Negro) | Civil — Río Negro | 2025 | Dos abogados sin honorarios |
| Otros fueros del país | Varias provincias | 2024–2025 | Múltiples episodios documentados |

> El precio profesional de no verificar lo que dice la IA ya tiene jurisprudencia.

---

### [F-17] Riesgo 2 — Confidencialidad y datos sensibles

@tipo: concepto-abstracto
@imagen: content
@prompt-imagen: A small lock shape dark bordo on the right side of a white background. Above and below the lock, two small horizontal lines dark gray representing data flow. A thin dotted dark gray line crosses the scene diagonally. Flat minimalist icon style. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# Lo que pegás en ChatGPT puede usarse para reentrenar al modelo

- Configuración por defecto de cuenta personal = los chats se usan para entrenamiento
- **Implicancia en PJN:**
  - Datos de partes, testigos, menores
  - Secreto de sumario
  - Datos médicos
- **Regla humana primero:** qué sale del sistema lo decide la persona, nunca por reflejo

> Bloque 4b: cómo desactivar el entrenamiento. Bloque 5b: cuándo anonimizar.

---

### [F-18] Riesgo 3 — Sesgos

@tipo: concepto-abstracto
@imagen: content
@prompt-imagen: A horizontal line dark gray across the middle of the right half of a white background. Above the line three small irregular dark bordo dots clustered together. Below the line one isolated dark bordo dot. Flat minimalist abstract. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# La IA reproduce sesgos del texto con que se entrenó

- Sesgos de género, etnia, clase social
- Pueden aparecer en redacción de resoluciones, descripciones de personas, evaluaciones
- **Regla humana primero:** la persona revisa el lenguaje del borrador antes de firmar
- No se acepta texto generado sin lectura crítica

---

### [F-19] Riesgo 4 — Confianza excesiva / dependencia

@tipo: concepto-abstracto
@imagen: content
@prompt-imagen: A small upward arrow shape bordo on the right side of a white background, gradually increasing in opacity from bottom to top. To its left, a small magnifying loop outline dark gray, fading. Flat minimalist abstract. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# "Si lo dijo la IA, debe ser verdad" — el reflejo más peligroso

- Con el tiempo se pierde el hábito de verificar
- El caso de Rosario es ilustrativo: el abogado actuó con la confianza de que ChatGPT decía jurisprudencia real
- **Regla humana primero:** leer críticamente lo que escribe la IA, como se leería un borrador de un practicante nuevo

---

### [F-20] Riesgo 5 — Trazabilidad y responsabilidad

@tipo: concepto-abstracto
@imagen: content
@prompt-imagen: A single signature loop shape dark bordo on the right half of a white background, drawn as one continuous flowing line. Below it a thin dark gray horizontal line. Flat minimalist abstract. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# La firma humana implica asumir todo el contenido como propio

- Si una IA "sugirió" un texto que se firmó, la responsabilidad sigue siendo del firmante
- No hay "culpa de la IA" — los abogados sancionados en Rosario y Río Negro no pudieron alegarla
- **Síntesis del bloque:** la IA propone borradores. El humano decide, valida y firma.

> Si quitamos al humano del medio, perdemos el control de la justicia.

---

## BLOQUE 4 — Ventana de contexto

---

### [F-21] Qué es la ventana de contexto

@tipo: concepto-abstracto
@imagen: content
@prompt-imagen: A horizontal rectangle dark gray outline on the right half of a white background, suggesting a board. Inside the rectangle, several small irregular bordo strokes scattered. A thin dotted dark gray line below the rectangle suggests erasure. Flat minimalist abstract. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# La memoria de trabajo de la IA durante una conversación

- Metáfora: el **pizarrón que se borra entre clases**
- Mientras estás en una conversación, el modelo ve todo lo escrito hasta ese momento
- Cuando cerrás el chat, el pizarrón se borra: la próxima vez no recuerda nada

---

### [F-22] Por qué importa en el PJN

@tipo: concepto-abstracto
@imagen: content
@prompt-imagen: Two horizontal rectangles stacked on the right half of a white background. Top rectangle small dark bordo. Bottom rectangle wide dark gray with detail texture. An arrow between them dark gray pointing from top to bottom. Flat minimalist abstract. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# Sin contexto, el resultado es genérico o inventado

- "Redactá un oficio" sin más → la IA no sabe nada del caso
- Hay que darle el contexto cada vez:
  - Tipo de causa
  - Partes intervinientes
  - Datos relevantes del expediente
  - Resultado esperado
- **Límite práctico:** modelos actuales aceptan docs largos, pero "olvidan" lo del principio en textos muy extensos

---

### [F-23] Regla práctica y puente al prompting

@tipo: concepto-abstracto
@imagen: content
@prompt-imagen: A small filled bordo arrow pointing right on the right half of a white background. Behind it a soft dark gray trail fading from left to right. Flat minimalist abstract. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# Si el contexto es clave, el prompt tiene que llevarlo todo

- Trozos manejables y pedidos específicos
- El contexto se da explícitamente, en cada conversación
- Esto nos lleva directo al prompting estructurado

---

## BLOQUE 5 — Introducción al prompting

---

### [F-24] Por qué la forma de pedir afecta el resultado

@tipo: concepto-abstracto
@imagen: content
@prompt-imagen: Two small irregular bordo shapes on the right half of a white background. Left shape blurry and ill-defined, fading edges. Right shape crisp, sharp, geometrically clear. A thin dark gray line separates them vertically. Flat minimalist abstract. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# La IA responde con la granularidad que le dás

- Orden vaga → respuesta genérica
- Instrucción precisa con contexto y restricciones → borrador útil
- Esto se llama **prompt engineering**
- Es la habilidad clave para usar bien cualquier LLM

> Recordatorio human-first: todo lo que sigue produce **borradores**.

---

### [F-25] Plantilla del prompt — cinco componentes

@tipo: concepto-abstracto
@imagen: content
@prompt-imagen: Five small horizontal rectangles stacked vertically on the right half of a white background. From top to bottom: first rectangle dark bordo, second dark gray, third dark bordo, fourth dark gray, fifth dark bordo. Each rectangle isolated, with thin connecting lines between them. Flat minimalist diagram style. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# Rol + Tarea + Contexto + Restricciones + Plantilla de salida

- **Rol** — desde qué perspectiva actúa el modelo ("Sos asistente redactor del PJN")
- **Tarea** — acción concreta ("reescribí", "resumí", "listá")
- **Contexto** — información de fondo del caso
- **Restricciones** — qué no hacer ("sin latinismos", "máximo 3 párrafos")
- **Plantilla de salida** — estructura esperada del resultado

> Esta filmina queda visible durante todas las demos siguientes.

---

### [F-26] Demo 1 — Prompt vago vs. prompt estructurado

@tipo: demo

# Misma IA, dos resultados muy distintos

## Prompt vago

```
Redactá un oficio.
```

## Prompt estructurado

```
Sos asistente redactor del PJN. Redactá un oficio de citación a testimonio
para el juzgado de familia N.º 3 de Ushuaia. El convocado es [NOMBRE],
la causa es [NÚMERO], la fecha de audiencia es [FECHA] a las [HORA].
Usá lenguaje formal, sin tuteo, con la fórmula de cierre:
'Sin otro particular, saludo a Ud. atte.' No uses latinismos.
```

> La diferencia no está en la IA — está en la instrucción.

---

### [F-27] Demo 2 — Restricción de confidencialidad

@tipo: demo

# Las restricciones controlan el comportamiento antes de generar

## Línea agregada al prompt anterior

```
No hagas referencia a ningún dato del expediente en el asunto
ni en el cuerpo del correo — sólo en el adjunto.
```

## Resultado

- La respuesta respeta exactamente esa restricción
- **No hace falta confiar en la IA — hace falta darle las reglas correctas desde el inicio**

---

### [F-28] Construcción colectiva — armemos un prompt entre todos

@tipo: socratica
@imagen: background
@prompt-imagen: Five small dark bordo dots and three dark gray dots scattered organically on a white background, connected by thin dark gray lines suggesting collaboration. Subtle empty space around. Flat minimalist abstract. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# ¿Qué tarea querés automatizar?

- Pensá una tarea cotidiana: oficio, informe, correo formal, notificación
- La armamos juntos en los 5 componentes
- Si el tiempo lo permite, la lanzamos en ChatGPT en vivo

> No es magia — es estructura.

---

## BLOQUE 4b — Configuraciones de ChatGPT

---

### [F-29] Cómo cambió ChatGPT en los últimos meses

@tipo: concepto-abstracto
@imagen: content
@prompt-imagen: A central small bordo circle on the right half of a white background. Around it four orbiting smaller shapes: a square dark gray, a triangle dark bordo, a diamond dark gray, a tiny gear outline dark bordo. Connecting thin lines between them. Flat minimalist abstract. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# Ya no es "un chat" — es una plataforma con varios modos

- Chat normal
- GPTs personalizados
- Modo agente
- Búsqueda profunda
- Controles de privacidad granulares

> Conviene saber que existen — aunque no se usen todas hoy.

---

### [F-30] Función 1 — GPTs personalizados

@tipo: demo

# Un "ChatGPT a medida" que se configura una vez

## Qué es

- Instrucciones fijas guardadas: rol, tono, reglas, plantilla
- Se reutiliza: alcanza con dar los datos del caso
- Requiere cuenta Plus

## Demo proyectada — GPT "Redactor de Oficios PJN"

```
Prompt corto:
"Oficio a la Secretaría de Trabajo por incumplimiento contractual,
expediente 12345/2025, plazo 5 días."
```

- La IA responde directamente con la plantilla completa
- **Regla humano primero:** el GPT es un atajo, el contenido sigue siendo revisado

---

### [F-31] Función 2 — Modo agente

@tipo: concepto-abstracto
@imagen: content
@prompt-imagen: A small dark bordo robot-like outline on the right side of a white background, simplified to geometric shapes: rectangle body, two circles for eyes, two thin lines as antennas. Around it three small dark gray arrows pointing outward. Flat minimalist icon. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# ChatGPT que ejecuta pasos por su cuenta

- Abre páginas, llena formularios, descarga archivos, encadena acciones
- **Ejemplo PJN:** "buscame los últimos 5 fallos sobre tenencia compartida y armame una planilla"

## Advertencias críticas

- Puede equivocarse en pasos intermedios sin avisar
- **Nunca dejarlo operar sobre sistemas internos del PJN ni con credenciales institucionales**
- Hoy: sólo tareas exploratorias con datos públicos

---

### [F-32] Función 3 — Búsqueda profunda (Deep Research)

@tipo: concepto-abstracto
@imagen: content
@prompt-imagen: A small open book outline dark gray on the right half of a white background. Above the book three small irregular bordo shapes radiating outward like rising particles. Flat minimalist icon. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# Informes extensos con citas verificables

- Tarda varios minutos investigando múltiples fuentes
- Produce un documento estructurado con referencias
- **Ejemplo PJN:** "investigación profunda sobre la evolución de la doctrina de prisión preventiva en los últimos 5 años"

> Limitación crítica: también puede equivocarse o citar fuentes mal interpretadas. Las citas se verifican una por una — recordar el caso Rosario.

---

### [F-33] Función 4 — Privacidad: el problema en una frase

@tipo: concepto-abstracto
@imagen: content
@prompt-imagen: A small open lock shape dark bordo on the right half of a white background. Behind it a faded dark gray cloud shape. A thin dotted bordo line connects them. Flat minimalist icon. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# Todo lo que escribís puede ser usado para entrenar futuros modelos

- En **cuenta personal con configuración de fábrica**, los chats se usan para entrenamiento
- Para un usuario común es un problema menor
- Para alguien que pega texto de expediente es un problema grave
- **Bueno saberlo: estos controles existen, hay que activarlos**

---

### [F-34] Control 1 — Desactivar entrenamiento sobre chats propios

@tipo: demo

# Settings → Data Controls → "Improve the model for everyone" OFF

## Pasos (demo en vivo en la pantalla real de ChatGPT)

1. Clic en ícono de perfil (arriba a la derecha)
2. **Settings**
3. **Data Controls**
4. Desactivar el toggle **"Improve the model for everyone"**

## Efecto

- Las conversaciones siguen guardándose en tu historial
- **OpenAI ya no las usa para entrenar**
- Existe en versión gratuita y Plus
- **No viene activado por defecto** — hay que activarlo explícitamente

---

### [F-35] Control 2 — Chat temporal

@tipo: demo

# El "modo incógnito" de ChatGPT

## Cómo activarlo

- Botón al iniciar un chat nuevo → **Chat temporal**
- O ícono de modo temporal en la cabecera

## Efecto

- **No se guarda en el historial**
- **No se usa para entrenar**
- **No genera memoria persistente**
- Se elimina automáticamente en 30 días

## Caso de uso PJN

- Consultas puntuales con texto sensible que no convenga dejar rastro

---

### [F-36] Control 3 — Memoria entre chats

@tipo: demo

# ChatGPT puede "recordar" cosas de chats anteriores

## Dónde está

- Settings → **Personalization** → **Memory**
- Permite activar / desactivar / borrar memorias específicas

## Recomendación para uso PJN

- **Desactivar** o revisar periódicamente
- No queremos que el modelo conserve fragmentos de casos previos entre sesiones

---

### [F-37] Control 4 — Cuentas Business / Enterprise / Edu

@tipo: concepto-abstracto
@imagen: content
@prompt-imagen: A small rectangular shield outline dark bordo on the right half of a white background. Inside the shield a small dark gray dot centered. Around the shield three small bordo dots arranged in a triangle. Flat minimalist icon. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# Protección automática en planes comerciales

- **Por defecto, Business / Team / Enterprise / Edu NO usan datos del usuario para entrenar**
- El contrato comercial activa esa protección automáticamente
- **Implicancia institucional:** si el PJN contrata ChatGPT a nivel institucional, hereda esta protección
- En cambio, **cuenta personal de un agente requiere la configuración manual** de los controles 1–3

> La privacidad en ChatGPT no es automática en cuentas personales — hay que activarla.

---

### [F-38] Cuándo usar cada modo

@tipo: tabla-comparativa

# Tabla de decisión rápida

| Tarea | Modo recomendado |
|---|---|
| Redactar un texto recurrente con formato fijo (oficios, cédulas) | **GPT personalizado** |
| Recolectar datos públicos de varias páginas en una tabla | **Modo agente** (con verificación) |
| Producir un informe doctrinario o de panorama extenso | **Búsqueda profunda** |
| Consulta puntual con texto sensible que no debe quedar en historial | **Chat temporal** |
| Pregunta rápida, ajuste de redacción, traducción | Chat normal (con "Improve the model" OFF) |

---

## BLOQUE 5b — Sentencia en lenguaje claro y anonimización

---

### [F-39] El problema del lenguaje judicial

@tipo: concepto-abstracto
@imagen: content
@prompt-imagen: Two small rectangle outlines stacked vertically on the right half of a white background. Top rectangle dense with many short horizontal lines dark gray inside, suggesting compact text. Bottom rectangle with fewer, longer horizontal lines dark bordo inside, suggesting clearer spacing. A small arrow dark gray pointing from top to bottom. Flat minimalist abstract. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# Las sentencias están escritas para abogados — las partes también tienen derecho a entender

- El lenguaje claro es política pública en varios tribunales argentinos
- Permite que las partes entiendan qué se decidió sobre su caso
- La IA puede acelerar la reescritura — el contenido jurídico lo sigue decidiendo el magistrado

---

### [F-40] Demo en vivo — sentencia ficticia a lenguaje claro

@tipo: demo

# Texto ficticio → ChatGPT → versión accesible

## Prompt reutilizable

```
Reescribí este fragmento de resolución judicial en lenguaje claro,
usando oraciones cortas, voz activa, sin latinismos y sin perder
ningún dato sustancial. Conservá la estructura: encabezado, hechos,
decisión, fundamento.

[pegar fragmento de resolución ficticia]
```

## Observación pedagógica

- La IA devuelve la versión en lenguaje claro en segundos
- El docente lee en voz alta y compara con el original
- **Regla humano-primero:** ¿perdió algún matiz? ¿cambió el sentido de alguna cláusula?

---

### [F-41] ¿Y si el texto tiene datos sensibles? — Concepto de anonimización

@tipo: tabla-comparativa

# Reemplazar datos reales por etiquetas genéricas antes de pegar

| Texto original | Texto anonimizado |
|---|---|
| La parte actora, **María González Díaz**, | La parte actora, **PERSONA_1**, |
| domiciliada en **Av. Mitre 1234 de Rosario**, | domiciliada en **DIRECCIÓN_1**, |
| representada por el Dr. **Juan Pérez** | representada por el Dr. **PERSONA_2** |

## Flujo

1. Anonimizar el texto (búsqueda y reemplazo manual en un editor)
2. Pegar en ChatGPT → la IA trabaja solo con etiquetas
3. Sustituir las etiquetas por los datos reales antes de usar el documento

---

### [F-42] Cuándo anonimizar en el PJN

@tipo: concepto-abstracto
@imagen: content
@prompt-imagen: Four small symbolic shapes arranged in a vertical column on the right half of a white background. Top shape a small triangle dark bordo. Second a small circle dark gray. Third a small square dark bordo. Bottom a small diamond dark gray. All isolated, flat minimalist icons. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# Casos del PJN que requieren anonimización previa

- Expedientes con **datos de menores** → obligación legal de reserva
- **Víctimas o testigos con protección de identidad** → dato que no debe circular
- **Datos médicos y psicológicos** de las partes → sensibilidad especial
- **Secreto de sumario** → el contenido no debe salir del sistema judicial

> La anonimización es una **segunda capa** sobre los controles de privacidad — no son excluyentes, se complementan.

---

### [F-43] Reflexión final — uso responsable de IA en el contexto judicial

@tipo: concepto-abstracto
@imagen: background
@prompt-imagen: Two large overlapping soft circles on a white background, one dark bordo with soft gradient, one dark gray with soft gradient. Where they overlap a subtle deeper bordo tone. Flat minimalist abstract. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# Velocidad de la IA + criterio humano + protección de datos

- La IA acelera la reescritura
- El magistrado o magistrada sigue decidiendo el contenido jurídico
- La anonimización garantiza que el proceso no comprometa datos sensibles

> Las tres cosas juntas hacen que el uso de IA en el ámbito judicial sea **responsable**.

---

## BLOQUE 6 — Cierre

---

### [F-44] Los 7 conceptos clave del día

@tipo: concepto-abstracto
@imagen: content
@prompt-imagen: Seven small dark bordo dots arranged in a vertical column on the right side of a white background. Each dot connected to the next with a thin dark gray line. Flat minimalist abstract. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# Lo que te llevás de hoy

1. **LLMs (ChatGPT, Claude, Gemini)** son una rama del Deep Learning dentro de la IA
2. La IA genera texto **probable** — no garantiza verdad. Rosario 2025 ya tiene consecuencias profesionales
3. **El humano decide primero**: la IA propone, la persona valida, decide y firma
4. **Nunca pegar datos reales** en un chat público; cuando sea imprescindible, anonimizar antes
5. **Privacidad no es automática** en cuentas personales — activar Data Controls
6. El **contexto del prompt** determina la calidad de la respuesta
7. ChatGPT tiene **modos especializados** — GPTs, agente, búsqueda profunda

---

### [F-45] Mensaje clave final

@tipo: cierre
@imagen: background
@prompt-imagen: A single large dark bordo shape centered on a white background, soft circular form with subtle radial gradient from center outward. Around it a thin dark gray halo line. Flat minimalist abstract. No text whatsoever. No letters, no labels, no code, no numbers. High resolution.

# La IA no garantiza verdad: genera respuestas plausibles

El humano decide primero.

> Nos vemos en el Encuentro 2. El link a los prompts usados queda en el grupo institucional.
