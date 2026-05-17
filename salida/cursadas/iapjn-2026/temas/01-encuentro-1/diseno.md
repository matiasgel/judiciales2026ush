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
3. Nombrar los principales riesgos del uso de IA en contextos legales (alucinaciones, confidencialidad, sesgos, dependencia) y aplicar el principio "el humano decide primero".
4. Describir qué es la ventana de contexto y cómo afecta la calidad de la respuesta.
5. Reconocer las configuraciones actuales de ChatGPT — GPTs personalizados, modo agente y búsqueda profunda — y entender para qué sirve cada una.
6. Formular un prompt básico con estructura: rol + tarea + contexto + restricciones + plantilla de salida.

---

## Indicadores de logro

> Señales observables durante la clase que confirman que los objetivos se están cumpliendo. Útiles para que el docente calibre el ritmo en tiempo real.

| Objetivo | Indicador observable |
|----------|---------------------|
| Entender qué es la IA y ubicar a los LLMs | El participante puede dibujar (o explicar) la jerarquía IA → Machine Learning → LLMs y nombrar al menos un ejemplo de cada nivel |
| Identificar casos de uso y herramientas en el PJN | Menciona al menos una herramienta (ChatGPT, Claude, Gemini, NotebookLM, Copilot) y un caso de uso propio de su área |
| Nombrar riesgos y aplicar "humano primero" | Puede decir "alucinación", "confidencialidad" y completar la frase "la IA propone, el humano _______" (decide / valida / firma) |
| Ventana de contexto | Explica por qué el modelo "se olvida" entre sesiones sin necesidad de repregunta |
| Configuraciones de ChatGPT | Diferencia oralmente las 3 funciones: un GPT personalizado, el modo agente, la búsqueda profunda — con un ejemplo de cuándo conviene cada una |
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

## Distribución de tiempo (120 min)

| Bloque | Nombre | Duración | Tipo |
|--------|--------|----------|------|
| 0 | Apertura y presentación del día | 5 min | Encuadre |
| 1 | ¿Qué es la IA? Dónde están los LLMs | 17 min | Conceptual |
| 2 | Herramientas de IA y usos en el Poder Judicial | 10 min | Aplicado |
| 3 | Riesgos del uso de IA — el humano decide primero | 13 min | Crítico / Preventivo |
| — | Pausa activa | 10 min | Descanso |
| 4 | Ventana de contexto | 6 min | Conceptual |
| 4b | Configuraciones actuales de ChatGPT: GPTs, modo agente, búsqueda profunda | 10 min | Demostrativo / Panorama |
| 5 | Introducción al prompting | 25 min | Práctico |
| 5b | Demo avanzada: sentencia en lenguaje claro → .docx | 15 min | Práctico / Demo |
| 6 | Cierre, preguntas y mensaje clave | 9 min | Síntesis |
| **Total** | | **120 min** | |

> **Perfil docente:** Ritmo de exposición ágil — los bloques teóricos están dimensionados para exposición fluida sin detenerse en detalles técnicos. El tiempo ganado en teoría se vuelca íntegro en el ejercicio práctico de prompting.

> **Regla de scope:** Cualquier contenido no listado en la tabla anterior está fuera de scope de este encuentro.

---

## Descripción por bloque

### Bloque 0 — Apertura (5 min)
- Presentación del docente y del programa del encuentro
- Pregunta inicial al público: "¿Alguien ya usó ChatGPT o una IA? ¿Para qué?"
- El docente registra mentalmente cuántos levantan la mano para calibrar el ritmo de los primeros bloques
- Objetivo: romper el hielo y activar conocimientos previos. Anticipa que la clase es **enteramente proyectada** — no se requiere computadora ni celular para seguirla

### Bloque 1 — ¿Qué es la IA? Dónde están los LLMs (17 min)

**Subtemas:**
- **Qué es la inteligencia artificial** (3 min): definición operativa sin tecnicismos — "programas que aprenden a hacer tareas que antes requerían inteligencia humana". Ejemplos cotidianos que la gente ya usa sin saberlo: filtro de spam del correo, recomendaciones de Netflix, autocomplete del teclado.
- **El mapa de la IA — dónde están los LLMs** (5 min): diagrama de círculos concéntricos que el docente explica de afuera hacia adentro:
  - **IA (Inteligencia Artificial)** — el universo entero: cualquier sistema que imita capacidades humanas (reconocer caras, traducir, decidir rutas).
  - **Machine Learning (Aprendizaje Automático)** — IA que aprende de ejemplos en vez de seguir reglas escritas. Ej: filtro de spam, sistemas de scoring crediticio.
  - **Deep Learning (Aprendizaje Profundo)** — ML con redes neuronales grandes. Ej: reconocimiento facial, traducción automática.
  - **LLMs (Modelos de Lenguaje Grandes)** — una rama del Deep Learning especializada en lenguaje. Ej: **ChatGPT, Claude, Gemini, Copilot**. Esto es lo que vamos a usar en la cursada.
  > **Frase clave del docente:** "Cuando alguien dice IA en una conversación hoy, en el 90% de los casos está hablando de un LLM. Pero IA es mucho más grande — los LLMs son una herramienta dentro de un universo más amplio."
- **Cómo funciona un LLM en una sola idea** (4 min): la metáfora del "predictor de palabras". Un LLM mira un texto y predice cuál es la palabra más probable que sigue, una y otra vez. Ejemplo en vivo: el docente escribe en el pizarrón "El acusado se presenta ante el..." y pregunta al grupo qué palabra va. El grupo dice "juez", "tribunal", "fiscal". Eso es exactamente lo que hace un LLM — con la diferencia de que vio millones de textos antes.
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

**Estrategia pedagógica:** Exposición con 1 diagrama visual (círculos concéntricos), 1 demo rápida de predicción de palabras en el pizarrón y 1 tabla comparativa. Sin profundizar en historia, arquitectura ni matemática.

**Filminas estimadas:** 5–6 (portada del bloque, diagrama de círculos concéntricos, predictor de palabras, tabla comparativa buscador/BD/LLM, glosario)

### Bloque 2 — Herramientas de IA y usos en el Poder Judicial (10 min)

**Subtemas:**
- **Panorama actual de herramientas de IA generativa** (3 min): el docente proyecta una slide con las herramientas más relevantes para trabajo administrativo y judicial, agrupadas por para qué sirven:

| Herramienta | Quién la hace | Para qué sirve principalmente | Disponible en navegador |
|---|---|---|---|
| **ChatGPT** | OpenAI | Conversación general, redacción, análisis de texto | Sí (chatgpt.com) |
| **Claude** | Anthropic | Conversación general, textos largos, raciocinio jurídico | Sí (claude.ai) |
| **Gemini** | Google | Conversación integrada con servicios Google | Sí (gemini.google.com) |
| **NotebookLM** | Google | "Cuaderno" donde se cargan documentos propios y la IA responde sólo en base a esos documentos | Sí (notebooklm.google.com) |
| **Copilot** | Microsoft | Integrado en Word, Outlook, Edge | En productos Microsoft 365 |
| **Perplexity** | Perplexity AI | Búsqueda con citas verificables tipo motor de búsqueda + LLM | Sí (perplexity.ai) |

  > **Aclaración del docente:** "En esta cursada vamos a usar ChatGPT como ejemplo principal porque es la más difundida, pero todo lo que aprendan se aplica casi igual al resto."

- **Casos de uso concretos en el PJN** (5 min): el docente repasa con 1 slide por caso y comenta cuándo lo usó él u otros docentes:
  1. **Redacción de oficios** — borrador inicial a partir de datos básicos (demo se verá en Bloque 5)
  2. **Resumen de expedientes** — darle el texto y pedirle síntesis por tema. **Atención: datos sensibles → ver Bloque 3.**
  3. **Mejora de redacción** — lenguaje más claro, más corto, más formal o más accesible.
  4. **Búsqueda y síntesis de jurisprudencia** — organizar criterios. **Atención: los fallos siempre se verifican en Saij/Infojus → ver Bloque 3.**
  5. **Traducción** de documentos en idiomas extranjeros.
  6. **Explicar tecnicismos** para partes no profesionales (sentencia en lenguaje claro → demo Bloque 5b).

- **Encuadre human-first** (2 min): "En todos estos casos la IA produce un borrador. **La firma, el criterio jurídico y la decisión son humanos.** Si una IA decide en el Poder Judicial, dejamos de tener Poder Judicial."

**Objetivo de bloque:** Que el participante reconozca las 5–6 herramientas más difundidas, identifique al menos 2 casos de uso concretos para su trabajo y entienda que el rol de la IA es asistir, no decidir.

**Estrategia pedagógica:** Slides de panorama, sin demos largas en este bloque — las herramientas se ven en acción en los Bloques 4b, 5 y 5b. El docente comenta cuál usa él y por qué.

**Filminas estimadas:** 4–5 (tabla de herramientas, slide-resumen de casos de uso, slide de "humano primero" como cierre del bloque)

### Bloque 3 — Riesgos del uso de IA — el humano decide primero (13 min)

> **Principio rector del bloque y del encuentro:** **El humano decide primero.** La IA propone; la persona valida, decide y firma. Este principio se enuncia al inicio del bloque y se repite explícitamente en cada riesgo.

**Subtemas:**
- **Riesgo 1 — Alucinaciones (3 min):** el modelo inventa información que suena creíble. Especialmente peligroso con fallos, artículos legales, números de expediente. **Caso real:** Mata vs Avianca (EE.UU., 2023) — un abogado presentó fallos generados por ChatGPT que **no existían**. El juez le aplicó sanción. → **Regla humana primero:** ningún dato que entregue la IA se cita sin verificar en la fuente oficial.
- **Riesgo 2 — Confidencialidad y datos sensibles (3 min):** cuando se pega texto en ChatGPT público, esa información puede ser usada para reentrenar al modelo. **Implicancia en PJN:** datos de partes, testigos, menores, secreto de sumario, datos médicos. **Regla humana primero:** la decisión de qué sale del sistema la toma siempre la persona — nunca por reflejo, nunca por comodidad. Anticipo del Bloque 5b: existen flujos donde el dato real **nunca sale** (anonimización local + IA).
- **Riesgo 3 — Sesgos (2 min):** los modelos aprenden de textos existentes y pueden reproducir sesgos de género, etnia o clase social en redacción de resoluciones, descripciones de personas o evaluaciones. **Regla humana primero:** la persona revisa el lenguaje del borrador antes de firmar — no se acepta texto generado sin lectura crítica.
- **Riesgo 4 — Confianza excesiva / dependencia (2 min):** "si lo dijo la IA, debe ser verdad". Con el tiempo se pierde el reflejo de verificar. **Regla humana primero:** mantener el hábito de leer críticamente lo que escribe la IA, igual que se leería un borrador de un practicante nuevo.
- **Riesgo 5 — Trazabilidad y responsabilidad (2 min):** si una IA "sugirió" un texto que se firmó, la responsabilidad sigue siendo del firmante. No hay "culpa de la IA". **Regla humana primero:** la firma humana implica que el firmante asume todo el contenido como propio.
- **Síntesis del bloque** (1 min): el docente proyecta el principio rector y lo lee en voz alta:

  > **"La IA propone borradores. El humano decide, valida y firma. Si quitamos al humano del medio, perdemos el control de la justicia."**

**Objetivo de bloque:** Que el participante sepa _cuándo NO usar IA_ y _qué nunca delegar a la IA_ antes de aprender a usarla. Que internalice el principio "humano primero" como filtro automático de cualquier interacción futura con la herramienta.

**Estrategia pedagógica:** 1 caso real contundente (Mata vs Avianca) + repetición explícita del principio "humano primero" al cerrar cada riesgo. La repetición no es retórica — es la herramienta pedagógica del bloque.

**Filminas estimadas:** 6–7 (1 slide por riesgo + caso real + síntesis del principio rector)

### Pausa activa (10 min)
- El docente anuncia el descanso y sugiere aprovechar para estirar, caminar o revisar el celular
- **Actividad opcional:** si el grupo está enganchado, dejar en la pantalla proyectada la slide de la regla de privacidad del Bloque 3 como recordatorio visual durante la pausa
- El docente verifica en la pausa que el MCP server sigue activo y que la demo del Bloque 5b está lista para ejecutar
- Al retomar: 1 slide de "¿Dónde estamos?" con la agenda marcando los bloques ya cubiertos y los que restan

**Filminas de la pausa:** 0 (la agenda sirve de puente al retomar)

### Bloque 4 — Ventana de contexto (6 min)
**Subtemas:**
- **Qué es la ventana de contexto** (2 min): "la memoria de trabajo de la IA durante una conversación". Metáfora del **pizarrón que se borra entre clases**: durante una conversación, el modelo ve todo lo escrito; cuando cerrás el chat, ese pizarrón se borra y el modelo no recuerda nada de la próxima vez.
- **Por qué importa en el PJN** (2 min): si el docente arranca una conversación nueva y pega solamente "redactá un oficio", la IA no sabe nada del caso. **Hay que darle el contexto cada vez**: tipo de causa, partes, datos relevantes. Sin contexto, el resultado es genérico o inventado.
- **Límite práctico** (1 min): los modelos actuales aceptan documentos largos (varias decenas de páginas), pero **al final de textos muy largos suelen "olvidar" lo del principio**. Práctica recomendada: trozos manejables, pedidos específicos.
- **Puente al Bloque 5** (1 min): "Si el contexto es clave — entonces el prompt tiene que tener todo el contexto necesario. Eso lo vemos ahora."

**Objetivo de bloque:** Que el participante sepa que la IA no recuerda entre sesiones y que el contexto debe proveerse explícitamente en cada conversación.

**Estrategia pedagógica:** Exposición directa con la metáfora del pizarrón. Sin demo técnica — el bloque sirve de puente conceptual al Bloque 5.

**Filminas estimadas:** 2–3 (metáfora del pizarrón, ejemplo con/sin contexto, regla práctica)

### Bloque 4b — Configuraciones actuales de ChatGPT: GPTs, modo agente, búsqueda profunda (10 min)

> **Nota de scope:** este bloque presenta funciones avanzadas que ChatGPT ya ofrece hoy en su interfaz web y que cambian sustancialmente la experiencia del usuario administrativo. **No** se enseña a configurarlas en profundidad — se muestran para que el participante sepa que existen y entienda para qué sirve cada una.

**Subtemas:**

- **Cómo cambió ChatGPT en los últimos meses** (1 min): hasta hace poco era "un chat". Hoy es una plataforma con varios modos: chat normal, GPTs personalizados, modo agente, búsqueda web, búsqueda profunda. Cada uno sirve para algo distinto.

- **Función 1 — GPTs personalizados (templates / asistentes propios)** (3 min):
  - **Qué es:** un "ChatGPT a medida" que el usuario configura una vez con instrucciones fijas (rol, tono, reglas, plantilla de salida) y queda guardado para reusar.
  - **Por qué importa en el PJN:** en lugar de escribir el mismo prompt largo cada vez ("sos asistente del PJN, respondé con esta plantilla…"), se configura una sola vez un GPT llamado "Redactor de Oficios PJN" y a partir de ahí alcanza con dar los datos del caso.
  - **Dónde se configura:** menú "Explorar GPTs" → "Crear un GPT" en chatgpt.com (requiere cuenta Plus). El docente muestra brevemente la pantalla de configuración y los campos "Nombre", "Instrucciones", "Conocimiento" (carga de archivos de referencia).
  - **Demo rápida (proyectada):** el docente abre un GPT que tenía preconfigurado para esta clase — escribe solo "oficio a tal destinatario por tal motivo" y la IA responde directamente con la plantilla completa.
  - **Regla humano primero:** el GPT es un atajo — el contenido sigue siendo revisado y firmado por la persona.

- **Función 2 — Modo agente** (3 min):
  - **Qué es:** un modo en el que ChatGPT no sólo responde texto, sino que **ejecuta pasos por su cuenta**: abre páginas web, llena formularios, descarga archivos, encadena varias acciones para cumplir un objetivo.
  - **Ejemplo apto para PJN:** "buscame los últimos 5 fallos sobre tenencia compartida del fuero de familia y armame una planilla con tema, fecha, tribunal y link a la fuente". El agente abre las páginas, extrae los datos y devuelve la tabla.
  - **Por qué importa:** ahorra clics y copy-paste para tareas repetitivas de búsqueda y consolidación.
  - **⚠️ Advertencias críticas (regla humano primero amplificada):**
    - El agente puede equivocarse en pasos intermedios sin avisar — hay que revisar el resultado contra las fuentes.
    - **Nunca dejarlo operar sobre sistemas internos del PJN ni con credenciales institucionales**: si una IA decide y actúa en un sistema judicial, perdemos trazabilidad de quien tomó la decisión.
    - Función recomendada hoy sólo para tareas exploratorias con datos públicos.
  - **Demo proyectada (si el tiempo y la conexión lo permiten):** el docente lanza una búsqueda agente sencilla en vivo y comenta lo que va haciendo el modelo paso a paso.

- **Función 3 — Búsqueda profunda (Deep Research)** (3 min):
  - **Qué es:** un modo en el que ChatGPT toma más tiempo (varios minutos) para investigar un tema consultando múltiples fuentes en internet y produce un **informe extenso con citas verificables**.
  - **Diferencia con la búsqueda normal:** la búsqueda normal responde en segundos con una respuesta corta y a veces sin citas. La búsqueda profunda produce un documento estructurado de varias páginas con referencias.
  - **Ejemplo apto para PJN:** "hace una investigación profunda sobre la evolución de la doctrina de la Corte Suprema argentina sobre prisión preventiva en los últimos 5 años".
  - **Ventaja:** ahorra horas de búsqueda manual para investigaciones doctrinarias o de políticas públicas.
  - **Limitación crítica (humano primero):** la búsqueda profunda **también puede equivocarse o citar fuentes secundarias mal interpretadas**. Sigue siendo un borrador. Las citas se verifican una por una antes de usar el informe en una actuación.

- **Cuándo usar cada modo** (síntesis, 0–1 min) — tabla en pantalla:

| Tarea | Modo recomendado |
|---|---|
| Redactar un texto recurrente con formato fijo (oficios, cédulas) | **GPT personalizado** |
| Recolectar datos públicos de varias páginas en una tabla | **Modo agente** (con verificación) |
| Producir un informe doctrinario o de panorama extenso | **Búsqueda profunda** |
| Pregunta rápida, ajuste de redacción, traducción | Chat normal |

**Objetivo de bloque:** Que el participante distinga 3 configuraciones avanzadas de ChatGPT — GPTs, modo agente y búsqueda profunda — reconozca para qué sirve cada una y entienda que ninguna elimina la necesidad de revisión humana.

**Estrategia pedagógica:** Slides + 1–2 demos breves proyectadas. El docente NO enseña a configurar paso a paso — muestra la pantalla y nombra los campos clave para que el participante reconozca el menú cuando vuelva a su escritorio. La cursada profundiza estas funciones en encuentros posteriores.

**Filminas estimadas:** 5–6 (intro "cómo cambió ChatGPT", 1 slide por función con capturas, tabla "cuándo usar cada una")

### Bloque 5 — Introducción al prompting (25 min)

> **Recordatorio human-first al iniciar el bloque:** todo lo que sigue produce **borradores**. La revisión, decisión y firma siguen siendo humanas.

**Subtemas:**
- **Por qué la forma de pedir afecta el resultado** (1 min — concepto disparador)
- **Estructura básica del prompt: Rol + Tarea + Contexto + Restricciones + Plantilla de salida** (4 min — explicación con plantilla visual que queda fija en pantalla todo el bloque)
- **Plantillas de salida** (3 min): cómo incluir en el prompt el formato esperado de la respuesta — tabla, listado, borrador de oficio con secciones fijas. Concepto clave: "si no le decís cómo responder, la IA inventa el formato". Ejemplo de plantilla de oficio genérico:
  ```
  OFICIO N°: {{numero}}
  Destinatario: {{destinatario}}
  Asunto: {{asunto}}
  Cuerpo: {{cuerpo}}
  Firma: {{firma}}
  ```
- **Demo 1 — Prompt vago vs. prompt estructurado** (5 min): el docente escribe un prompt vago en vivo, muestra el resultado pobre, luego lo reescribe con la estructura completa y el grupo compara los dos resultados en pantalla.
- **Demo 2 — Prompt con restricción de confidencialidad** (4 min): el docente agrega "respondé solo con la información que te proveo, no inventes datos faltantes" y muestra cómo cambia el comportamiento. Conexión directa con el principio human-first: el humano decide qué datos entran al prompt y qué datos no.
- **Demo 3 — De la respuesta al .docx vía MCP** (4 min): el docente copia los campos de la respuesta estructurada de ChatGPT y los pasa al tool `edu.generar_oficio_docx`. Se genera un `.docx` listo para usar. Mensaje clave: "la IA produce el borrador, el sistema produce el documento, **la persona firma**."
- **Construcción colectiva** (4 min): el docente proyecta una situación nueva (ej: redactar un oficio o un texto explicativo para una parte) y el grupo dicta en voz alta el prompt + la plantilla de salida; el docente lo escribe, ejecuta y genera el .docx en tiempo real.

**Objetivo de bloque:** Que el participante comprenda la estructura del prompt, sepa incluir una plantilla de salida para obtener respuestas predecibles y pueda dictar o corregir un prompt oralmente verificando el resultado en pantalla.

**Estrategia pedagógica:** Todas las interacciones son demos en vivo proyectadas — el docente opera la herramienta, los participantes observan, diagnostican y proponen mejoras oralmente. No se requiere ningún dispositivo individual.

**Material de apoyo:** Slide fija con la plantilla `[Rol] + [Tarea] + [Contexto] + [Restricciones] + [Plantilla de salida]` visible durante todo el bloque. Una filmina adicional con 2–3 ejemplos de plantillas de salida típicas del PJN (tabla de campos de oficio, listado numerado, borrador con secciones fijas).

**Nota de scope:** La búsqueda estructurada de jurisprudencia se difiere al Encuentro 2 (donde se trabaja a fondo con NotebookLM y verificación contra Saij/Infojus). Aquí se prioriza el oficio porque es el caso de uso más universal en el público objetivo.

**Filminas estimadas:** 8–9

### Bloque 5b — Demo avanzada: sentencia en lenguaje claro → .docx (15 min)

> **Nota de scope:** Este bloque es la culminación práctica del encuentro. Muestra el flujo completo con privacidad garantizada: documento de referencia como contexto → anonimización local → prompt reutilizable → salida estructurada → .docx generado por MCP con datos reales restituidos localmente.

**Subtemas:**
- **El problema** (1 min): las sentencias judiciales son largas, técnicas y difíciles de entender para las partes. El lenguaje claro es una política pública adoptada en varios tribunales argentinos.
- **El prompt reutilizable y la guía de referencia** (3 min): el docente muestra brevemente `guia-lenguaje-claro.md` (principios: oraciones cortas, voz activa, evitar latinismos) y `prompt-sentencia-lenguaje-claro.md` (prompt completo con la plantilla embebida). Concepto a transmitir: "el contexto se pega en el prompt; el prompt es reutilizable; sólo cambian los datos del caso".
- **Demo en vivo — flujo de 4 pasos con privacidad** (8 min):
  1. El docente tiene un texto con datos de un caso **ficticio** (no usar causas reales, ni siquiera públicas).
  2. Invoca `edu.anonimizar_documento` vía MCP → Presidio (Microsoft) detecta nombres, organizaciones, fechas y los reemplaza con marcadores `{{PERSON_1}}`, `{{ORG_1}}`, etc. El mapping real→marcador se guarda en `anon_mapping.json` localmente. **Ningún dato real sale hacia ChatGPT.**
  3. El texto anonimizado se pega en el prompt reutilizable y se envía a ChatGPT → responde con la sentencia en lenguaje claro, manteniendo los marcadores.
  4. Se invoca `edu.generar_sentencia_docx` con la respuesta + la ruta del `anon_mapping.json` → el MCP sustituye los marcadores por los valores reales y genera el `.docx` final con nombres reales — sin que hayan salido del sistema.
- **Reflexión final y principio human-first** (3 min): diferencia entre "usar IA para hacer el trabajo del juez/a" vs "usar IA como asistente de redacción con el criterio del juez/a". Regla: **el contenido jurídico lo decide el magistrado o magistrada — la IA da forma, no criterio**. El flujo demostrado preserva ambas cosas: privacidad de los datos y autoridad humana sobre el contenido.

**Objetivo de bloque:** Que el participante vea en acción un flujo completo y real que respeta confidencialidad y autoridad humana. Que entienda que la IA no reemplaza el juicio jurídico sino que acelera la redacción bajo supervisión humana.

**Archivos de demo en la carpeta del tema:**
- `guia-lenguaje-claro.md` — principios de lenguaje claro para sentencias (fuentes: lenguajeclaroargentina.gob.ar)
- `prompt-sentencia-lenguaje-claro.md` — prompt reutilizable con plantilla de sentencia embebida
- Tool MCP: `edu.anonimizar_documento` (Microsoft Presidio) → genera `anon_mapping.json`
- Tool MCP: `edu.generar_sentencia_docx` → acepta `ruta_mapping` para revertir anonimización en el .docx

**Mensaje clave sobre privacidad:**
> "El dato real nunca sale al exterior: se anonimiza antes de ir a ChatGPT y se restituye localmente al generar el documento."

**Estrategia pedagógica:** Demo completamente en pantalla proyectada. El docente opera — los participantes observan. El impacto está en ver que un documento institucional formal sale en menos de un minuto con formato correcto y con datos sensibles que nunca abandonan el equipo.

**Filminas estimadas:** 4–5

### Bloque 6 — Cierre (9 min)

**Los 6 conceptos clave del día** (slide de síntesis, nombrarlos explícitamente):
1. Los **LLMs (ChatGPT, Claude, Gemini)** son una rama del Deep Learning dentro del universo más amplio de la IA.
2. La IA genera texto **probable** — no garantiza verdad.
3. **El humano decide primero**: la IA propone, la persona valida, decide y firma.
4. **Nunca pegar datos reales** en un chat público; cuando sea imprescindible, anonimizar antes.
5. El **contexto del prompt** determina la calidad de la respuesta.
6. ChatGPT hoy tiene **3 modos avanzados** — GPTs personalizados, modo agente, búsqueda profunda — cada uno con su uso.

**Dinámica de cierre:**
- El docente proyecta los 6 puntos y pide al grupo que mencione cuál le parece más útil para su trabajo diario — mano alzada o comentario libre (2 min)
- Mensaje central en voz alta: **"La IA no garantiza verdad: genera respuestas plausibles. El humano decide primero."** (1 min)
- Ronda de preguntas abiertas — el docente responde hasta 3 preguntas breves; las que requieran desarrollo se difieren al Encuentro 2 (4 min)
- Anuncio del Encuentro 2 y entrega de materiales ("el link a los prompts usados queda en el grupo institucional") (2 min)

**Filminas:** 2 (síntesis de los 6 conceptos + mensaje clave final)

---

## Filminas estimadas: 37–45 filminas

> Distribución orientativa (ajustable por Roberto en la redacción):
> - 1 portada
> - 1 agenda
> - 5–6 bloque 1 (diagrama de círculos concéntricos IA→ML→DL→LLM, predictor de palabras, tabla buscador/BD/LLM, glosario)
> - 4–5 bloque 2 (tabla de herramientas, casos de uso, "humano primero")
> - 6–7 bloque 3 (1 por riesgo + caso Mata vs Avianca + principio rector)
> - 1 agenda al retomar de la pausa
> - 2–3 bloque 4 (ventana de contexto)
> - 5–6 bloque 4b (intro "cómo cambió ChatGPT", GPTs, modo agente, búsqueda profunda, tabla "cuándo usar cada modo")
> - 8–9 bloque 5 (plantilla de prompt + demos del oficio)
> - 4–5 bloque 5b (demo avanzada: anonimización + sentencia en lenguaje claro)
> - 2 cierre (síntesis de 6 conceptos + mensaje clave)

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
2. Bloque 3 — al final de cada uno de los 5 riesgos, como cierre operativo.
3. Bloque 4b — al presentar el modo agente, donde el riesgo de delegación es mayor.
4. Bloque 5 y 5b — como recordatorio al iniciar el bloque práctico.

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
| Proyector / pantalla | Obligatorio | Toda la clase es proyectada — sin proyector no se puede dictar |
| Laptop del docente | Obligatorio | Con acceso a ChatGPT y MCP server corriendo |
| Conexión a internet | Obligatorio | Necesario para ChatGPT y Gemini (si se generan imágenes) |
| Pizarrón o flip chart | Recomendado | Para anotar prompts que surjan del grupo en el Bloque 5 |
| Micrófono | Recomendado en salas >15 personas | Voz clara es clave para las demos |

### Software y cuentas
| Herramienta | Estado requerido | Verificación pre-clase |
|-------------|----------------|------------------------|
| ChatGPT (cuenta del docente) | Activa y con sesión iniciada | Abrir y hacer un prompt de prueba |
| MCP server EDU (`edu-mcp-server/server.py`) | Corriendo en localhost | `python edu-mcp-server/server.py` — verificar que responde |
| Python + `python-docx` | Instalado | `python -c "import docx; print('ok')"`|
| `oficio_desde_template.py` | Presente en carpeta del tema | Fallback si MCP falla |
| `guia-lenguaje-claro.md` | Presente en carpeta del tema | Contexto para Bloque 5b |
| `prompt-sentencia-lenguaje-claro.md` | Presente en carpeta del tema | Prompt demo para Bloque 5b |

---

## Setup técnico pre-clase

> Ejecutar **al menos 30 minutos antes** del inicio. No hacerlo en el momento — las demos en vivo requieren que todo esté probado.

1. **Iniciar MCP server:** `python edu-mcp-server/server.py` — dejar corriendo en una terminal
2. **Test `edu.generar_oficio_docx`:** ejecutar una generación de oficio de prueba con datos ficticios — verificar que el `.docx` se genera correctamente
3. **Test `edu.anonimizar_documento`:** correr anonimización sobre un texto de prueba — verificar que genera `anon_mapping.json`
4. **Abrir ChatGPT** y dejar la sesión iniciada — hacer al menos un prompt para confirmar que no hay bloqueo de red
5. **Abrir los archivos de demo** en el editor: `guia-lenguaje-claro.md` y `prompt-sentencia-lenguaje-claro.md` — listos para copiar
6. **Preparar el texto ficticio** para la demo de Bloque 5b: resolución o sentencia con datos inventados coherentes (no usar causas reales aunque sean públicas)
7. **Proyectar la slide de portada** antes de que entre el grupo — confirmar que la escala de fuente es legible desde el fondo de la sala

---

## Contingencias técnicas

| Escenario | Plan B |
|-----------|--------|
| **ChatGPT caído o sin internet** | Mostrar capturas de pantalla pre-grabadas de los resultados esperados. Continuar la clase como demo conceptual — el docente explica el resultado en lugar de generarlo. |
| **MCP server no arranca** | Usar `oficio_desde_template.py` como fallback para la Demo 4. Para la Demo 5b (Bloque 5b), mostrar el `.docx` pre-generado que debe estar en la carpeta. |
| **Sin proyector** | La clase no puede dictarse en formato demo. Opción: redirigir a discusión grupal con los prompts escritos en pizarrón y resultados leídos en voz alta. Notificar a coordinación. |
| **El grupo usa sus propios dispositivos** | No es el formato esperado, pero si surgen espontáneamente, aprovechar para comparar resultados. Recordar la regla de privacidad antes de que peguen cualquier contenido. |
| **Preguntas que se extienden demasiado** | El docente usa la frase: "Eso lo desarrollamos en el Encuentro 2 — lo anoto para no perderlo." Anota en el pizarrón y continúa. |

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
5. **Duración:** No usar los 120 min como límite estricto — el docente avanza más rápido. Generar el contenido completo sin recortar bloques para ajustar al tiempo estimado.

---

## Criterios de aprobación del diseño

- [ ] Duración total ≤ 120 minutos con los bloques propuestos
- [ ] Los 5 tópicos del plan-mínimo (Día 1) están cubiertos
- [ ] Los LLMs están ubicados explícitamente dentro del mapa general de la IA (jerarquía IA→ML→DL→LLM en Bloque 1)
- [ ] El panorama de herramientas relevantes para PJN aparece nombrado (Bloque 2)
- [ ] El principio "el humano decide primero" está enunciado en al menos 4 momentos de la clase
- [ ] Las 3 configuraciones avanzadas de ChatGPT (GPTs, agente, búsqueda profunda) están cubiertas con para qué sirve cada una (Bloque 4b)
- [ ] El diseño es ejecutable por un docente con perfil investigador
- [ ] El público objetivo (no técnico) puede seguir el hilo sin perderse — los tecnicismos están acompañados de analogías o glosario
- [ ] El bloque de prompting es enteramente en vivo (demo proyectada por el docente — sin dispositivos individuales)
