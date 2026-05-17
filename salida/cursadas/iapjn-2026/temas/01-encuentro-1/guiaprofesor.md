# Guía del profesor — Encuentro 1

> Documento operativo del docente. Complementa minuta.md (qué decir) con **cómo conducir la clase, contingencias y material de demo listo para copiar**.

**Materia:** Inteligencia Artificial en el Poder Judicial de la Nación
**Encuentro:** 1 — Entender para no equivocarse
**Duración:** 120 min
**Modalidad:** Presencial con proyección vía Google Meet

---

## 1. Checklist pre-clase (T-30 min)

### Equipamiento

- [ ] Proyector encendido y enfocado
- [ ] Laptop docente conectada a corriente
- [ ] Internet probado (velocidad ≥ 20 Mbps, ChatGPT responde sin lag)
- [ ] Micrófono operativo (si la sala es grande)
- [ ] Botella de agua a mano

### Software abierto y listo

- [ ] **Google Meet** — reunión iniciada, compartir pantalla activado, audio del docente verificado
- [ ] **Navegador con dos pestañas:**
  - Pestaña 1 — `chatgpt.com` logueado con cuenta docente (Plus recomendado)
  - Pestaña 2 — editor de texto con material de demo (ver sección 2)
- [ ] **GPT personalizado** "Redactor de Oficios PJN" probado y accesible
- [ ] **Filminas** abiertas en pantalla completa, proyectadas vía Google Meet
- [ ] **Memoria de ChatGPT** y **Improve the model** en estado conocido (para mostrar antes/después en F-34)

### Material físico opcional

- [ ] Marcador y notas para uno mismo (no hay pizarrón físico en la sala — toda la proyección es vía Google Meet)
- [ ] Reloj o cronómetro visible (Pomodoro 25/5 sirve)

---

## 2. Material de demo listo para copiar

### Fragmento de sentencia ficticia (Bloque 5b, F-40)

> **⚠️ Personajes y hechos completamente inventados. No usar causas reales ni siquiera públicas.**

```
RESOLUCIÓN N° 247/2026

VISTOS: estos autos caratulados "PEREZ, MARIO RICARDO C/ EMPRESA LOGÍSTICA
NORTE S.A. S/ DAÑOS Y PERJUICIOS" (Expte. N° 3458/2025), traídos a despacho
para resolver, y CONSIDERANDO:

Que la parte actora, mediante presentación de fs. 142/156, ha interpuesto
recurso de apelación contra la sentencia de fecha 12 de febrero de 2026
dictada por la Sra. Juez de Primera Instancia, mediante la cual se rechazó
la pretensión indemnizatoria. Que el recurrente fundamenta su agravio en
una pretendida errónea valoración de la prueba testimonial obrante a fs.
89/92, así como en la omisión del análisis de la pericia técnica de fs.
105/118. Que examinadas las constancias de autos en su totalidad, este
Tribunal advierte que los testimonios glosados a fs. 89 y 91 resultan
contestes en cuanto al modo de producción del evento dañoso, y que las
conclusiones periciales no fueron objeto de impugnación en término. Por
ello, corresponde acoger los agravios formulados.

POR ELLO, FALLAMOS: I) Revocar la sentencia apelada. II) Hacer lugar a la
demanda. III) Costas de ambas instancias al vencido.
```

### Prompt reutilizable para reescribir en lenguaje claro (F-40)

```
Reescribí este fragmento de resolución judicial en lenguaje claro, usando
oraciones cortas, voz activa, sin latinismos y sin perder ningún dato
sustancial. Conservá la estructura: encabezado, hechos, decisión,
fundamento.

[PEGAR EL FRAGMENTO DE ARRIBA]
```

### Tabla ORIGINAL → ANONIMIZADO (F-41) — para mostrar en pantalla

```
ORIGINAL:
"La parte actora, María González Díaz, domiciliada en Av. Mitre 1234 de
Rosario, representada por el Dr. Juan Pérez, demanda a la empresa
Transportes del Sur S.A."

ANONIMIZADO:
"La parte actora, PERSONA_1, domiciliada en DIRECCIÓN_1, representada por
el Dr. PERSONA_2, demanda a la empresa ORG_1."
```

### Prompt para construcción colectiva (F-28) — caso de reserva si nadie propone

> Usar solo si el grupo no propone nada en 30 segundos.

```
Tarea propuesta: "Notificación al asegurador del demandado tras sentencia firme"

Lo armamos juntos en 5 componentes:

Rol: Sos asistente redactor del PJN, especialista en notificaciones formales.
Tarea: Redactá una notificación dirigida a la compañía aseguradora del
       demandado, comunicando que la sentencia ha quedado firme.
Contexto: Causa "[ACTOR] C/ [DEMANDADO] S/ DAÑOS Y PERJUICIOS", Expte.
          N° [NÚMERO], juzgado civil N° [NÚMERO] de Ushuaia. La aseguradora
          es [NOMBRE].
Restricciones: Lenguaje formal, sin tuteo. Máximo 4 párrafos. No incluir
               datos personales de las partes en el asunto del correo —
               sólo en el cuerpo.
Plantilla de salida: encabezado con datos del expediente, párrafo de
                     comunicación, párrafo con plazos, cierre con fórmula
                     PJN.
```

### Prompts para Demo 1 (F-26)

**Versión vaga:**
```
Redactá un oficio.
```

**Versión estructurada:**
```
Sos asistente redactor del PJN. Redactá un oficio de citación a testimonio
para el juzgado de familia N.º 3 de Ushuaia. El convocado es JUAN PEREZ,
la causa es 12345/2025, la fecha de audiencia es 15 de mayo a las 10:00 hs.
Usá lenguaje formal, sin tuteo, con la fórmula de cierre: "Sin otro
particular, saludo a Ud. atte." No uses latinismos.
```

### Prompt para Demo 2 (F-27) — restricción de confidencialidad

```
[Mismo prompt anterior, agregando esta línea al final:]

No hagas referencia a ningún dato del expediente en el asunto ni en el
cuerpo del correo — sólo en el adjunto.
```

### Pregunta de seguimiento sugerida para F-11

```
Primer prompt en F-11:
"¿Qué es un oficio judicial y para qué sirve?"

Seguimiento (sin repetir contexto, para mostrar que recuerda la sesión):
"Dame un ejemplo concreto de oficio de citación."
```

---

## 3. Ritmo y manejo del grupo

### Cronograma fino

| Min | Bloque | Filmina | Energía esperada |
|-----|--------|---------|------------------|
| 0–5 | B0 Apertura | F-00, F-01 | Alta, expectativa |
| 5–20 | B1 ¿Qué es IA? | F-02 a F-06 | Atención conceptual |
| 20–30 | B2 Herramientas | F-07 a F-09 | Atención aplicada |
| 30–37 | B2b Interfaz | F-10 a F-12 | Pico de curiosidad (primer ChatGPT) |
| 37–52 | B3 Riesgos | F-13 a F-20 | Pico emocional en F-15 (caso Rosario) |
| 52–58 | B4 Contexto | F-21 a F-23 | Atención conceptual |
| 58–80 | B5 Prompting | F-24 a F-28 | Más alta del día — práctica |
| 80–95 | B4b Configs | F-29 a F-38 | Posible cansancio — micropausa si hace falta |
| 95–108 | B5b Lenguaje claro | F-39 a F-43 | Pico de utilidad percibida |
| 108–120 | B6 Cierre | F-44, F-45 | Síntesis, mensaje rector |

### Puntos de máxima atención (no fallar)

1. **F-15 — Cita textual del juez Puccinelli.** Leer pausado, en voz alta. Hacer silencio breve después. Es el momento de mayor impacto del día.
2. **F-25 — Plantilla del prompt.** Dejarla visible durante toda la demo de B5. Si la perdés de vista, los participantes pierden el hilo.
3. **F-34 — Demo de privacidad.** Mostrar el switch antes y después en la pantalla real de ChatGPT. Sin esto, el mensaje de privacidad pierde concreción.
4. **F-45 — Mensaje rector final.** Leer en voz alta, sin apuro: *"La IA no garantiza verdad: genera respuestas plausibles. El humano decide primero."*

### Lectura del grupo

- **Si miran el celular en B1–B2:** son los bloques más expositivos. Acelerá y llegá rápido a F-10 (primera demo).
- **Si toman notas frenéticamente en B3:** ritmo adecuado, no acelerar.
- **Si surgen muchas preguntas en B5:** señal positiva. Tomar 1–2, derivar las complejas al final.
- **Si bostezan en B4b:** ofrecer micropausa informal de 2–3 min antes de F-33. Esos minutos salen de la holgura del Bloque 6.

### Manejo de preguntas

- **Pregunta dentro de scope, breve:** responder en el momento, máx 30 segundos.
- **Pregunta dentro de scope, compleja:** "Buena pregunta — la respondo al cierre del bloque" y volver.
- **Pregunta fuera de scope:** "Eso lo vemos en el Encuentro 2/3, viene después".
- **Pregunta sobre cuenta personal o caso real privado:** "Lo conversamos al final, fuera de la grabación de Google Meet".

---

## 4. Contingencias

### Tecnológicas

| Problema | Acción |
|----------|--------|
| **Se cae internet** | Continuar con filminas en pantalla local. Demos se difieren al final del bloque correspondiente. Si no vuelve, sustituir demos por explicación verbal apoyándose en F-26/F-27/F-34 que ya tienen el código mostrado. |
| **ChatGPT lento (lag > 10 seg)** | No esperar en silencio: usar el tiempo para repasar la filmina. Si persiste, mostrar resultado preparado. |
| **Demo se traba o da error raro** | No insistir más de 1 minuto. Decir "esto a veces pasa — el modelo no está disponible" y pasar al siguiente punto. |
| **Google Meet se cuelga** | Reiniciar share screen. Si no funciona, cambiar a proyección directa (HDMI). Avisar que se interrumpió la grabación. |
| **GPT personalizado no responde** | Saltar la demo de F-30 — describir verbalmente. No es crítica. |

### Pedagógicas

| Situación | Acción |
|-----------|--------|
| **Cansancio cerca del min 80** | Micropausa informal de 2–3 min antes de F-33 (privacidad). Esos minutos vienen de la holgura del Bloque 6. |
| **Nadie propone tarea en F-28** | Usar el caso de reserva (notificación al asegurador, sección 2 de esta guía). |
| **Participante muy escéptico** ("esto es peligroso, no debería usarse") | Validar la preocupación. Volver a la regla rectora: "Por eso decimos *el humano decide primero*". Continuar. |
| **Participante muy entusiasta** ("¿puede hacer todo?") | Validar el entusiasmo. Recordar caso Rosario. Volver a la regla rectora. |
| **Pregunta política o institucional** ("¿el PJN va a contratar ChatGPT?") | "No es nuestra decisión. Lo que mostramos hoy aplica con cuenta personal y con cuenta institucional — los criterios de uso responsable son los mismos." |
| **Pregunta sobre IA fuera de LLMs** (autos autónomos, reconocimiento facial) | Validar, ubicar en el mapa de F-03. "Es IA pero no LLM — hoy nos enfocamos en LLMs." |

### Si el grupo va más rápido de lo previsto

> El docente conoce el material y suele terminar antes de los 120 min — es esperable.

- **No estirar artificialmente.** Cerrar antes y dedicar el tiempo sobrante a preguntas abiertas.
- **No agregar contenido fuera de scope.** El plan mínimo está cerrado en 5 tópicos.
- **Si quedan más de 10 min libres al final:** pedir a 2–3 participantes que cuenten cómo aplicarían algo de lo visto en su área específica.

---

## 5. Errores a evitar (lecciones acumuladas)

- ❌ **Decir "ChatGPT entiende".** Decir "ChatGPT calcula la palabra más probable".
- ❌ **Decir "la IA garantiza".** La IA no garantiza nada — esa es la regla rectora.
- ❌ **Mostrar la cita del juez Puccinelli sin leerla en voz alta.** Pierde 80% del impacto.
- ❌ **Saltarse la demo de privacidad (F-34) por falta de tiempo.** Es la única acción concreta que el participante puede hacer al volver a casa hoy. Si hay que sacrificar algo, sacrificar Demo 2 del modo agente (F-31).
- ❌ **Usar datos reales en la demo de F-40.** Siempre ficticio.
- ❌ **Decir "anonimizar es fácil".** Decir "anonimizar es manual y requiere atención — por eso conviene tener un buen reemplazo en mente".
- ❌ **Comprometer fechas de futuros encuentros sin confirmar el cronograma.**

---

## 6. Mapa rápido filmina → recursos

| Filmina | Recurso necesario |
|---------|-------------------|
| F-00 a F-09 | Solo filminas — exposición |
| F-10 | Mostrar chatgpt.com en navegador |
| F-11 | ChatGPT abierto + primer prompt en vivo |
| F-12 | Solo filmina — síntesis |
| F-13 a F-20 | Solo filminas — la cita de F-15 se lee del texto en la slide |
| F-21 a F-25 | Solo filminas — exposición conceptual |
| F-26 | ChatGPT en pantalla + prompts de la sección 2 de esta guía |
| F-27 | Continuar el chat de F-26, agregar línea de restricción |
| F-28 | ChatGPT en pantalla + caso del grupo (o caso de reserva) |
| F-29 | Solo filmina |
| F-30 | GPT personalizado preconfigurado abierto |
| F-31 | Filmina + demo opcional de modo agente (si hay tiempo) |
| F-32 | Solo filmina — describir Deep Research verbalmente |
| F-33 a F-37 | ChatGPT abierto en Settings → Data Controls + Personalization → Memory |
| F-38 | Solo filmina — tabla de decisión |
| F-39 | Solo filmina |
| F-40 | Texto ficticio de sentencia (sección 2) + ChatGPT en pantalla |
| F-41 | Editor de texto con tabla ORIGINAL → ANONIMIZADO (sección 2) |
| F-42, F-43 | Solo filminas |
| F-44 | Solo filmina + ronda de comentarios del grupo |
| F-45 | Solo filmina + anuncio del Encuentro 2 |

---

## 7. Anti-cheat: tres frases que el docente NO debe decir

1. ❌ "Confíen en la IA" — siempre decir "verifiquen lo que dice la IA".
2. ❌ "Esto es seguro" — decir "esto es responsable si seguimos estas reglas".
3. ❌ "La IA piensa / entiende / sabe" — decir "la IA calcula / genera / predice".

---

## 8. Cierre operativo

- [ ] Después de F-45, dejar la portada (F-00) en pantalla mientras los participantes salen.
- [ ] Detener grabación de Google Meet.
- [ ] Cerrar pestaña con datos de demo (por si quedó histórico visible).
- [ ] **Borrar el chat usado en las demos** (especialmente si pegó algún dato que terminó pareciéndose a algo real).
- [ ] Si activó "Improve the model OFF" para la demo de F-34, decidir si lo deja así o lo vuelve a su estado original.
- [ ] Guardar el GPT personalizado para reusar en Encuentro 2.
- [ ] Enviar al grupo institucional:
  - Link a `guia-estudio.md`
  - Link a los prompts usados (los de la sección 2 de esta guía)
  - Confirmación de fecha del Encuentro 2

---

## 9. Apéndice — frases rectoras para memorizar

> Estas se repiten varias veces durante la clase. Conviene saberlas de memoria.

1. **"La IA propone borradores. El humano decide, valida y firma."**
2. **"Si una IA decide en el Poder Judicial, dejamos de tener Poder Judicial."**
3. **"La diferencia no está en la IA. Está en la instrucción."**
4. **"No hace falta confiar en la IA. Hace falta darle las reglas correctas desde el inicio."**
5. **"La privacidad en ChatGPT no es automática en cuentas personales — hay que activarla."**
6. **"La IA no garantiza verdad: genera respuestas plausibles. El humano decide primero."** _(mensaje rector final)_

---

> **Cierre interno del docente:** si los participantes salen recordando una sola cosa, que sea: *el humano decide primero*. Todo lo demás se aprende con la práctica de los próximos encuentros.
