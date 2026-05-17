# Diseño: Encuentro 1 — Entender para no equivocarse
<!-- STATUS: BORRADOR -->

## Metadatos
- **Tema:** 01 — encuentro-1
- **Título completo:** Encuentro 1 — Entender para no equivocarse
- **Materia:** Inteligencia Artificial en el Poder Judicial de la Nación
- **Institución:** Poder Judicial de la Nación
- **Duración estimada:** 120 minutos ← _referencia orientativa; el docente suele completar el contenido en menos tiempo — no usarla como constraint rígido de generación_
- **Público:** Usuarios sin experiencia previa o con bajo nivel técnico
- **Perfil docente:** Licenciado en Informática, investigador docente en IA
- **Fecha de diseño:** 2026-04-27

---

## Objetivo general del encuentro

Brindar a los participantes una comprensión básica y operativa de la inteligencia artificial y sus riesgos, para que puedan tomar decisiones informadas sobre su uso en el entorno judicial.

---

## Objetivos específicos de aprendizaje

Al finalizar el encuentro, el participante podrá:

1. Explicar con sus propias palabras qué es la inteligencia artificial, ubicar a los LLMs (ChatGPT, Claude, Gemini) dentro del mapa general de la IA y diferenciarlos de un buscador o base de datos.
2. Identificar al menos dos casos de uso concreto de IA en tareas del Poder Judicial de la Nación y reconocer las herramientas más relevantes disponibles hoy.
3. Nombrar los principales riesgos del uso de IA en contextos legales (alucinaciones, confidencialidad, sesgos, dependencia) y aplicar el principio "el humano decide primero", apoyándose en un caso real de la justicia argentina.
4. Describir qué es la ventana de contexto y cómo afecta la calidad de la respuesta.
5. Reconocer las configuraciones actuales de ChatGPT — GPTs personalizados, modo agente, búsqueda profunda y controles de privacidad de datos — y entender para qué sirve cada una, incluyendo cómo desactivar el entrenamiento sobre conversaciones propias.
6. Formular un prompt básico con estructura: rol + tarea + contexto + restricciones + plantilla de salida.

---

## Indicadores de logro

> Señales observables durante la clase que confirman que los objetivos se están cumpliendo. Útiles para que el docente calibre el ritmo en tiempo real.

| Objetivo | Indicador observable |
|----------|---------------------|
| Entender qué es la IA y ubicar a los LLMs | El participante puede dibujar (o explicar) la jerarquía IA → Machine Learning → LLMs y nombrar al menos un ejemplo de cada nivel |
| Identificar casos de uso y herramientas en el PJN | Menciona al menos una herramienta (ChatGPT, Claude, Gemini, NotebookLM, Copilot) y un caso de uso propio de su área |
| Nombrar riesgos y aplicar "humano primero" | Puede decir "alucinación", "confidencialidad" y completar la frase "la IA propone, el humano _______" (decide / valida / firma). Recuerda el caso del abogado sancionado en Rosario por citar fallos inventados por ChatGPT |
| Ventana de contexto | Explica por qué el modelo "se olvida" entre sesiones sin necesidad de repregunta |
| Configuraciones de ChatGPT | Diferencia oralmente las funciones: GPT personalizado, modo agente, búsqueda profunda y controles de privacidad ("que no entrene con mis datos", chat temporal) — con un ejemplo de cuándo conviene cada una |
| Formular un prompt | En la construcción colectiva del Bloque 5, el grupo dicta los componentes (rol, tarea, contexto, restricciones, plantilla de salida) sin que el docente los nombre |

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

## Distribución de tiempo (120 min) — clase corrida sin pausa

| Bloque | Nombre | Duración | Tipo |
|--------|--------|----------|------|
| 0 | Apertura y presentación del día | 5 min | Encuadre |
| 1 | ¿Qué es la IA? Dónde están los LLMs | 15 min | Conceptual |
| 2 | Herramientas de IA y usos en el Poder Judicial | 10 min | Aplicado |
| 2b | Primera mirada a ChatGPT: la interfaz | 7 min | Práctico introductorio |
| 3 | Riesgos — el humano decide primero (caso argentino real) | 15 min | Crítico / Preventivo |
| 4 | Ventana de contexto | 6 min | Conceptual |
| 5 | Introducción al prompting | 22 min | Práctico |
| 4b | Configuraciones de ChatGPT: GPTs, agente, búsqueda profunda y **privacidad** | 15 min | Demostrativo / Panorama |
| 5b | Demo: sentencia en lenguaje claro + anonimización de datos (concepto) | 13 min | Práctico / Conceptual |
| 6 | Cierre, preguntas y mensaje clave | 12 min | Síntesis |
| **Total** | | **120 min** | |

> **Decisión pedagógica — reordenamiento:** el Bloque 5 (prompting) se dicta **antes** que el Bloque 4b (funciones avanzadas). Razón: es más natural aprender a escribir prompts con la interfaz básica de ChatGPT antes de conocer sus modos especializados. El Bloque 2b introduce la interfaz; el Bloque 5 la usa para prompting; recién entonces el Bloque 4b muestra las configuraciones avanzadas como extensiones de lo aprendido.

> **Perfil docente:** Ritmo ágil. Si el grupo manifiesta cansancio cerca del minuto 80 (después de los bloques prácticos 2b + 5), el docente puede tomar una micropausa informal de 2–3 minutos — esos minutos salen de la ventana de holgura del Bloque 6.

> **Regla de scope:** Cualquier contenido no listado en la tabla anterior está fuera de scope de este encuentro.

---

## Descripción por bloque

### Bloque 0 — Apertura (5 min)
- Presentación del docente y del programa del encuentro
- Pregunta inicial al público: "¿Alguien ya usó ChatGPT o una IA? ¿Para qué?"
- El docente registra mentalmente cuántos levantan la mano para calibrar el ritmo de los primeros bloques
- Objetivo: romper el hielo y activar conocimientos previos. Anticipa que la clase es **enteramente proyectada vía Google Meet** — no se requiere computadora ni celular para seguirla

### Bloque 1 — ¿Qué es la IA? Dónde están los LLMs (15 min)

**Subtemas:**
- **Qué es la inteligencia artificial** (3 min): definición operativa sin tecnicismos — "programas que aprenden a hacer tareas que antes requerían inteligencia humana". Ejemplos cotidianos que la gente ya usa sin saberlo: filtro de spam del correo, recomendaciones de Netflix, autocomplete del teclado.
- **El mapa de la IA — dónde están los LLMs** (5 min): diagrama de círculos concéntricos que el docente explica de afuera hacia adentro:
  - **IA (Inteligencia Artificial)** — el universo entero: cualquier sistema que imita capacidades humanas (reconocer caras, traducir, decidir rutas).
  - **Machine Learning (Aprendizaje Automático)** — IA que aprende de ejemplos en vez de seguir reglas escritas. Ej: filtro de spam, sistemas de scoring crediticio.
  - **Deep Learning (Aprendizaje Profundo)** — ML con redes neuronales grandes. Ej: reconocimiento facial, traducción automática.
  - **LLMs (Modelos de Lenguaje Grandes)** — una rama del Deep Learning especializada en lenguaje. Ej: **ChatGPT, Claude, Gemini, Copilot**. Esto es lo que vamos a usar en la cursada.
  > **Frase clave del docente:** "Cuando alguien dice IA en una conversación hoy, en el 90% de los casos está hablando de un LLM. Pero IA es mucho más grande — los LLMs son una herramienta dentro de un universo más amplio."
- **Cómo funciona un LLM en una sola idea** (4 min): la metáfora del "predictor de palabras". Un LLM mira un texto y predice cuál es la palabra más probable que sigue, una y otra vez. Ejemplo en vivo: el docente proyecta vía Google Meet la frase "El acusado se presenta ante el..." y pregunta al grupo qué palabra va. El grupo dice "juez", "tribunal", "fiscal". Eso es exactamente lo que hace un LLM — con la diferencia de que vio millones de textos antes.
- **Qué NO es un LLM** (3 min): tabla comparativa simple en pantalla.

| | Buscador (Google) | Base de datos (Lex Doctor, Saij) | LLM (ChatGPT) |
|---|---|---|---|
| **Qué hace** | Encuentra | Almacena hechos verificados | Genera texto probable |
| **Garantiza verdad** | Sigue una fuente | Sí (lo que está cargado) | **No** — puede inventar |
| **Necesita conexión** | Sí | Depende | Sí |
| **Cita la fuente** | Sí (link) | Sí (registro) | A veces — y puede mentir sobre ella |

- **Glosario de bolsillo** (2 min): 3 palabras que se van a usar toda la clase — el docente las dice en voz alta y deja la slide visible:
  - **LLM** = Modelo de Lenguaje Grande (ChatGPT y similares)
  - **Prompt** = lo que vos le escribís al modelo
  - **Alucinación** = cuando el modelo inventa algo que suena creíble pero es falso

**Objetivo de bloque:** Que el participante ubique a ChatGPT y similares en el mapa general de la IA, entienda que un LLM genera texto probable (no verdad verificada) y maneje 3 términos clave para el resto de la clase.

**Estrategia pedagógica:** Exposición con 1 diagrama visual (círculos concéntricos), 1 demo rápida de predicción de palabras proyectada vía Google Meet y 1 tabla comparativa. Sin profundizar en historia, arquitectura ni matemática.

**Filminas estimadas:** 5–6 (portada del bloque, diagrama de círculos concéntricos, predictor de palabras, tabla comparativa buscador/BD/LLM, glosario)

> **Nota de tiempo:** se recortaron 2 minutos del Bloque 1 original. Si el grupo está muy activo con preguntas, el docente condensa la tabla comparativa y avanza — el Bloque 2b retoma la herramienta en pantalla.

### Bloque 2 — Herramientas de IA y usos en el Poder Judicial (10 min)

**Subtemas:**
- **Panorama actual de herramientas de IA generativa** (3 min): el docente comparte vía Google Meet una slide con las herramientas más relevantes para trabajo administrativo y judicial, agrupadas por para qué sirven:

| Herramienta | Quién la hace | Para qué sirve principalmente | Disponible en navegador |
|---|---|---|---|
| **ChatGPT** | OpenAI | Conversación general, redacción, análisis de texto | Sí (chatgpt.com) |
| **Claude** | Anthropic | Conversación general, textos largos, raciocinio jurídico | Sí (claude.ai) |
| **Gemini** | Google | Conversación integrada con servicios Google | Sí (gemini.google.com) |
| **NotebookLM** | Google | "Cuaderno" donde se cargan documentos propios y la IA responde sólo en base a esos documentos | Sí (notebooklm.google.com) |
| **Copilot** | Microsoft | Integrado en Word, Outlook, Edge | En productos Microsoft 365 |

  > **Aclaración del docente:** "En esta cursada vamos a usar ChatGPT como ejemplo principal porque es la más difundida y la que más configuraciones tiene para el tipo de trabajo que hacemos, pero todo lo que aprendan se aplica casi igual al resto. Existen otras herramientas (por ejemplo, motores de búsqueda potenciados por IA); las dejamos fuera para no dispersarnos."

- **Casos de uso concretos en el PJN** (5 min): el docente repasa con 1 slide por caso y comenta cuándo lo usó él u otros docentes:
  1. **Redacción de oficios** — borrador inicial a partir de datos básicos (demo se verá en Bloque 5)
  2. **Resumen de expedientes** — darle el texto y pedirle síntesis por tema. **Atención: datos sensibles → ver Bloque 3.**
  3. **Mejora de redacción** — lenguaje más claro, más corto, más formal o más accesible.
  4. **Búsqueda y síntesis de jurisprudencia** — organizar criterios. **Atención: los fallos siempre se verifican en Saij/Infojus → ver Bloque 3.**
  5. **Traducción** de documentos en idiomas extranjeros.
  6. **Explicar tecnicismos** para partes no profesionales (sentencia en lenguaje claro → demo Bloque 5b).

- **Encuadre human-first** (2 min): "En todos estos casos la IA produce un borrador. **La firma, el criterio jurídico y la decisión son humanos.** Si una IA decide en el Poder Judicial, dejamos de tener Poder Judicial."

**Objetivo de bloque:** Que el participante reconozca las 5 herramientas más difundidas, identifique al menos 2 casos de uso concretos para su trabajo y entienda que el rol de la IA es asistir, no decidir.

**Estrategia pedagógica:** Slides de panorama, sin demos largas en este bloque — la primera interacción real con ChatGPT ocurre en el Bloque 2b; el prompting se trabaja en el Bloque 5; las funciones avanzadas en el Bloque 4b.

**Filminas estimadas:** 4–5 (tabla de herramientas, slide-resumen de casos de uso, slide de "humano primero" como cierre del bloque)

### Bloque 2b — Primera mirada a ChatGPT: la interfaz (7 min)

> **Propósito del bloque:** el participante llegará a casa y querrá intentar usar ChatGPT. Este bloque le da el mapa de la pantalla para que sepa adónde ir y qué tocar. Es la "visita guiada" antes de la práctica.

**Subtemas:**

- **Acceso** (1 min): abrir un navegador e ir a **chatgpt.com** — no se instala nada. Una cuenta gratuita alcanza para seguir toda la cursada. El docente lo muestra vía Google Meet (compartir pantalla desde la laptop).

- **Tour de la interfaz** (2 min): el docente señala en la pantalla de Google Meet los elementos clave:
  - **Barra lateral izquierda:** historial de conversaciones anteriores. Cada conversación es independiente.
  - **Área central:** donde se ve la conversación en curso.
  - **Caja de texto inferior:** ahí se escribe el *prompt*. Botón de enviar (o Enter).
  - **Selector de modelo** (arriba): GPT-4o, GPT-4o mini, etc. — por ahora dejar en el que viene por defecto.
  - **Botón "New chat":** abre una conversación nueva con la memoria en blanco.
  - **Ícono de perfil** (arriba a la derecha): acceso a Settings, donde están los controles de privacidad que veremos en el Bloque 4b.
  > **Mensaje del docente:** *"La interfaz cambia frecuentemente — OpenAI actualiza el diseño cada pocos meses. Los elementos clave siempre están, a veces en distinto lugar."*

- **Primer prompt en vivo** (3 min): el docente escribe en el chat una pregunta completamente neutra y relevante para el grupo:
  - Ejemplo: *"¿Qué es un oficio judicial y para qué sirve?"*
  - El grupo observa cómo la respuesta aparece **token por token** (el modelo escribe en tiempo real).
  - El docente señala: se puede hacer una **pregunta de seguimiento** sin repetir el contexto — el modelo recuerda lo dicho antes dentro del mismo chat.
  - El docente muestra cómo **copiar la respuesta**, cómo **regenerarla** si no convenció, y cómo abrir un **chat nuevo** para empezar de cero.

- **Regla de uso básica** (1 min): tres cosas para recordar antes de usar ChatGPT:
  1. No pegar información sensible de expedientes (lo desarrollamos en el Bloque 3).
  2. Lo que genera es un **borrador** — siempre revisar.
  3. Siempre revisar los **controles de privacidad** antes de usar con tareas del PJN (lo veremos en el Bloque 4b).

**Objetivo de bloque:** Que el participante reconozca la interfaz de ChatGPT, sepa dónde escribir y cómo leer la respuesta, y se lleve 3 reglas básicas de uso.

**Estrategia pedagógica:** Demo en la pantalla real de ChatGPT compartida vía Google Meet. El docente opera — los participantes observan. El impacto es ver la generación en tiempo real por primera vez (efecto «wow» controlado). El docente lo hace despacio y nombra cada elemento.

**Filminas estimadas:** 3–4 (slide de acceso con URL, slide del mapa de la interfaz con flechas anotadas, slide de las 3 reglas básicas)

### Bloque 3 — Riesgos del uso de IA — el humano decide primero (15 min)

> **Principio rector del bloque y del encuentro:** **El humano decide primero.** La IA propone; la persona valida, decide y firma. Este principio se enuncia al inicio del bloque y se repite explícitamente en cada riesgo.

**Subtemas:**
- **Riesgo 1 — Alucinaciones (5 min):** el modelo inventa información que suena creíble. Especialmente peligroso con fallos, artículos legales, números de expediente.

  **Caso argentino real — Cámara Civil de Rosario, agosto 2025 (juez Oscar Puccinelli):** un abogado presentó un escrito de apelación citando jurisprudencia que **no existía**. Ante la observación del tribunal, el letrado **reconoció** que había usado ChatGPT para buscar precedentes y que **no verificó** las citas. El juez interpretó que actuó de buena fe pero advirtió textualmente:
  > *"Es sumamente riesgoso y hasta temerario delegar la labor de búsqueda de jurisprudencia de soporte y luego volcarla sin cotejar la fuente."*

  Resultado: la apelación se rechazó, el abogado fue reprendido y se notificó al Tribunal de Ética. **Casos similares se replicaron** en Cipolletti (Río Negro, 2025, donde un tribunal dejó sin honorarios a dos abogados por la misma razón) y en otros fueros del país — la justicia argentina ya registra múltiples episodios documentados.

  → **Regla humana primero:** ningún dato que entregue la IA —especialmente jurisprudencia, artículos o números de expediente— se cita sin verificar en la fuente oficial (SAIJ, InfoJus, sitio del tribunal). El precio de saltarse este paso, en Argentina, ya tiene jurisprudencia propia.

- **Riesgo 2 — Confidencialidad y datos sensibles (3 min):** cuando se pega texto en ChatGPT con la configuración por defecto de una cuenta personal, esa información **puede ser usada para reentrenar al modelo**. **Implicancia en PJN:** datos de partes, testigos, menores, secreto de sumario, datos médicos. **Regla humana primero:** la decisión de qué sale del sistema la toma siempre la persona — nunca por reflejo, nunca por comodidad. Más adelante en la clase: el Bloque 4b muestra cómo desactivar el entrenamiento sobre los propios datos; el Bloque 5b explica el concepto de anonimización y cuándo aplicarla antes de usar IA con textos sensibles.
- **Riesgo 3 — Sesgos (2 min):** los modelos aprenden de textos existentes y pueden reproducir sesgos de género, etnia o clase social en redacción de resoluciones, descripciones de personas o evaluaciones. **Regla humana primero:** la persona revisa el lenguaje del borrador antes de firmar — no se acepta texto generado sin lectura crítica.
- **Riesgo 4 — Confianza excesiva / dependencia (2 min):** "si lo dijo la IA, debe ser verdad". Con el tiempo se pierde el reflejo de verificar. El caso de Rosario es ilustrativo: el abogado actuó con la confianza de que el resultado de ChatGPT era jurisprudencia real. **Regla humana primero:** mantener el hábito de leer críticamente lo que escribe la IA, igual que se leería un borrador de un practicante nuevo.
- **Riesgo 5 — Trazabilidad y responsabilidad (2 min):** si una IA "sugirió" un texto que se firmó, la responsabilidad sigue siendo del firmante. No hay "culpa de la IA" — los abogados sancionados en Rosario y Río Negro no pudieron alegar la culpa del modelo. **Regla humana primero:** la firma humana implica que el firmante asume todo el contenido como propio.
- **Síntesis del bloque** (1 min): el docente proyecta vía Google Meet el principio rector y lo lee en voz alta:

  > **"La IA propone borradores. El humano decide, valida y firma. Si quitamos al humano del medio, perdemos el control de la justicia — y, como mostró la Cámara de Rosario, terminamos pagando el costo profesional."**

**Objetivo de bloque:** Que el participante sepa _cuándo NO usar IA_ y _qué nunca delegar a la IA_ antes de aprender a usarla. Que internalice el principio "humano primero" como filtro automático de cualquier interacción futura con la herramienta, anclado en un caso de la justicia argentina que el participante puede contar en su oficina.

**Estrategia pedagógica:** 1 caso argentino contundente y reciente (Rosario 2025, con cita textual del juez) + repetición explícita del principio "humano primero" al cerrar cada riesgo. La cita textual del juez Puccinelli debe ir en una slide y leerse en voz alta — es el momento de mayor impacto del bloque.

**Filminas estimadas:** 7–8 (1 slide por riesgo + slide del caso Rosario con cita textual + slide complementaria mencionando casos similares + síntesis del principio rector)

### Bloque 4 — Ventana de contexto (6 min)
**Subtemas:**
- **Qué es la ventana de contexto** (2 min): "la memoria de trabajo de la IA durante una conversación". Metáfora del **pizarrón que se borra entre clases**: durante una conversación, el modelo ve todo lo escrito; cuando cerrás el chat, ese pizarrón se borra y el modelo no recuerda nada de la próxima vez.
- **Por qué importa en el PJN** (2 min): si el docente arranca una conversación nueva y pega solamente "redactá un oficio", la IA no sabe nada del caso. **Hay que darle el contexto cada vez**: tipo de causa, partes, datos relevantes. Sin contexto, el resultado es genérico o inventado.
- **Límite práctico** (1 min): los modelos actuales aceptan documentos largos (varias decenas de páginas), pero **al final de textos muy largos suelen "olvidar" lo del principio**. Práctica recomendada: trozos manejables, pedidos específicos.
- **Puente al Bloque 5** (1 min): "Si el contexto es clave — entonces el prompt tiene que tener todo el contexto necesario. Eso lo vemos ahora."

**Objetivo de bloque:** Que el participante sepa que la IA no recuerda entre sesiones y que el contexto debe proveerse explícitamente en cada conversación.

**Estrategia pedagógica:** Exposición directa con la metáfora del pizarrón. Sin demo técnica — el bloque sirve de puente conceptual al Bloque 5.

**Filminas estimadas:** 2–3 (metáfora del pizarrón, ejemplo con/sin contexto, regla práctica)

### Bloque 5 — Introducción al prompting (22 min)

> **Recordatorio human-first al iniciar el bloque:** todo lo que sigue produce **borradores**. La revisión, decisión y firma siguen siendo humanas.

> **Nota de continuidad:** este bloque usa ChatGPT tal como quedó abierto en el Bloque 2b. No se necesita ninguna herramienta adicional.

**Subtemas:**

- **Por qué la forma de pedir afecta el resultado** (1 min — concepto disparador): el modelo no "sabe" qué tan específico ser — responde con la granularidad que le dás. Una orden vaga produce una respuesta genérica; una instrucción precisa con contexto y restricciones produce un borrador útil. Esta diferencia se llama *prompt engineering* y es la habilidad clave para usar bien cualquier LLM.

- **Estructura básica del prompt: Rol + Tarea + Contexto + Restricciones + Plantilla de salida** (4 min):
  - **Rol:** "Sos un redactor judicial del PJN" — le dice al modelo desde qué perspectiva actuar.
  - **Tarea:** qué acción concreta se pide ("reescribí", "resumí", "listá", "respondé a").
  - **Contexto:** la información de fondo que el modelo necesita para producir algo útil ("se trata de un oficio de citación para un expediente de familia…").
  - **Restricciones:** qué no hacer o cómo hacerlo ("sin latinismos", "máximo 3 párrafos", "no uses 'estimado'").
  - **Plantilla de salida:** la estructura esperada del resultado ("la salida debe tener: encabezado, cuerpo, cierre formal con fórmula PJN").
  - **Visualización en pantalla:** la filmina con la plantilla `[Rol] + [Tarea] + [Contexto] + [Restricciones] + [Plantilla de salida]` queda visible durante todas las demos.

- **Demo 1 — prompt vago vs. prompt estructurado** (5 min):
  - El docente escribe primero el prompt vago: *"Redactá un oficio"* → ChatGPT responde con algo genérico, incompleto, que necesita mucha corrección.
  - Luego escribe el prompt estructurado con todos los componentes: *"Sos asistente redactor del PJN. Redactá un oficio de citación a testimonio para el juzgado de familia N.º 3 de Ushuaia. El convocado es [NOMBRE], la causa es [NÚMERO], la fecha de audiencia es [FECHA] a las [HORA]. Usá lenguaje formal, sin tuteo, con la fórmula de cierre: 'Sin otro particular, saludo a Ud. atte.' No uses latinismos."* → Respuesta útil, directamente aprovechable.
  - **Observación:** la diferencia no está en la IA — está en la instrucción. El modelo siempre hizo lo que pudo con lo que le diste.

- **Demo 2 — la restricción de confidencialidad** (5 min):
  - El docente agrega al prompt anterior una restricción explícita: *"No hagas referencia a ningún dato del expediente en el asunto ni en el cuerpo del correo — sólo en el adjunto."*
  - Resultado: la respuesta respeta exactamente esa restricción.
  - **Punto pedagógico:** las restricciones son instrucciones preventivas — son la forma en que el operador judicial controla el comportamiento de la IA antes de que genere la respuesta. No hace falta "confiar" en la IA; hace falta darle las reglas correctas desde el inicio.

- **Construcción colectiva** (5 min): el docente propone al grupo construir juntos un prompt para una tarea cotidiana que alguien del grupo mencione — oficio, informe, correo formal, notificación. El docente escribe en la pantalla de Google Meet lo que el grupo propone, organizado en los 5 componentes. Opcional: se lanza el prompt en ChatGPT y se lee el resultado en voz alta.
  - **Objetivo:** que los participantes sientan que pueden construir un prompt — no es magia, es estructura.

**Objetivo de bloque:** Que el participante comprenda que la calidad de la salida de la IA depende de la calidad de la instrucción, domine la estructura Rol + Tarea + Contexto + Restricciones + Plantilla, y haya visto en pantalla la diferencia entre un prompt vago y uno estructurado en un contexto judicial real.

**Estrategia pedagógica:** Dos demos cortas vía Google Meet + construcción colectiva con el grupo. No se distribuyen herramientas — Google Meet (compartir pantalla) solamente. La filmina con la plantilla se mantiene visible durante todo el bloque.

**Filminas estimadas:** 7–8 (concepto disparador, plantilla Rol+Tarea+Contexto+Restricciones+Plantilla, Demo 1 antes/después, Demo 2 restricción, slide construcción colectiva)

### Bloque 4b — Configuraciones de ChatGPT: GPTs, modo agente, búsqueda profunda y privacidad (15 min)

> **Nota de scope:** este bloque presenta funciones que ChatGPT ya ofrece hoy en su interfaz web y que cambian sustancialmente la experiencia del usuario administrativo. **No** se enseña a configurarlas en profundidad — se muestran para que el participante sepa que existen, entienda para qué sirve cada una y — críticamente — sepa que existen controles de privacidad y cómo encontrarlos.

**Subtemas:**

- **Cómo cambió ChatGPT en los últimos meses** (1 min): hasta hace poco era "un chat". Hoy es una plataforma con varios modos (chat normal, GPTs personalizados, modo agente, búsqueda web, búsqueda profunda) y con **controles de privacidad granulares** que conviene revisar antes de usarla con tareas del PJN.

- **Función 1 — GPTs personalizados (templates / asistentes propios)** (3 min):
  - **Qué es:** un "ChatGPT a medida" que el usuario configura una vez con instrucciones fijas (rol, tono, reglas, plantilla de salida) y queda guardado para reusar.
  - **Por qué importa en el PJN:** en lugar de escribir el mismo prompt largo cada vez ("sos asistente del PJN, respondé con esta plantilla…"), se configura una sola vez un GPT llamado "Redactor de Oficios PJN" y a partir de ahí alcanza con dar los datos del caso.
  - **Dónde se configura:** menú "Explorar GPTs" → "Crear un GPT" en chatgpt.com (requiere cuenta Plus). El docente muestra brevemente la pantalla de configuración y los campos "Nombre", "Instrucciones", "Conocimiento" (carga de archivos de referencia).
  - **Demo rápida (vía Google Meet):** el docente abre un GPT que tenía preconfigurado para esta clase — escribe solo "oficio a tal destinatario por tal motivo" y la IA responde directamente con la plantilla completa.
  - **Regla humano primero:** el GPT es un atajo — el contenido sigue siendo revisado y firmado por la persona.

- **Función 2 — Modo agente** (3 min):
  - **Qué es:** un modo en el que ChatGPT no sólo responde texto, sino que **ejecuta pasos por su cuenta**: abre páginas web, llena formularios, descarga archivos, encadena varias acciones para cumplir un objetivo.
  - **Ejemplo apto para PJN:** "buscame los últimos 5 fallos sobre tenencia compartida del fuero de familia y armame una planilla con tema, fecha, tribunal y link a la fuente". El agente abre las páginas, extrae los datos y devuelve la tabla.
  - **Por qué importa:** ahorra clics y copy-paste para tareas repetitivas de búsqueda y consolidación.
  - **⚠️ Advertencias críticas (regla humano primero amplificada):**
    - El agente puede equivocarse en pasos intermedios sin avisar — hay que revisar el resultado contra las fuentes.
    - **Nunca dejarlo operar sobre sistemas internos del PJN ni con credenciales institucionales**: si una IA decide y actúa en un sistema judicial, perdemos trazabilidad de quien tomó la decisión.
    - Función recomendada hoy sólo para tareas exploratorias con datos públicos.
  - **Demo vía Google Meet (si el tiempo y la conexión lo permiten):** el docente lanza una búsqueda agente sencilla en vivo y comenta lo que va haciendo el modelo paso a paso.

- **Función 3 — Búsqueda profunda (Deep Research)** (3 min):
  - **Qué es:** un modo en el que ChatGPT toma más tiempo (varios minutos) para investigar un tema consultando múltiples fuentes en internet y produce un **informe extenso con citas verificables**.
  - **Diferencia con la búsqueda normal:** la búsqueda normal responde en segundos con una respuesta corta y a veces sin citas. La búsqueda profunda produce un documento estructurado de varias páginas con referencias.
  - **Ejemplo apto para PJN:** "hace una investigación profunda sobre la evolución de la doctrina de la Corte Suprema argentina sobre prisión preventiva en los últimos 5 años".
  - **Ventaja:** ahorra horas de búsqueda manual para investigaciones doctrinarias o de políticas públicas.
  - **Limitación crítica (humano primero):** la búsqueda profunda **también puede equivocarse o citar fuentes secundarias mal interpretadas**. Sigue siendo un borrador. Las citas se verifican una por una antes de usar el informe en una actuación — recordar el caso de Rosario.

- **Función 4 — Controles de privacidad: que ChatGPT NO entrene con tus datos** (5 min) — **bloque crítico para uso en PJN, conectado con el Riesgo 2 del Bloque 3**:

  - **El problema en una frase:** en una cuenta personal con la configuración de fábrica, **todo lo que escribas en ChatGPT puede ser usado por OpenAI para entrenar futuros modelos**. Para un usuario común es un problema menor; para alguien que pega texto de un expediente, es un problema grave.

  - **Control 1 — Desactivar el entrenamiento sobre los propios chats:** **demo paso a paso vía Google Meet (compartir pantalla)**:
    - En la interfaz web: icóno de perfil (arriba a la derecha) → **Settings** → **Data Controls** → desactivar el toggle **"Improve the model for everyone"** ("Mejorar el modelo para todos").
    - El docente comparte vía Google Meet la pantalla real con el switch antes y después.
    - Efecto: las conversaciones siguen guardándose en el propio historial (para que el usuario pueda consultarlas), **pero OpenAI ya no las usa para entrenar**.
    - **Importante:** este control existe en la versión gratuita y en la versión Plus. Hay que activarlo explícitamente — no viene así por defecto.

  - **Control 2 — Chat temporal ("modo incógnito" de ChatGPT):** para conversaciones puntuales que no deben quedar en el historial:
    - Botón al iniciar un chat nuevo → **Chat temporal** (o icóno de modo temporal en la cabecera).
    - Efecto: ese chat **no se guarda en el historial**, **no se usa para entrenar** y **no genera memoria persistente**. Se elimina automáticamente en 30 días (sólo se conserva por razones de abuso/seguridad).
    - Caso de uso PJN: cualquier consulta donde se experimente con texto sensible y no convenga dejar rastro en el historial personal.

  - **Control 3 — Memoria entre chats:** ChatGPT puede "recordar" cosas que dijiste en chats anteriores para personalizar las respuestas (preferencias, contexto recurrente):
    - Settings → **Personalization** → **Memory** → activar/desactivar / borrar memorias específicas.
    - **Recomendación para uso PJN:** desactivar la memoria o revisarla periódicamente. No queremos que el modelo conserve fragmentos de casos previos entre sesiones.

  - **Control 4 — Cuentas Business / Enterprise / Edu:** mensaje importante para el área institucional:
    - **Por defecto, las cuentas Business, Team, Enterprise y Edu de ChatGPT NO usan los datos del usuario para entrenar al modelo.** Es decir: el contrato comercial activa esa protección automáticamente.
    - **Implicancia institucional:** si el PJN decide alguna vez contratar ChatGPT a nivel institucional, hereda esta protección. En cambio, una cuenta personal de un agente requiere la configuración manual descrita arriba.

  - **Mensaje de cierre del bloque de privacidad:** *"La privacidad en ChatGPT no es automática en cuentas personales — hay que activarla. Y aun activándola, el principio sigue: dato sensible real, mejor no se pega; se anonimiza primero (lo vemos en el Bloque 5b)."*

- **Cuándo usar cada modo** (síntesis, 1 min) — tabla en pantalla:

| Tarea | Modo recomendado |
|---|---|
| Redactar un texto recurrente con formato fijo (oficios, cédulas) | **GPT personalizado** |
| Recolectar datos públicos de varias páginas en una tabla | **Modo agente** (con verificación) |
| Producir un informe doctrinario o de panorama extenso | **Búsqueda profunda** |
| Consulta puntual con texto sensible que no debe quedar en historial | **Chat temporal** |
| Pregunta rápida, ajuste de redacción, traducción | Chat normal (con "Improve the model" desactivado) |

**Objetivo de bloque:** Que el participante distinga las configuraciones de ChatGPT — GPTs, modo agente, búsqueda profunda — reconozca para qué sirve cada una, **sepa que existen controles de privacidad y cómo encontrarlos** y entienda que ninguna función elimina la necesidad de revisión humana.

**Estrategia pedagógica:** Slides + 2–3 demos breves vía Google Meet (compartir pantalla). La demo de privacidad (desactivar entrenamiento) es **obligatoria y se muestra en la pantalla real de ChatGPT compartida vía Google Meet** — los participantes deben ver el menú concreto. El docente lleva su cuenta ya logueada para esto.

**Filminas estimadas:** 8–9 (intro, GPT personalizado, modo agente, búsqueda profunda, 3–4 slides de privacidad con capturas reales del menú, tabla "cuándo usar cada modo")

### Bloque 5b — Demo: sentencia en lenguaje claro y anonimización de datos (13 min)

> **Nota de scope:** Este bloque muestra el flujo de usar IA para reescribir texto judicial en lenguaje accesible para las partes, e introduce el concepto de anonimización de datos como práctica de resguardo ante información sensible. La demo corre completamente en el navegador — sin herramientas externas.

**Subtemas:**
- **El problema del lenguaje judicial** (1 min): las sentencias están escritas para abogados, pero las partes tienen derecho a entender qué se decidió sobre su caso. El lenguaje claro es una política pública adoptada en varios tribunales argentinos.

- **Demo en vivo — sentencia ficticia a lenguaje claro** (5 min):
  1. El docente tiene preparado un fragmento de resolución judicial **ficticia** (personajes y hechos inventados — nunca usar causas reales ni siquiera públicas).
  2. Pega el texto en ChatGPT con un prompt reutilizable: *"Reescribí este fragmento de resolución judicial en lenguaje claro, usando oraciones cortas, voz activa, sin latinismos y sin perder ningún dato sustancial. Conservá la estructura: encabezado, hechos, decisión, fundamento."*
  3. La IA devuelve la versión en lenguaje claro en segundos — el docente la lee en voz alta y compara con el original.
  - **Observación pedagógica:** el docente señala qué cosas convendría revisar (¿perdió algún matiz? ¿cambió el sentido de alguna cláusula?). Regla humano-primero en acción.

- **¿Y si el texto tiene datos sensibles? — Concepto de anonimización** (5 min):
  - **Qué es anonimizar:** antes de pegar texto con datos reales (nombres de partes, domicilios, datos de menores, condición médica, número de DNI, identidad de testigo protegido) en cualquier herramienta de IA, se **reemplazan esos datos con etiquetas genéricas**: `PERSONA_1`, `ORG_1`, `DIRECCIÓN_1`, etc.
  - **Ejemplo proyectado vía Google Meet:**
    - Texto original: *"La parte actora, María González Díaz, domiciliada en Av. Mitre 1234 de Rosario..."*
    - Texto anonimizado: *"La parte actora, PERSONA_1, domiciliada en DIRECCIÓN_1..."*
    - El prompt se arma con el texto anonimizado → la IA trabaja solo con etiquetas → la persona que recibe el resultado sustituye manualmente las etiquetas por los datos reales antes de usar el documento.
  - **Por qué importa en el PJN — casos que lo requieren:**
    - Expedientes con datos de menores → obligación legal de reserva.
    - Víctimas o testigos con protección de identidad → dato que no debe circular.
    - Datos médicos y psicológicos de las partes → sensibilidad especial.
    - Secreto de sumario → el contenido no debe salir del sistema judicial.
  - **La anonimización como segunda capa de protección:** incluso con los controles de privacidad activados en ChatGPT (Bloque 4b), la anonimización previa añade una capa adicional para los expedientes de máxima sensibilidad. No son excluyentes — se complementan.
  - **Regla práctica:** si el texto tiene datos que no deberían salir del sistema, anonimizarlos antes de pegar en ChatGPT — aunque sea manualmente con búsqueda y reemplazo en un editor de texto.
  > **Nota de producción:** encuentros posteriores mostrarán flujos donde la anonimización y la restitución de datos se hacen de forma automática. Por ahora lo más importante es que el participante entienda el concepto y la razón de hacerlo.

- **Reflexión final y principio human-first** (2 min): la IA acelera la reescritura — el magistrado o magistrada sigue decidiendo el contenido jurídico. La anonimización garantiza que el proceso no comprometa datos sensibles de las partes. Ambas cosas juntas hacen que el uso de IA en este contexto sea **responsable**.

**Objetivo de bloque:** Que el participante entienda el flujo básico de usar IA para reescribir texto judicial en lenguaje accesible, e internalice el concepto de anonimización de datos como práctica preventiva antes de usar IA con información sensible.

**Estrategia pedagógica:** Demo vía Google Meet (compartir pantalla) + explicación conceptual con ejemplo proyectado. No se requiere ninguna herramienta adicional — todo corre en ChatGPT desde el navegador. El ejemplo de anonimización se muestra en la pantalla de Google Meet con texto real en el editor.

**Filminas estimadas:** 4–5 (el problema, demo antes/después de lenguaje claro, slide de anonimización con ejemplo visual ORIGINAL → ANONIMIZADO, slide "cuándo anonimizar en el PJN", reflexión final)

### Bloque 6 — Cierre (12 min)

**Los 7 conceptos clave del día** (slide de síntesis, nombrarlos explícitamente):
1. Los **LLMs (ChatGPT, Claude, Gemini)** son una rama del Deep Learning dentro del universo más amplio de la IA.
2. La IA genera texto **probable** — no garantiza verdad. **El caso Rosario 2025** prueba que en Argentina esto ya tiene consecuencias profesionales.
3. **El humano decide primero**: la IA propone, la persona valida, decide y firma.
4. **Nunca pegar datos reales** en un chat público; cuando sea imprescindible, anonimizar antes.
5. **Privacidad no es automática en cuentas personales:** hay que entrar a Settings → Data Controls y desactivar "Improve the model for everyone". Para conversaciones sensibles puntuales, usar chat temporal.
6. El **contexto del prompt** determina la calidad de la respuesta.
7. ChatGPT hoy tiene **modos especializados** — GPTs personalizados, modo agente, búsqueda profunda — cada uno con su uso.

**Dinámica de cierre:**
- El docente proyecta vía Google Meet los 7 conceptos y pide al grupo que mencione cuál le parece más útil para su trabajo diario — mano alzada o comentario libre (2 min)
- Mensaje central en voz alta: **"La IA no garantiza verdad: genera respuestas plausibles. El humano decide primero."** (1 min)
- Ronda de preguntas abiertas — el docente responde hasta 3 preguntas breves; las que requieran desarrollo se difieren al Encuentro 2 (4 min)
- Anuncio del Encuentro 2 y entrega de materiales ("el link a los prompts usados queda en el grupo institucional") (2 min)

**Filminas:** 2 (síntesis de los 7 conceptos + mensaje clave final)

---

## Filminas estimadas: 43–53 filminas

> Distribución orientativa (ajustable por Roberto en la redacción):
> - 1 portada
> - 1 agenda
> - 5–6 bloque 1 (diagrama de círculos concéntricos IA→ML→DL→LLM, predictor de palabras, tabla buscador/BD/LLM, glosario)
> - 4–5 bloque 2 (tabla de 5 herramientas — sin Perplexity —, casos de uso, "humano primero")
> - 3–4 bloque 2b (acceso a chatgpt.com, mapa de la interfaz con anotaciones, primer prompt en vivo, 3 reglas básicas)
> - 7–8 bloque 3 (1 por riesgo + slide con cita textual del juez Puccinelli + slide de casos similares en Argentina + principio rector)
> - 2–3 bloque 4 (ventana de contexto)
> - 7–8 bloque 5 (plantilla de prompt + demos de prompting — sin MCP)
> - 8–9 bloque 4b (intro, GPTs, modo agente, búsqueda profunda, 3–4 slides de privacidad con capturas reales del menú Data Controls, tabla "cuándo usar cada modo")
> - 4–5 bloque 5b (lenguaje claro + concepto de anonimización con ejemplo visual ORIGINAL → ANONIMIZADO)
> - 2 cierre (síntesis de 7 conceptos + mensaje clave)

> **Nota de producción:** La filmina con la plantilla `[Rol] + [Tarea] + [Contexto] + [Restricciones] + [Plantilla de salida]` debe permanecer visible durante todas las demos del Bloque 5. La frase del principio rector "El humano decide primero" debe aparecer como banda inferior recurrente en todos los bloques prácticos (4b, 5, 5b) — puede implementarse como elemento fijo de footer.

---

## Concepto no negociable del encuentro

> **"La IA no garantiza verdad: genera respuestas plausibles."**
> Debe quedar grabado en el participante antes de que use cualquier herramienta de IA en su trabajo.

---

## Principio rector — El humano decide primero

> **La IA propone borradores. El humano valida, decide y firma.**

Este principio se enuncia explícitamente en cuatro momentos de la clase:

1. Bloque 2 — al cerrar el panorama de herramientas ("si la IA decide, dejamos de tener Poder Judicial").
2. Bloque 2b — al enunciar las 3 reglas básicas de uso de ChatGPT.
3. Bloque 3 — al final de cada uno de los 5 riesgos, como cierre operativo.
4. Bloque 4b — al presentar el modo agente, donde el riesgo de delegación es mayor.
5. Bloque 5 y 5b — como recordatorio al iniciar el bloque práctico.

Es el filtro mental que el participante se lleva a su escritorio. Si solo recuerda una cosa del encuentro, debe ser ésta.

---

## Restricciones de scope

Los siguientes temas se **mencionan** en este encuentro pero NO se enseñan en profundidad (se difieren a encuentros posteriores):
- **NotebookLM y herramientas específicas de documentos** → trabajo a fondo en Encuentro 2 (sólo mención en el panorama de herramientas del Bloque 2).
- **Búsqueda estructurada de jurisprudencia con verificación** → Encuentro 2.
- **Configuración paso a paso de GPTs personalizados** → Bloque 4b sólo muestra qué es y para qué sirve; la configuración hands-on queda para encuentros posteriores.

Los siguientes temas están **fuera de scope completo** de este encuentro:
- Futuro de la IA en el derecho → Encuentro 3.
- Algoritmos o código fuente.
- Historia de la IA (más allá de la mínima ubicación histórica de los LLMs en el Bloque 1).
- Comparativas técnicas de modelos (parámetros, benchmarks).
- Aspectos regulatorios (ley de protección de datos, Pacto Digital) más allá de la regla práctica de confidencialidad.

---

## Recursos y materiales necesarios

### En la sala
| Recurso | Requerido | Notas |
|---------|-----------|-------|
| Proyector / pantalla | Obligatorio | Toda la clase se proyecta vía Google Meet — sin proyección no se puede dictar |
| Laptop del docente | Obligatorio | Con acceso a ChatGPT, Google Meet y sesión iniciada |
| Conexión a internet | Obligatorio | Necesario para ChatGPT y Google Meet |
| Micrófono | Recomendado en salas >15 personas | Voz clara es clave para las demos |

### Software y cuentas
| Herramienta | Estado requerido | Verificación pre-clase |
|-------------|----------------|------------------------|
| ChatGPT (cuenta del docente) | Activa y con sesión iniciada | Abrir y hacer un prompt de prueba |
| Google Meet | Sesión abierta y compartir pantalla activo | Verificar que la pantalla se ve nítida en el proyector de la sala |
| Navegador web | Actualizado | Chrome, Firefox o Edge — verificar que chatgpt.com carga sin bloqueo de red |
| `guia-lenguaje-claro.md` | Presente en carpeta del tema | Referencia conceptual para el Bloque 5b |
| Texto ficticio de sentencia (preparado por el docente) | Listo para copiar | Para la demo del Bloque 5b — datos completamente inventados |

---

## Setup técnico pre-clase

> Ejecutar **al menos 30 minutos antes** del inicio. No hacerlo en el momento — las demos en vivo requieren que todo esté probado.

1. **Abrir ChatGPT** y dejar la sesión iniciada — hacer al menos un prompt para confirmar que no hay bloqueo de red en la sala
2. **Preparar el texto ficticio de sentencia** para la demo del Bloque 5b: resolución o fragmento de sentencia con datos de personajes completamente inventados — coherente y realista pero sin ningún dato real (no usar causas reales aunque sean públicas)
3. **Preparar el ejemplo de anonimización** para la demo de Bloque 5b: tener el mismo texto ficticio en dos versiones — original y con los datos reemplazados por etiquetas (`PERSONA_1`, `DIRECCIÓN_1`, etc.) — listos para proyectar vía Google Meet
4. **Abrir Google Meet** y activar "Compartir pantalla" — confirmar que la proyección es nítida desde el fondo de la sala y que el audio del micrófono llega bien
5. **Proyectar la slide de portada vía Google Meet** antes de que entre el grupo — confirmar que la escala de fuente es legible desde el fondo de la sala

---

## Contingencias técnicas

| Escenario | Plan B |
|-----------|--------|
| **ChatGPT caído o sin internet** | Mostrar capturas de pantalla pre-grabadas de los resultados esperados. Continuar la clase como demo conceptual — el docente explica el resultado en lugar de generarlo. |
| **Sin proyección / Google Meet caido** | La clase no puede dictarse en formato demo. Opción: redirigir a discusión grupal con los prompts leídos en voz alta y resultados descriptos por el docente. Notificar a coordinación. |
| **El grupo usa sus propios dispositivos** | No es el formato esperado, pero si surgen espontáneamente, aprovechar para comparar resultados. Recordar la regla de privacidad antes de que peguen cualquier contenido. |
| **Preguntas que se extienden demasiado** | El docente usa la frase: "Eso lo desarrollamos en el Encuentro 2 — lo anoto para no perderlo." Escribe la pregunta en el chat de Meet y continúa. |

---

## Instrucciones de producción para Roberto (class-writer)

> **Leer antes de generar `minuta.md` y `filminas.md`**

### Prompts de demo para el docente

> **Nota:** No hay herramientas externas en este encuentro. Todas las demos corren enteramente en ChatGPT desde el navegador.

**Demo 1 — Prompt vago (Bloque 5, para mostrar el contraste):**
```
Redactá un oficio.
```

**Demo 1 — Prompt estructurado (Bloque 5):**
```
Sos asistente redactor del PJN. Redactá un oficio de citación a testimonio para el juzgado de familia N.º 3 de Ushuaia. El convocado es [NOMBRE], la causa es [NÚMERO], la fecha de audiencia es [FECHA] a las [HORA]. Usá lenguaje formal, sin tuteo, con la fórmula de cierre: 'Sin otro particular, saludo a Ud. atte.' No uses latinismos.
```

**Demo 2 — Restricción de confidencialidad (Bloque 5):**
(mismo prompt anterior, agregar al final:)
```
No hagas referencia a ningún dato del expediente en el asunto ni en el cuerpo del correo — sólo en el adjunto.
```

**Demo Bloque 5b — Sentencia en lenguaje claro:**
```
Reescribí este fragmento de resolución judicial en lenguaje claro, usando oraciones cortas, voz activa, sin latinismos y sin perder ningún dato sustancial. Conservá la estructura: encabezado, hechos, decisión, fundamento.
[pegar fragmento de sentencia ficticia]
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
5. **Duración:** No usar los 120 min como límite estricto — el docente avanza más rápido. Generar el contenido completo sin recortar bloques para ajustar al tiempo estimado.

---

## Criterios de aprobación del diseño

- [ ] Duración total ≤ 120 minutos con los bloques propuestos
- [ ] Los 5 tópicos del plan-mínimo (Día 1) están cubiertos
- [ ] Los LLMs están ubicados explícitamente dentro del mapa general de la IA (jerarquía IA→ML→DL→LLM en Bloque 1)
- [ ] El panorama de herramientas relevantes para PJN aparece nombrado (Bloque 2) — sin Perplexity, foco en las 5 más relevantes
- [ ] El principio "el humano decide primero" está enunciado en al menos 4 momentos de la clase
- [ ] **El bloque de riesgos incluye un caso argentino real y reciente** (Cámara Civil de Rosario 2025, juez Puccinelli) con cita textual proyectada
- [ ] Las funciones de ChatGPT (GPTs, agente, búsqueda profunda) están cubiertas (Bloque 4b)
- [ ] **Los controles de privacidad de ChatGPT están cubiertos en demo proyectada** sobre la pantalla real: cómo desactivar "Improve the model", chat temporal, memoria, comportamiento por defecto en planes Business/Enterprise (Bloque 4b)
- [ ] El diseño es ejecutable por un docente con perfil investigador
- [ ] El público objetivo (no técnico) puede seguir el hilo sin perderse — los tecnicismos están acompañados de analogías o glosario
- [ ] **La interfaz de ChatGPT se presenta explícitamente** en el Bloque 2b: el participante ve la pantalla real antes de la primera demo de prompting
- [ ] El bloque de prompting (Bloque 5) viene **antes** que las configuraciones avanzadas (Bloque 4b) — el participante practica primero con la interfaz básica
- [ ] El bloque de prompting es enteramente en vivo (demo proyectada por el docente — sin dispositivos individuales)
- [ ] **No hay demo MCP** en este encuentro — la integración avanzada (generación de .docx, anonimización automática) se deja para encuentros posteriores
- [ ] **No hay pausa formal:** la clase corre los 120 minutos sin descanso programado (puede haber micropausas espontáneas del docente si el grupo lo necesita)
