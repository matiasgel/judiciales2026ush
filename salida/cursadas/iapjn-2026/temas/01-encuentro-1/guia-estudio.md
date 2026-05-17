# Guía de estudio — Encuentro 1

> **Para repasar después de la clase. Te llevás esto a casa y lo leés con tiempo.**

**Materia:** Inteligencia Artificial en el Poder Judicial de la Nación
**Encuentro:** 1 — Entender para no equivocarse
**Duración estimada de lectura:** 40 minutos

---

## Cómo usar esta guía

- Leela una vez completa, de corrido, sin tomar notas.
- Volvé sobre las secciones que te dejaron dudas.
- Hacé los ejercicios de autoevaluación al final.
- Si una respuesta no te sale, no busques en internet — volvé al texto.
- La frase **"el humano decide primero"** aparece varias veces. No es repetición: es la regla rectora del curso.

---

## 1. ¿Qué es la inteligencia artificial?

La inteligencia artificial (IA) es un conjunto de **programas que aprenden a hacer tareas que antes requerían inteligencia humana**. No es una sola tecnología — es un campo muy grande con muchas ramas.

Ya usás IA todos los días sin pensarlo:

- El filtro de spam de tu correo.
- Las recomendaciones de Netflix o Spotify.
- El autocomplete del teclado del celular.
- Los asistentes de voz (Siri, Alexa, Google Assistant).

Lo nuevo en estos años **no es la IA** — la IA tiene más de 60 años de historia. Lo nuevo son los **LLMs** (modelos de lenguaje grandes) como ChatGPT, Claude y Gemini, que en 2022–2025 cambiaron radicalmente lo que se puede hacer con texto.

### Cómo se ubica un LLM dentro de la IA

Pensalo como **círculos concéntricos** — del universo más amplio al más específico:

1. **IA** (universo entero) — cualquier sistema que imita capacidades humanas.
2. **Machine Learning (ML)** — IA que aprende de ejemplos. Filtro de spam, scoring crediticio.
3. **Deep Learning (DL)** — ML con redes neuronales grandes. Reconocimiento facial, traducción automática.
4. **LLM** — Deep Learning especializado en lenguaje. ChatGPT, Claude, Gemini, Copilot.

> Cuando hoy alguien dice "IA", en el 90% de los casos habla de un LLM. **Pero IA es mucho más grande.**

### Cómo funciona un LLM, en una sola idea

Un LLM es **un predictor de la palabra siguiente**. Punto.

Durante su entrenamiento, leyó millones de textos y aprendió qué palabra suele venir después de cierta secuencia. Cuando le hacés una pregunta, calcula la palabra más probable que sigue, y otra, y otra — hasta que arma una respuesta completa.

> **Parece que entiende — pero está calculando probabilidades, no comprendiendo.**

Por eso un LLM no es lo mismo que:

| | Buscador (Google) | Base de datos (SAIJ) | LLM (ChatGPT) |
|---|---|---|---|
| **Qué hace** | Encuentra | Almacena hechos verificados | Genera texto probable |
| **¿Garantiza verdad?** | Sigue la fuente | Sí (lo que está cargado) | **No — puede inventar** |
| **¿Cita la fuente?** | Sí (link) | Sí (registro) | A veces — y puede mentir |

---

## 2. Herramientas y usos en el Poder Judicial

### Las cinco herramientas más relevantes hoy

| Herramienta | Quién la hace | Para qué sirve | Acceso |
|---|---|---|---|
| **ChatGPT** | OpenAI | Conversación, redacción, análisis de texto | chatgpt.com |
| **Claude** | Anthropic | Textos largos, raciocinio jurídico | claude.ai |
| **Gemini** | Google | Integrado con servicios Google | gemini.google.com |
| **NotebookLM** | Google | "Cuaderno" con documentos propios cargados | notebooklm.google.com |
| **Copilot** | Microsoft | Integrado en Word, Outlook, Edge | Microsoft 365 |

En el curso usamos **ChatGPT** como ejemplo principal — es la más difundida y la que más opciones de configuración tiene. Pero lo que aprendas se aplica casi igual a las demás.

### Seis usos concretos en el PJN

1. **Redacción de oficios** — borrador inicial a partir de datos básicos.
2. **Resumen de expedientes** — síntesis por tema. ⚠️ Atención con datos sensibles.
3. **Mejora de redacción** — lenguaje más claro, formal o accesible.
4. **Búsqueda de jurisprudencia** — organizar criterios. ⚠️ Verificar siempre en SAIJ/InfoJus.
5. **Traducción** de documentos en idiomas extranjeros.
6. **Explicar tecnicismos** a partes no profesionales (sentencia en lenguaje claro).

### Principio rector — el humano decide primero

En todos estos casos la IA **produce un borrador**. La firma, el criterio jurídico y la decisión son siempre humanos.

> **Si una IA decide en el Poder Judicial, dejamos de tener Poder Judicial.**

---

## 3. Primera mirada a ChatGPT

Cuando llegues a casa y quieras probar ChatGPT, este es el mapa.

### Acceder

- Abrí cualquier navegador (Chrome, Firefox, Edge).
- Andá a **chatgpt.com**.
- Creá una cuenta gratuita con tu correo o cuenta Google.
- No se instala nada.

### El mapa de la interfaz

Cinco lugares que conviene ubicar:

- **Barra lateral izquierda** — el historial de tus conversaciones. Cada chat es independiente.
- **Área central** — la conversación en curso.
- **Caja de texto inferior** — donde escribís el *prompt* (la pregunta o instrucción).
- **Selector de modelo (arriba)** — GPT-4o, GPT-4o mini, etc. Dejá el que viene por defecto.
- **Botón "New chat"** — abre una conversación nueva, con la memoria en blanco.
- **Ícono de perfil (arriba a la derecha)** — Settings, donde están los controles de privacidad (sección 7 de esta guía).

> La interfaz cambia cada pocos meses — OpenAI actualiza el diseño. **Los elementos clave siempre están, a veces en distinto lugar.**

### Tres reglas antes del primer prompt

1. **No pegar información sensible** de expedientes.
2. Lo que genera es un **borrador** — siempre revisar.
3. **Revisar los controles de privacidad** antes de usar para tareas del PJN.

---

## 4. Riesgos — el humano decide primero

### Riesgo 1 — Alucinaciones

Una **alucinación** es cuando el modelo **inventa información que suena creíble**. Es especialmente peligroso con fallos, artículos legales, números de expediente. La IA escribe con la misma seguridad cuando dice verdad y cuando inventa — **no avisa**.

### El caso argentino real — Rosario, agosto 2025

En la Cámara Civil de Rosario, ante el juez **Oscar Puccinelli**, un abogado presentó un escrito de apelación citando jurisprudencia que **no existía**. Ante la observación del tribunal, reconoció haber usado ChatGPT para buscar precedentes y **no haber verificado las citas**.

El juez Puccinelli escribió textualmente:

> *"Es sumamente riesgoso y hasta temerario delegar la labor de búsqueda de jurisprudencia de soporte y luego volcarla sin cotejar la fuente."*

**Resultado:** la apelación fue rechazada, el abogado recibió una reprensión y se notificó al Tribunal de Ética.

Casos similares se replicaron en **Cipolletti (Río Negro, 2025)**, donde un tribunal dejó sin honorarios a dos abogados por la misma razón, y en otros fueros del país.

> **Regla humana primero:** ningún dato que entregue la IA —especialmente jurisprudencia, artículos o números de expediente— se cita sin verificar en la fuente oficial (SAIJ, InfoJus, sitio del tribunal). El precio de saltarse este paso, en Argentina, ya tiene jurisprudencia propia.

### Riesgo 2 — Confidencialidad y datos sensibles

Cuando pegás texto en ChatGPT con la **configuración por defecto de una cuenta personal**, esa información **puede ser usada para reentrenar al modelo**.

**Implicancias en el PJN:**

- Datos de partes, testigos, menores.
- Secreto de sumario.
- Datos médicos.
- Datos de víctimas o testigos protegidos.

> **Regla humana primero:** la decisión de qué sale del sistema la toma siempre la persona — nunca por reflejo, nunca por comodidad.

En la sección 7 (privacidad) vemos cómo desactivar el entrenamiento. En la sección 8 (anonimización) vemos cuándo aplicarla.

### Riesgo 3 — Sesgos

Los modelos aprenden de textos existentes y pueden reproducir **sesgos de género, etnia o clase social** en redacción de resoluciones, descripciones de personas o evaluaciones.

> **Regla humana primero:** la persona revisa el lenguaje del borrador antes de firmar. No se acepta texto generado sin lectura crítica.

### Riesgo 4 — Confianza excesiva / dependencia

"Si lo dijo la IA, debe ser verdad" es el reflejo más peligroso. Con el tiempo se pierde el hábito de verificar. **El caso de Rosario es ilustrativo:** el abogado actuó con la confianza de que el resultado de ChatGPT era jurisprudencia real.

> **Regla humana primero:** mantené el hábito de leer críticamente lo que escribe la IA — igual que leerías un borrador de un practicante nuevo.

### Riesgo 5 — Trazabilidad y responsabilidad

Si una IA "sugirió" un texto que firmaste, **la responsabilidad sigue siendo del firmante**. No hay "culpa de la IA" — los abogados sancionados en Rosario y Río Negro **no pudieron alegar la culpa del modelo**.

> **Regla humana primero:** la firma humana implica que el firmante asume todo el contenido como propio.

### Síntesis

> **La IA propone borradores. El humano decide, valida y firma. Si quitamos al humano del medio, perdemos el control de la justicia — y, como mostró la Cámara de Rosario, terminamos pagando el costo profesional.**

---

## 5. La ventana de contexto

La **ventana de contexto** es la memoria de trabajo de la IA **durante una conversación**.

### La metáfora del pizarrón

Imaginá un pizarrón en un aula:

- Mientras estamos en la clase, todo lo que se escribe en el pizarrón está disponible para todos.
- Cuando termina la clase, el pizarrón se borra.
- La próxima clase empieza con el pizarrón en blanco.

Lo mismo pasa con ChatGPT: mientras estás en una conversación, el modelo ve todo lo escrito hasta ese punto. Cuando cerrás el chat, el "pizarrón" se borra y el modelo no recuerda nada de la próxima vez que abras un chat nuevo.

### Por qué importa en el PJN

Si abrís un chat nuevo y solo escribís *"redactá un oficio"*, **la IA no sabe nada del caso**. Tenés que darle el contexto cada vez:

- Tipo de causa.
- Partes intervinientes.
- Datos relevantes.
- Resultado esperado.

**Sin contexto, el resultado es genérico o inventado.**

### Límite práctico

Los modelos actuales aceptan documentos largos (varias decenas de páginas), pero **al final de textos muy largos suelen "olvidar" lo del principio**. Práctica recomendada: trozos manejables, pedidos específicos.

---

## 6. Cómo escribir un buen prompt

Un **prompt** es lo que vos le escribís al modelo. La calidad del prompt determina la calidad de la respuesta — esto se llama **prompt engineering** y es la habilidad clave para usar bien cualquier LLM.

### La plantilla — cinco componentes

| Componente | Qué significa | Ejemplo |
|---|---|---|
| **Rol** | Desde qué perspectiva actúa la IA | "Sos asistente redactor del PJN" |
| **Tarea** | La acción concreta | "Redactá un oficio de citación" |
| **Contexto** | Información del caso | "Juzgado de familia N.º 3 de Ushuaia, causa [N°], convocado [NOMBRE]" |
| **Restricciones** | Qué no hacer o cómo hacerlo | "Sin latinismos. Sin tuteo. Máximo 3 párrafos." |
| **Plantilla de salida** | Estructura esperada del resultado | "Encabezado, cuerpo, cierre con fórmula PJN" |

### Prompt vago vs. prompt estructurado

**Vago:**
```
Redactá un oficio.
```
→ Resultado genérico, incompleto, requiere mucha corrección.

**Estructurado:**
```
Sos asistente redactor del PJN. Redactá un oficio de citación a testimonio
para el juzgado de familia N.º 3 de Ushuaia. El convocado es [NOMBRE],
la causa es [NÚMERO], la fecha de audiencia es [FECHA] a las [HORA].
Usá lenguaje formal, sin tuteo, con la fórmula de cierre:
'Sin otro particular, saludo a Ud. atte.' No uses latinismos.
```
→ Resultado útil, directamente aprovechable.

> **La diferencia no está en la IA. Está en la instrucción.**

### Las restricciones — el control judicial sobre el borrador

Las restricciones son **instrucciones preventivas**. Son la forma en que el operador judicial controla el comportamiento de la IA **antes de que genere la respuesta**.

Ejemplo de restricción importante:

```
No hagas referencia a ningún dato del expediente en el asunto
ni en el cuerpo del correo — sólo en el adjunto.
```

> **No hace falta confiar en la IA. Hace falta darle las reglas correctas desde el inicio.**

---

## 7. Configuraciones de ChatGPT y privacidad

ChatGPT hoy es **una plataforma con varios modos**:

- **Chat normal** — pregunta y respuesta.
- **GPTs personalizados** — un ChatGPT a medida que configurás una vez (rol, tono, reglas, plantilla) y reusás. Requiere cuenta Plus.
- **Modo agente** — ChatGPT que ejecuta pasos por su cuenta: abre páginas, llena formularios, descarga archivos. ⚠️ **Nunca dejarlo operar sobre sistemas internos del PJN ni con credenciales institucionales**.
- **Búsqueda profunda (Deep Research)** — toma varios minutos, consulta múltiples fuentes, produce un informe extenso con citas. ⚠️ **Las citas se verifican una por una — recordar el caso de Rosario.**

### Privacidad — bloque crítico para uso en PJN

**El problema en una frase:** en una cuenta personal con la configuración de fábrica, **todo lo que escribas en ChatGPT puede ser usado por OpenAI para entrenar futuros modelos**.

#### Control 1 — Desactivar el entrenamiento

1. Clic en el **ícono de perfil** (arriba a la derecha).
2. **Settings**.
3. **Data Controls**.
4. Desactivar el toggle **"Improve the model for everyone"** ("Mejorar el modelo para todos").

**Efecto:** las conversaciones siguen guardándose en tu historial, **pero OpenAI ya no las usa para entrenar**.

> **Importante:** este control existe en la versión gratuita y en la versión Plus. **Hay que activarlo explícitamente — no viene así por defecto.**

#### Control 2 — Chat temporal

El "modo incógnito" de ChatGPT. Botón al iniciar un chat nuevo → **Chat temporal**.

**Efecto:** ese chat **no se guarda en el historial**, **no se usa para entrenar** y **no genera memoria persistente**. Se elimina automáticamente en 30 días.

**Caso de uso PJN:** cualquier consulta donde experimentes con texto sensible y no convenga dejar rastro.

#### Control 3 — Memoria entre chats

ChatGPT puede "recordar" cosas dichas en chats anteriores. Se controla en: **Settings → Personalization → Memory**.

> **Recomendación para uso PJN:** desactivar la memoria o revisarla periódicamente. No queremos que el modelo conserve fragmentos de casos previos entre sesiones.

#### Control 4 — Cuentas Business / Enterprise / Edu

**Por defecto, las cuentas Business, Team, Enterprise y Edu de ChatGPT NO usan los datos del usuario para entrenar al modelo.** El contrato comercial activa esa protección automáticamente.

**Implicancia institucional:** si el PJN decide alguna vez contratar ChatGPT a nivel institucional, hereda esta protección. **En cambio, una cuenta personal de un agente requiere la configuración manual descrita arriba.**

> **La privacidad en ChatGPT no es automática en cuentas personales — hay que activarla.**

### Cuándo usar cada modo

| Tarea | Modo recomendado |
|---|---|
| Redactar un texto recurrente con formato fijo (oficios, cédulas) | **GPT personalizado** |
| Recolectar datos públicos de varias páginas en una tabla | **Modo agente** (con verificación) |
| Producir un informe doctrinario o de panorama extenso | **Búsqueda profunda** |
| Consulta puntual con texto sensible que no debe quedar en historial | **Chat temporal** |
| Pregunta rápida, ajuste de redacción, traducción | Chat normal (con "Improve the model" desactivado) |

---

## 8. Sentencia en lenguaje claro y anonimización

### El problema del lenguaje judicial

Las sentencias están escritas para abogados, pero **las partes tienen derecho a entender qué se decidió sobre su caso**. El lenguaje claro es una **política pública** adoptada en varios tribunales argentinos.

La IA acelera la reescritura — el contenido jurídico lo sigue decidiendo el magistrado.

### Prompt reutilizable para sentencia en lenguaje claro

```
Reescribí este fragmento de resolución judicial en lenguaje claro,
usando oraciones cortas, voz activa, sin latinismos y sin perder
ningún dato sustancial. Conservá la estructura: encabezado, hechos,
decisión, fundamento.

[pegar fragmento]
```

### Anonimización — la segunda capa de protección

**Anonimizar** es reemplazar datos reales por etiquetas genéricas **antes** de pegar texto en cualquier herramienta de IA.

**Ejemplo:**

| Texto original | Texto anonimizado |
|---|---|
| La parte actora, **María González Díaz**, | La parte actora, **PERSONA_1**, |
| domiciliada en **Av. Mitre 1234 de Rosario**, | domiciliada en **DIRECCIÓN_1**, |
| representada por el Dr. **Juan Pérez** | representada por el Dr. **PERSONA_2** |

**Flujo de tres pasos:**

1. **Anonimizar** el texto (búsqueda y reemplazo manual en un editor).
2. **Pegar en ChatGPT** → la IA trabaja solo con etiquetas.
3. **Sustituir las etiquetas** por los datos reales antes de usar el documento.

### Cuándo anonimizar en el PJN

- Expedientes con **datos de menores** → obligación legal de reserva.
- **Víctimas o testigos con protección de identidad** → dato que no debe circular.
- **Datos médicos y psicológicos** de las partes → sensibilidad especial.
- **Secreto de sumario** → el contenido no debe salir del sistema judicial.

> **La anonimización es una segunda capa sobre los controles de privacidad — no son excluyentes, se complementan.**

---

## 9. Glosario

- **Alucinación** — Cuando un LLM inventa información que suena creíble pero es falsa. Especialmente peligroso con fallos, artículos legales o números de expediente.
- **Anonimización** — Reemplazar datos reales (nombres, direcciones, DNI) por etiquetas genéricas (PERSONA_1, DIRECCIÓN_1) antes de procesar el texto en una herramienta de IA.
- **Chat temporal** — Modo de ChatGPT que no guarda la conversación en el historial, no se usa para entrenamiento y no genera memoria persistente.
- **Deep Learning (DL)** — Rama del Machine Learning basada en redes neuronales grandes.
- **GPT personalizado** — Configuración guardada de ChatGPT que se reutiliza para tareas recurrentes (rol, tono, reglas, plantilla).
- **IA (Inteligencia Artificial)** — Conjunto de programas que imitan capacidades humanas.
- **LLM (Large Language Model)** — Modelo de lenguaje grande. ChatGPT, Claude, Gemini son LLMs.
- **Machine Learning (ML)** — IA que aprende de ejemplos.
- **Modo agente** — Modo de ChatGPT en que ejecuta pasos por su cuenta (abre páginas, llena formularios, descarga archivos).
- **Prompt** — Lo que el usuario le escribe al modelo. La instrucción.
- **Prompt engineering** — La habilidad de escribir prompts efectivos.
- **Ventana de contexto** — La memoria de trabajo de la IA durante una conversación. Se borra al cerrar el chat.

---

## 10. Autoevaluación

> Respondé de memoria. Si no te sale, volvé al texto.

### Verdadero o falso

1. Un LLM **garantiza** que las citas que produce son verdaderas. (V / F)
2. La ventana de contexto se mantiene entre chats distintos. (V / F)
3. En una cuenta personal de ChatGPT con configuración de fábrica, los chats se usan para entrenar al modelo. (V / F)
4. Las cuentas Business y Enterprise **NO** usan los datos del usuario para entrenar. (V / F)
5. La firma humana implica asumir todo el contenido del documento como propio, aunque lo haya redactado una IA. (V / F)

### Completar

6. La frase rectora del encuentro es: "La IA no garantiza verdad: genera respuestas plausibles. El humano _______."
7. El abogado sancionado en Rosario en 2025 fue advertido por el juez Puccinelli porque presentó jurisprudencia _______.
8. La metáfora que usamos para explicar la ventana de contexto fue: el _______ que se borra entre clases.
9. Los cinco componentes del prompt estructurado son: Rol, Tarea, _______, Restricciones y Plantilla de salida.
10. Antes de pegar texto con datos sensibles en ChatGPT, conviene _______ ese texto.

### Aplicación

11. Listá los cuatro casos del PJN donde la anonimización es claramente requerida.
12. Mencioná dos diferencias entre el modo agente y la búsqueda profunda.
13. Explicá con tus palabras por qué un LLM no es lo mismo que un buscador.

### Respuestas

1. F — un LLM **no** garantiza verdad; calcula la palabra más probable.
2. F — la ventana de contexto se borra al cerrar el chat (metáfora del pizarrón).
3. V — por eso hay que activar el control manualmente.
4. V — la protección viene por contrato comercial.
5. V — no hay "culpa de la IA".
6. **decide primero**.
7. **inexistente / inventada** (generada por ChatGPT sin verificar).
8. **pizarrón**.
9. **Contexto**.
10. **anonimizar**.
11. Menores, víctimas o testigos protegidos, datos médicos/psicológicos, secreto de sumario.
12. Modo agente: ejecuta pasos en navegador (abrir páginas, llenar formularios). Búsqueda profunda: produce un informe extenso con citas verificables tras varios minutos de investigación.
13. Un buscador encuentra contenido existente y cita la fuente; un LLM genera texto probable y puede inventar (alucinar).

---

## 11. Referencias y lecturas sugeridas

- **Caso Cámara Civil Rosario, agosto 2025** — juez Oscar Puccinelli. Cita textual incluida en la sección 4 de esta guía.
- **Caso Cipolletti, Río Negro, 2025** — tribunal civil deja sin honorarios a dos abogados por jurisprudencia inventada con ChatGPT.
- **Política pública de lenguaje claro** — Procuración General de la Nación y otras jurisdicciones provinciales en Argentina.
- **OpenAI Help Center — Data Controls** — documentación oficial sobre cómo desactivar el entrenamiento sobre chats propios.

---

## 12. Frase para llevarse a casa

> **La IA no garantiza verdad: genera respuestas plausibles. El humano decide primero.**

Si te llevás solamente una idea del Encuentro 1, que sea esta.

Nos vemos en el Encuentro 2.
