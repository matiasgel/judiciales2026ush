# Clase: Encuentro 1 — Entender para no equivocarse

**Materia:** Inteligencia Artificial en el Poder Judicial de la Nación
**Duración:** 120 min
**Modalidad:** Presencial con proyección vía Google Meet (compartir pantalla)
**Total de filminas:** 46

---

## Objetivos

Al finalizar el encuentro, el participante podrá:

1. Explicar con sus propias palabras qué es la inteligencia artificial, ubicar a los LLMs (ChatGPT, Claude, Gemini) dentro del mapa general y diferenciarlos de un buscador o base de datos.
2. Identificar al menos dos casos de uso concreto de IA en tareas del PJN y reconocer las herramientas más relevantes.
3. Nombrar los principales riesgos del uso de IA en contextos legales y aplicar el principio "el humano decide primero", apoyándose en el caso real de Rosario 2025.
4. Describir qué es la ventana de contexto y cómo afecta la calidad de la respuesta.
5. Reconocer las configuraciones actuales de ChatGPT — GPTs personalizados, modo agente, búsqueda profunda y controles de privacidad — y saber para qué sirve cada una.
6. Formular un prompt básico con estructura: Rol + Tarea + Contexto + Restricciones + Plantilla de salida.

---

## Setup pre-clase (5 minutos antes)

1. Abrir ChatGPT en una pestaña, logueado con la cuenta docente (Plus si es posible para mostrar GPT personalizado)
2. Tener preparado el fragmento de **sentencia ficticia** para la demo de B5b
3. Tener preparado el ejemplo **ORIGINAL → ANONIMIZADO** en un editor de texto visible
4. Abrir Google Meet, iniciar reunión y compartir pantalla con el navegador
5. Proyectar la portada (F-00) vía Google Meet antes de que entre el grupo

---

## BLOQUE 0 — Apertura (5 min)

### [F-00] Portada
**Tiempo:** 1 min
**Qué decir:**
- Saludo, bienvenida, breve presentación personal del docente
- "Esta clase está enteramente proyectada vía Google Meet — todos vemos lo mismo, nadie necesita laptop ni celular"
- Mencionar que la IA será el eje del curso completo y que hoy se sientan las bases conceptuales
**Conceptos clave:** encuadre, modalidad presencial + Google Meet
**Preguntas anticipadas:**
- "¿Hay que instalar algo?" → No, hoy no
- "¿Vamos a usar nuestras propias cuentas?" → Hoy observamos; las cuentas las usaremos en encuentros siguientes
**Transición:** "Antes de arrancar, miremos lo que vamos a ver"

### [F-01] Agenda del día
**Tiempo:** 4 min
**Qué decir:**
- Recorrer los 10 puntos de la agenda sin profundizar
- Anticipar el caso argentino real (Rosario 2025) como momento alto del bloque de riesgos
- Aclarar la regla rectora: "La IA no garantiza verdad; el humano decide primero" — la repetiremos varias veces durante el día
**Conceptos clave:** scope del encuentro, modalidad de trabajo, principio rector
**Preguntas anticipadas:**
- "¿Va a haber tareas para casa?" → Habrá un encuentro 2 con práctica
- "¿Esto sirve para mi área específica?" → Sí, los ejemplos cubren oficios, expedientes, jurisprudencia
**Transición:** "Empecemos por entender qué es esto que llamamos IA"

---

## BLOQUE 1 — ¿Qué es la IA? Dónde están los LLMs (15 min)

### [F-02] ¿Qué es la inteligencia artificial?
**Tiempo:** 3 min
**Qué decir:**
- Definición operativa: programas que imitan capacidades antes consideradas exclusivamente humanas
- Ejemplos cotidianos: spam, recomendaciones, autocomplete, asistentes de voz
- "La IA está hace décadas — lo nuevo no es la IA, son los LLMs"
**Conceptos clave:** IA operativa, ubicuidad
**Preguntas anticipadas:**
- "¿La IA piensa?" → No, calcula
- "¿Tiene conciencia?" → No
**Transición:** "Si la IA es esto, ¿dónde entra ChatGPT?"

### [F-03] El mapa de la IA — dónde están los LLMs
**Tiempo:** 4 min
**Qué decir:**
- Recorrer los círculos del más grande al más chico
- IA → ML → DL → LLM, con un ejemplo de cada nivel
- "Cuando hoy alguien dice IA, en el 90% de los casos habla de un LLM. Pero IA es mucho más grande"
**Conceptos clave:** jerarquía conceptual, ubicación de los LLMs
**Preguntas anticipadas:**
- "¿Y los autos autónomos?" → IA + DL, pero no LLM
- "¿Reconocimiento facial es lo mismo?" → DL pero no LLM
**Transición:** "Ahora veamos cómo funciona un LLM por dentro"

### [F-04] Cómo funciona un LLM en una sola idea
**Tiempo:** 4 min
**Qué decir:**
- "Un LLM es un predictor de la palabra siguiente. Punto."
- Lo hizo millones de veces sobre millones de textos en el entrenamiento
- Ejemplo en vivo: leer en voz alta "El acusado se presenta ante el..." y dejar que el grupo complete
- "Parece que entiende — pero calcula probabilidades, no comprende"
**Conceptos clave:** predicción de tokens, no hay comprensión
**Preguntas anticipadas:**
- "¿Entonces miente?" → No miente, completa con lo más probable
- "¿Por eso inventa fallos?" → Exacto, lo veremos en el Bloque 3
**Transición:** "Ahora veamos qué NO es un LLM"

### [F-05] Qué NO es un LLM
**Tiempo:** 3 min
**Qué decir:**
- Recorrer la tabla columna por columna: buscador, base de datos, LLM
- Énfasis en la fila "Garantiza verdad": **No — puede inventar**
- "Esta diferencia es la que nos lleva al bloque 3 (riesgos)"
**Conceptos clave:** garantía de verdad, diferencia con buscador y BD
**Preguntas anticipadas:**
- "¿Entonces no sirve para buscar jurisprudencia?" → Sirve para organizar criterios, no para confirmar fuentes
**Transición:** "Antes de cerrar el bloque, fijemos vocabulario"

### [F-06] Glosario de bolsillo
**Tiempo:** 1 min
**Qué decir:**
- LLM, prompt, alucinación — tres palabras que se usan todo el día en este curso
- "Si las anotan, alcanza con eso"
**Conceptos clave:** vocabulario mínimo
**Preguntas anticipadas:** (ninguna típica)
**Transición:** "Sabiendo qué es un LLM, veamos qué herramientas concretas hay y cómo se usan en el PJN"

---

## BLOQUE 2 — Herramientas de IA y usos en el PJN (10 min)

### [F-07] Panorama actual de herramientas
**Tiempo:** 3 min
**Qué decir:**
- Recorrer las 5 herramientas: ChatGPT, Claude, Gemini, NotebookLM, Copilot
- "Vamos a usar ChatGPT como ejemplo principal porque es la más difundida y la que más configuraciones tiene"
- "Lo que aprendan se aplica casi igual al resto"
- Aclarar: existen otras herramientas (buscadores con IA), las dejamos fuera para no dispersarnos
**Conceptos clave:** panorama, focalización en ChatGPT
**Preguntas anticipadas:**
- "¿Cuál es mejor?" → Depende del uso; hoy nos enfocamos en ChatGPT
- "¿Hay alguna argentina?" → No con esta escala
**Transición:** "Veamos casos concretos donde otros compañeros ya usan estas herramientas"

### [F-08] Casos de uso concretos en el PJN
**Tiempo:** 5 min
**Qué decir:**
- Recorrer los 6 casos uno por uno con un ejemplo breve
- Marcar los dos que tienen "atención":
  - Resumen de expedientes → cuidado con datos sensibles (B3)
  - Búsqueda de jurisprudencia → siempre verificar en SAIJ/InfoJus (caso Rosario)
- "El caso 1 — redacción de oficios — lo vamos a ver en demo en el Bloque 5"
- "El caso 6 — explicar tecnicismos — lo vamos a ver en demo en el Bloque 5b"
**Conceptos clave:** 6 usos, dos con alerta
**Preguntas anticipadas:**
- "¿Puedo subir un expediente entero?" → No con datos reales; lo vemos en B3 y B5b
**Transición:** "Antes de pasar al siguiente bloque, fijemos el principio que va a aparecer una y otra vez"

### [F-09] Encuadre human-first
**Tiempo:** 2 min
**Qué decir:**
- Leer la frase en voz alta: "Si una IA decide en el Poder Judicial, dejamos de tener Poder Judicial"
- "Esto no es un eslogan: es la regla de uso para todo lo que sigue"
- Anticipar que la frase vuelve en B3, B4b, B5, B5b y B6
**Conceptos clave:** humano decide primero
**Preguntas anticipadas:**
- "¿Pero la IA no decide nada?" → Propone, sugiere; la firma y la decisión son humanas
**Transición:** "Vamos a abrir ChatGPT por primera vez juntos"

---

## BLOQUE 2b — Primera mirada a ChatGPT (7 min)

### [F-10] Acceso — chatgpt.com
**Tiempo:** 1 min
**Qué decir:**
- "Abrimos un navegador, vamos a chatgpt.com — no se instala nada"
- Mostrar pantalla de login vía Google Meet
- "Hoy yo opero, ustedes observan; la primera vez es de visita guiada"
**Conceptos clave:** acceso web, cuenta gratuita
**Preguntas anticipadas:**
- "¿Necesito crear cuenta?" → Sí, gratuita; con correo o Google
**Transición:** "Ya estamos adentro — veamos qué tenemos en pantalla"

### [F-11] Mapa de la interfaz de ChatGPT
**Tiempo:** 3 min
**Qué decir:**
- Mostrar la pantalla real de ChatGPT vía Google Meet
- Señalar uno por uno: barra lateral, área central, caja de texto, selector de modelo, "New chat", ícono de perfil
- Advertir: "La interfaz cambia cada pocos meses, los elementos clave siempre están — a veces en distinto lugar"
**Conceptos clave:** 5 lugares clave de la interfaz
**Preguntas anticipadas:**
- "¿Qué modelo conviene?" → El que viene por defecto está bien para hoy
- "¿Las conversaciones se guardan solas?" → Sí, en la barra lateral
**Transición:** "Hagamos el primer prompt en vivo"

> **Demo en vivo (3 min, dentro de F-11):** el docente escribe en ChatGPT *"¿Qué es un oficio judicial y para qué sirve?"* — el grupo observa la generación token por token. Mostrar también: pregunta de seguimiento sin repetir contexto, botón copiar, botón regenerar, botón new chat.

### [F-12] Tres reglas básicas antes de usar ChatGPT
**Tiempo:** 3 min
**Qué decir:**
- Recorrer las 3 reglas en voz alta
- "Estas tres cosas son lo que se llevan hoy si no se llevan nada más: no pegar datos sensibles, todo es borrador, revisar privacidad"
**Conceptos clave:** 3 reglas básicas, anclaje al human-first
**Preguntas anticipadas:**
- "¿Y si me equivoco y pegué algo?" → Borrar el chat ayuda; ideal es no pegar
**Transición:** "Ahora que vimos cómo se ve, hablemos de los riesgos antes de aprender a sacarle provecho"

---

## BLOQUE 3 — Riesgos: el humano decide primero (15 min)

### [F-13] Principio rector del bloque y del encuentro
**Tiempo:** 1 min
**Qué decir:**
- Leer en voz alta y pausada: "El humano decide primero. La IA propone. La persona valida, decide y firma."
- "Esta frase la vamos a repetir al cerrar cada riesgo"
**Conceptos clave:** principio rector
**Preguntas anticipadas:** (ninguna típica — momento de anclaje)
**Transición:** "Empezamos por el riesgo más conocido"

### [F-14] Riesgo 1 — Alucinaciones
**Tiempo:** 2 min
**Qué decir:**
- "Alucinación = el modelo inventa información que suena creíble"
- Especialmente peligroso con fallos, artículos legales, números de expediente
- "La IA escribe con la misma seguridad cuando dice verdad y cuando inventa — no avisa"
**Conceptos clave:** alucinación, sin avisos
**Preguntas anticipadas:**
- "¿Se puede saber cuándo está alucinando?" → No directamente; por eso se verifica
**Transición:** "Esto no es teoría. Veamos un caso argentino reciente"

### [F-15] Caso argentino real — Cámara Civil de Rosario, agosto 2025
**Tiempo:** 3 min
**Qué decir:**
- Leer la cita textual del juez Puccinelli en voz alta, despacio
- Contar el caso: abogado presentó apelación con jurisprudencia inexistente generada por ChatGPT, reconoció no haber verificado
- Consecuencia: apelación rechazada, reprensión, notificación al Tribunal de Ética
- "Este momento es el de mayor impacto del bloque — quiero que esta cita la recuerden cuando lleguen al PJN mañana"
**Conceptos clave:** caso real, consecuencia profesional concreta
**Preguntas anticipadas:**
- "¿Es público?" → Sí, fue ampliamente difundido en la prensa jurídica
- "¿La sanción fue grave?" → Tribunal de Ética, no es menor
**Transición:** "Y no fue un caso aislado"

### [F-16] El caso no fue único — Argentina ya tiene jurisprudencia propia
**Tiempo:** 1 min
**Qué decir:**
- Recorrer la tabla: Rosario, Cipolletti, otros fueros
- "El precio profesional de no verificar lo que dice la IA ya tiene jurisprudencia en Argentina"
**Conceptos clave:** multiplicidad de casos
**Preguntas anticipadas:** (ninguna típica)
**Transición:** "Pasamos al segundo riesgo, conectado con cómo cuidamos los datos"

### [F-17] Riesgo 2 — Confidencialidad y datos sensibles
**Tiempo:** 2 min
**Qué decir:**
- "En cuenta personal con configuración de fábrica, todo lo que pegues puede usarse para reentrenar al modelo"
- Implicancia PJN: partes, testigos, menores, secreto de sumario, datos médicos
- **Regla humana primero:** qué sale del sistema lo decide la persona, nunca por reflejo
- Anticipar: "En Bloque 4b vemos cómo desactivar el entrenamiento; en Bloque 5b vemos cuándo anonimizar"
**Conceptos clave:** entrenamiento por defecto, alcance en PJN
**Preguntas anticipadas:**
- "¿Y si borro el chat?" → Mejor que no pegarlo, pero ya viajó al servidor
**Transición:** "Tercer riesgo — la IA hereda lo que aprendió"

### [F-18] Riesgo 3 — Sesgos
**Tiempo:** 2 min
**Qué decir:**
- "Los modelos aprenden de textos existentes; reproducen sesgos de género, etnia, clase social"
- Aparecen en redacción de resoluciones, descripciones de personas, evaluaciones
- **Regla humana primero:** revisar el lenguaje del borrador antes de firmar
**Conceptos clave:** sesgo heredado, revisión humana
**Preguntas anticipadas:**
- "¿Se puede entrenar sin sesgos?" → No completamente; por eso siempre se revisa
**Transición:** "El riesgo siguiente es más sutil — el de costumbre"

### [F-19] Riesgo 4 — Confianza excesiva / dependencia
**Tiempo:** 2 min
**Qué decir:**
- "Si lo dijo la IA, debe ser verdad" — el reflejo más peligroso
- Con el tiempo se pierde el hábito de verificar
- "El caso Rosario es ilustrativo: el abogado actuó con la confianza de que ChatGPT decía jurisprudencia real"
- **Regla humana primero:** leer críticamente, como se leería un borrador de un practicante nuevo
**Conceptos clave:** automatización mental, hábito de verificar
**Preguntas anticipadas:**
- "¿Y si lo uso mucho?" → Más razón para mantener el reflejo crítico
**Transición:** "Último riesgo — la responsabilidad"

### [F-20] Riesgo 5 — Trazabilidad y responsabilidad
**Tiempo:** 2 min
**Qué decir:**
- "Si una IA sugirió un texto que se firmó, la responsabilidad sigue siendo del firmante"
- "No hay culpa de la IA — los abogados sancionados en Rosario y Río Negro no pudieron alegarla"
- Cerrar el bloque con la síntesis: "La IA propone borradores. El humano decide, valida y firma. Si quitamos al humano del medio, perdemos el control de la justicia"
**Conceptos clave:** firma humana = responsabilidad total
**Preguntas anticipadas:**
- "¿Las empresas que hacen IA no son responsables?" → Comercialmente sí; profesionalmente firma el humano
**Transición:** "Sabemos los riesgos. Ahora vamos a una idea técnica clave para entender cómo escribir buenos prompts: la ventana de contexto"

---

## BLOQUE 4 — Ventana de contexto (6 min)

### [F-21] Qué es la ventana de contexto
**Tiempo:** 2 min
**Qué decir:**
- "Es la memoria de trabajo de la IA durante una conversación"
- Metáfora del **pizarrón que se borra entre clases**: mientras estamos hablando, ve todo lo escrito; cuando cerrás el chat, se borra
- "La próxima vez que abras un chat nuevo, no recuerda nada de vos"
**Conceptos clave:** memoria de trabajo, borrado entre sesiones
**Preguntas anticipadas:**
- "¿Y la función Memory que mencionaste?" → Eso es otra cosa que vemos en B4b
**Transición:** "Vamos al efecto práctico"

### [F-22] Por qué importa en el PJN
**Tiempo:** 2 min
**Qué decir:**
- "Si abrís un chat nuevo y solo escribís 'redactá un oficio', la IA no sabe nada del caso"
- Hay que darle contexto cada vez: tipo de causa, partes, datos relevantes, resultado esperado
- Sin contexto → resultado genérico o inventado
- Límite práctico: docs largos se aceptan, pero "olvidan" lo del principio cuando son muy extensos
**Conceptos clave:** contexto explícito por sesión, límite práctico
**Preguntas anticipadas:**
- "¿Puedo cargar un PDF largo?" → Sí, mejor en trozos manejables
**Transición:** "Esta idea nos lleva directo al núcleo del día"

### [F-23] Regla práctica y puente al prompting
**Tiempo:** 2 min
**Qué decir:**
- "Si el contexto es clave, el prompt tiene que llevarlo todo"
- Trozos manejables y pedidos específicos
- "Ahora pasamos al bloque más operativo: cómo escribir un prompt útil"
**Conceptos clave:** prompt = contenedor del contexto
**Preguntas anticipadas:** (ninguna típica)
**Transición:** "Bienvenidos al bloque de prompting"

---

## BLOQUE 5 — Introducción al prompting (22 min)

### [F-24] Por qué la forma de pedir afecta el resultado
**Tiempo:** 1 min
**Qué decir:**
- "La IA responde con la granularidad que le dás"
- Orden vaga → respuesta genérica; instrucción precisa → borrador útil
- "Esto se llama prompt engineering — es la habilidad clave para usar bien cualquier LLM"
- Recordatorio human-first: lo que sigue produce **borradores**
**Conceptos clave:** prompt engineering, calidad-en-calidad-fuera
**Preguntas anticipadas:**
- "¿Hay cursos enteros de esto?" → Sí, pero la base la vemos hoy
**Transición:** "La buena noticia: hay una plantilla"

### [F-25] Plantilla del prompt — cinco componentes
**Tiempo:** 4 min
**Qué decir:**
- Recorrer los 5 componentes con ejemplo breve:
  - **Rol** — "Sos asistente redactor del PJN"
  - **Tarea** — qué acción ("reescribí", "resumí", "listá")
  - **Contexto** — información del caso
  - **Restricciones** — qué no hacer ("sin latinismos", "máx 3 párrafos")
  - **Plantilla de salida** — estructura esperada
- **Importante:** dejar esta filmina visible durante toda la demo siguiente
**Conceptos clave:** 5 componentes del prompt
**Preguntas anticipadas:**
- "¿Tengo que poner los 5 siempre?" → No, pero cuanto más estructurado, mejor resultado
- "¿Va en este orden?" → Es la práctica recomendada
**Transición:** "Veamos en vivo la diferencia"

### [F-26] Demo 1 — Prompt vago vs. prompt estructurado
**Tiempo:** 5 min
**Qué decir:**
- Primero escribir en ChatGPT: *"Redactá un oficio"*
- Leer en voz alta lo que devuelve — genérico, incompleto, requiere mucha corrección
- "Ahora la versión estructurada" — escribir el prompt completo con los 5 componentes (ejemplo de F-26)
- Leer la respuesta — borrador directamente aprovechable
- Cerrar con: "La diferencia no está en la IA. Está en la instrucción."
**Conceptos clave:** comparación demostrada
**Preguntas anticipadas:**
- "¿Siempre funciona así?" → Sí, con consistencia
**Transición:** "Ahora la pieza más importante para el PJN — la restricción de confidencialidad"

### [F-27] Demo 2 — Restricción de confidencialidad
**Tiempo:** 5 min
**Qué decir:**
- Agregar al prompt anterior la línea de restricción: *"No hagas referencia a ningún dato del expediente en el asunto ni en el cuerpo del correo — sólo en el adjunto"*
- Mostrar el resultado — la IA respeta la restricción
- Punto pedagógico clave: "Las restricciones son instrucciones preventivas. Es la forma en que el operador judicial controla el comportamiento de la IA antes de que genere la respuesta"
- "No hace falta confiar en la IA — hace falta darle las reglas correctas desde el inicio"
**Conceptos clave:** restricciones preventivas
**Preguntas anticipadas:**
- "¿La IA siempre respeta las restricciones?" → En general sí, conviene verificar
**Transición:** "Ahora la parte participativa"

### [F-28] Construcción colectiva — armemos un prompt entre todos
**Tiempo:** 7 min (5 min real + 2 min margen)
**Qué decir:**
- "Necesito que alguien me proponga una tarea cotidiana de su oficina: oficio, informe, correo formal, notificación"
- Recibir la propuesta y armar el prompt en pantalla compartida vía Google Meet
- Pedir al grupo que dicte cada componente (rol, tarea, contexto, restricciones, plantilla) — el docente solo escribe lo que ellos proponen
- Si el tiempo lo permite, lanzar el prompt en ChatGPT y leer el resultado en voz alta
- Cierre del bloque: "No es magia. Es estructura."
**Conceptos clave:** apropiación participativa
**Preguntas anticipadas:**
- "¿Y si nadie propone nada?" → Tener un caso de reserva (notificación al asegurador)
**Transición:** "Ya saben prompting básico. Ahora veamos qué configuraciones tiene ChatGPT que multiplican el uso — y los controles de privacidad imprescindibles"

---

## BLOQUE 4b — Configuraciones de ChatGPT (15 min)

### [F-29] Cómo cambió ChatGPT en los últimos meses
**Tiempo:** 1 min
**Qué decir:**
- "Hasta hace poco era un chat. Hoy es una plataforma con varios modos"
- Listar: chat normal, GPTs personalizados, modo agente, búsqueda web, búsqueda profunda, controles de privacidad
- "No hace falta usar todo — sí conviene saber que existen"
**Conceptos clave:** evolución, panorama
**Preguntas anticipadas:** (ninguna típica)
**Transición:** "Empezamos por la función más útil para tareas recurrentes"

### [F-30] Función 1 — GPTs personalizados
**Tiempo:** 3 min
**Qué decir:**
- "Es un ChatGPT a medida que configurás una vez y reutilizás"
- Instrucciones fijas: rol, tono, reglas, plantilla
- Requiere Plus
- Dónde se configura: "Explorar GPTs" → "Crear un GPT"
- **Demo rápida vía Google Meet:** abrir el GPT preconfigurado "Redactor de Oficios PJN", escribir prompt corto, mostrar respuesta directa con plantilla completa
- Regla humano primero: el GPT es un atajo; el contenido sigue siendo revisado y firmado
**Conceptos clave:** GPT personalizado, atajo reutilizable
**Preguntas anticipadas:**
- "¿Lo puedo compartir?" → Sí, con quien quieras o público
- "¿Vale la pena Plus?" → Depende del uso; para tareas recurrentes sí
**Transición:** "Ahora el modo más nuevo y delicado"

### [F-31] Función 2 — Modo agente
**Tiempo:** 3 min
**Qué decir:**
- "ChatGPT que ejecuta pasos por su cuenta — abre páginas, llena formularios, descarga archivos"
- Ejemplo: "buscame los últimos 5 fallos sobre tenencia compartida y armame una planilla"
- **Advertencias críticas — leer pausado:**
  - Puede equivocarse en pasos intermedios sin avisar
  - **Nunca dejarlo operar sobre sistemas internos del PJN ni con credenciales institucionales**
  - Hoy: sólo tareas exploratorias con datos públicos
- Demo opcional si el tiempo y la conexión lo permiten
**Conceptos clave:** modo agente, riesgo amplificado
**Preguntas anticipadas:**
- "¿Puede entrar a SAIJ?" → No deberíamos darle credenciales para sistemas oficiales
**Transición:** "La tercera función avanzada"

### [F-32] Función 3 — Búsqueda profunda (Deep Research)
**Tiempo:** 3 min
**Qué decir:**
- "Tarda varios minutos consultando múltiples fuentes y produce un informe extenso con citas"
- Diferencia con búsqueda normal: respuesta corta vs documento estructurado con referencias
- Ejemplo PJN: "investigación profunda sobre la evolución de la doctrina de prisión preventiva en los últimos 5 años"
- **Limitación crítica:** también puede equivocarse o citar fuentes mal interpretadas
- "Sigue siendo un borrador. Las citas se verifican una por una — recordar el caso de Rosario"
**Conceptos clave:** búsqueda profunda, verificación obligatoria
**Preguntas anticipadas:**
- "¿Es la herramienta más confiable?" → No automáticamente; la verificación sigue
**Transición:** "Y ahora el bloque más importante para el PJN — privacidad"

### [F-33] Función 4 — Privacidad: el problema en una frase
**Tiempo:** 1 min
**Qué decir:**
- "En cuenta personal con configuración de fábrica, todo lo que escribís puede ser usado para entrenar futuros modelos"
- "Para un usuario común es un problema menor; para alguien que pega texto de expediente es un problema grave"
- "Bueno saberlo: estos controles existen y hay que activarlos"
**Conceptos clave:** privacidad no automática
**Preguntas anticipadas:** (ninguna típica — anclaje para demo)
**Transición:** "Demo paso a paso del control más importante"

### [F-34] Control 1 — Desactivar entrenamiento sobre chats propios
**Tiempo:** 2 min
**Qué decir:**
- **Demo en vivo en la pantalla real de ChatGPT compartida vía Google Meet:**
  1. Clic en ícono de perfil arriba a la derecha
  2. **Settings**
  3. **Data Controls**
  4. Desactivar el toggle **"Improve the model for everyone"**
- Mostrar el switch antes y después
- Efecto: las conversaciones siguen guardándose en tu historial, pero OpenAI ya no las usa para entrenar
- "Existe en versión gratuita y Plus. **No viene activado por defecto**"
**Conceptos clave:** Data Controls, switch manual
**Preguntas anticipadas:**
- "¿Tengo que hacerlo cada vez?" → No, una vez y queda
- "¿Funciona retroactivo?" → No, sólo para adelante
**Transición:** "Para conversaciones puntuales sensibles, hay algo más"

### [F-35] Control 2 — Chat temporal
**Tiempo:** 2 min
**Qué decir:**
- "Es el modo incógnito de ChatGPT"
- Botón al iniciar un chat nuevo → **Chat temporal**, o ícono en la cabecera
- Efecto: no se guarda en historial, no se usa para entrenar, no genera memoria persistente, se elimina automáticamente en 30 días
- Caso de uso PJN: consultas puntuales con texto sensible que no convenga dejar rastro
**Conceptos clave:** chat temporal, modo incógnito
**Preguntas anticipadas:**
- "¿Lo puedo recuperar?" → No, ese es el punto
**Transición:** "Hay una tercera configuración que conviene revisar"

### [F-36] Control 3 — Memoria entre chats
**Tiempo:** 2 min
**Qué decir:**
- "ChatGPT puede recordar cosas que dijiste en chats anteriores para personalizar las respuestas"
- Dónde: Settings → **Personalization** → **Memory**
- Permite activar / desactivar / borrar memorias específicas
- **Recomendación para uso PJN:** desactivar o revisar periódicamente
- "No queremos que el modelo conserve fragmentos de casos previos entre sesiones"
**Conceptos clave:** memoria persistente, desactivación recomendada
**Preguntas anticipadas:**
- "¿Es lo mismo que la ventana de contexto?" → No, esa es de la sesión; la memoria es entre sesiones
**Transición:** "Hay una protección automática para cuentas comerciales"

### [F-37] Control 4 — Cuentas Business / Enterprise / Edu
**Tiempo:** 1 min
**Qué decir:**
- "Por defecto, Business / Team / Enterprise / Edu NO usan datos del usuario para entrenar"
- El contrato comercial activa esa protección automáticamente
- **Implicancia institucional:** si el PJN contrata ChatGPT a nivel institucional, hereda esta protección
- "En cambio, cuenta personal de un agente requiere la configuración manual de los controles 1–3"
- Mensaje de cierre del bloque: "La privacidad en ChatGPT no es automática en cuentas personales — hay que activarla. Y aun activándola, el dato sensible real mejor no se pega: se anonimiza primero. Lo vemos ahora."
**Conceptos clave:** protección institucional automática
**Preguntas anticipadas:**
- "¿El PJN tiene contratado algo?" → No es nuestra decisión; conviene saber que existe la opción
**Transición:** "Síntesis del bloque"

### [F-38] Cuándo usar cada modo
**Tiempo:** 1 min
**Qué decir:**
- Recorrer la tabla rápidamente
- "Si no se acuerdan nada de las funciones, alcanza con tener clara la pregunta: '¿para qué tarea uso cuál?'"
**Conceptos clave:** tabla de decisión rápida
**Preguntas anticipadas:** (ninguna típica)
**Transición:** "Vamos al último bloque temático — donde aplicamos todo lo aprendido"

---

## BLOQUE 5b — Sentencia en lenguaje claro y anonimización (13 min)

### [F-39] El problema del lenguaje judicial
**Tiempo:** 1 min
**Qué decir:**
- "Las sentencias están escritas para abogados, pero las partes también tienen derecho a entender"
- Lenguaje claro: política pública en varios tribunales argentinos
- La IA acelera la reescritura — el contenido jurídico lo sigue decidiendo el magistrado
**Conceptos clave:** lenguaje claro como política
**Preguntas anticipadas:**
- "¿Hay una guía oficial?" → Sí, varios protocolos provinciales
**Transición:** "Veamos la demo"

### [F-40] Demo en vivo — sentencia ficticia a lenguaje claro
**Tiempo:** 5 min
**Qué decir:**
- Aclarar: "Este texto es **ficticio**, personajes y hechos inventados — nunca usamos causas reales, ni siquiera públicas"
- Pegar el fragmento en ChatGPT con el prompt reutilizable de F-40
- Leer la respuesta de ChatGPT en voz alta
- Comparar con el original
- Observación pedagógica: "¿Perdió algún matiz? ¿Cambió el sentido de alguna cláusula?"
- "Regla humano-primero en acción — la IA produjo el borrador, nosotros lo evaluamos"
**Conceptos clave:** demo concreta, revisión crítica
**Preguntas anticipadas:**
- "¿Y si la IA cambia el sentido?" → Por eso el firmante revisa siempre
**Transición:** "Y ahora la pregunta clave — ¿y si el texto tiene datos sensibles?"

### [F-41] ¿Y si el texto tiene datos sensibles? — Concepto de anonimización
**Tiempo:** 5 min
**Qué decir:**
- "Antes de pegar texto con datos reales en cualquier herramienta de IA, reemplazamos esos datos por etiquetas genéricas"
- Mostrar la tabla ORIGINAL → ANONIMIZADO en pantalla
- Recorrer cada fila: nombre → PERSONA_1, dirección → DIRECCIÓN_1, etc.
- Explicar el flujo de tres pasos:
  1. Anonimizar manualmente (búsqueda y reemplazo en un editor)
  2. Pegar en ChatGPT → la IA trabaja solo con etiquetas
  3. Sustituir las etiquetas por los datos reales antes de usar el documento
- Mencionar nota de producción: "Encuentros posteriores van a mostrar flujos donde esto se hace de forma automática. Hoy importa que entiendan el concepto"
**Conceptos clave:** anonimización manual, flujo de tres pasos
**Preguntas anticipadas:**
- "¿Pierdo coherencia si anonimizo?" → No si usás etiquetas consistentes
- "¿Vale para nombres extranjeros?" → Sí, mismo principio
**Transición:** "¿Cuándo aplica esto en el PJN?"

### [F-42] Cuándo anonimizar en el PJN
**Tiempo:** 1 min
**Qué decir:**
- Recorrer los 4 casos: menores, víctimas/testigos protegidos, datos médicos, secreto de sumario
- "La anonimización es una segunda capa sobre los controles de privacidad — no son excluyentes, se complementan"
**Conceptos clave:** 4 casos, anonimización como capa adicional
**Preguntas anticipadas:**
- "¿Y para datos de funcionarios públicos?" → Si están en información pública oficial, generalmente no requiere; igual conviene
**Transición:** "Cerramos el bloque con la mirada de fondo"

### [F-43] Reflexión final — uso responsable de IA en el contexto judicial
**Tiempo:** 1 min
**Qué decir:**
- Leer: "La IA acelera la reescritura. El magistrado o magistrada sigue decidiendo el contenido jurídico. La anonimización garantiza que el proceso no comprometa datos sensibles."
- "Las tres cosas juntas hacen que el uso de IA en el ámbito judicial sea **responsable**"
**Conceptos clave:** uso responsable = velocidad + criterio humano + protección de datos
**Preguntas anticipadas:** (ninguna típica — momento de síntesis)
**Transición:** "Llegamos al cierre"

---

## BLOQUE 6 — Cierre (12 min)

### [F-44] Los 7 conceptos clave del día
**Tiempo:** 6 min (2 min recorrido + 4 min ronda)
**Qué decir:**
- Recorrer los 7 conceptos uno por uno, recordando dónde se vio cada uno
- Pedir al grupo que mencione cuál le parece más útil para su trabajo diario — mano alzada o comentario libre
- Tomar 3–5 intervenciones; agradecer y conectar con el resumen
**Conceptos clave:** síntesis del día, apropiación participativa
**Preguntas anticipadas:**
- "¿Tendremos material para repasar?" → Sí, la guía de estudio y la guía del profesor quedan en el grupo institucional
**Transición:** "Cierre con la frase rectora"

### [F-45] Mensaje clave final
**Tiempo:** 6 min (1 min mensaje + 4 min preguntas + 1 min anuncio)
**Qué decir:**
- Leer en voz alta y pausada: **"La IA no garantiza verdad: genera respuestas plausibles. El humano decide primero."**
- Ronda de preguntas abiertas — responder hasta 3 preguntas breves
- Las que requieran desarrollo se difieren al Encuentro 2
- Anuncio del Encuentro 2 y entrega de materiales:
  - "El link a los prompts usados queda en el grupo institucional"
  - "Tienen la guía de estudio para repasar en casa"
- Despedida, agradecimiento, cierre de Google Meet
**Conceptos clave:** mensaje rector, próxima clase
**Preguntas anticipadas:**
- "¿Cuándo es el siguiente encuentro?" → Confirmar fecha
- "¿Hay TP para casa?" → Habrá uno al final del módulo
**Transición:** Fin de la clase.

---

## Anexo — Recursos necesarios

- Proyector + laptop docente + internet estable + micrófono
- Google Meet con compartir pantalla activado
- Cuenta de ChatGPT (idealmente Plus) logueada
- GPT personalizado "Redactor de Oficios PJN" preconfigurado
- Fragmento de **sentencia ficticia** listo para copiar
- Ejemplo **ORIGINAL → ANONIMIZADO** preparado en un editor de texto

## Anexo — Contingencias

- **Si se cae la conexión:** continuar con las filminas en pantalla local; las demos se difieren al final del bloque
- **Si el grupo manifiesta cansancio cerca del minuto 80:** micropausa informal de 2–3 minutos (sale de la holgura del Bloque 6)
- **Si una demo en vivo se traba:** mostrar resultado preparado, no perder más de 1 minuto intentando reproducirla
- **Si alguien propone una tarea fuera de scope en B5:** redirigir a un caso similar dentro del scope
