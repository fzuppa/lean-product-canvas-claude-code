---
name: lean-product-canvas
description: "Use when trabajando en un Lean Product Canvas (LPD): completar una caja a través de preguntas, elegir entre varias opciones generadas, o revisar una caja ya escrita. Triggers: 'Lean Product Canvas', 'LPD', 'caja 1..8', 'business problem statement', 'business outcomes', 'proto-persona', 'JTBD', 'hipótesis del canvas', 'ayudame a completar el canvas', 'revisá mi caja', 'tengo varias opciones para la caja'."
---

# Lean Product Canvas (LPD)

Guía para completar, seleccionar y revisar las 8 cajas del [Lean Product Canvas](https://jeffgothelf.com/blog/the-lean-product-canvas/) de una oportunidad, usando los prompts empaquetados en `references/` (relativo a este archivo). Skill autocontenido: no depende de ninguna carpeta externa al propio skill, solo del proyecto donde se lo invoca para guardar sus resultados.

**Idioma:** este skill y sus prompts están en español. Los archivos LPD que genera también quedan en español.

**Principio del canvas (repetilo cuando corresponda):** los resultados generados por IA son suposiciones que deben validarse, no hechos a aceptar.

## Las 8 cajas

El nombre de la columna "Nombre de sección en el archivo" es el título exacto (bilingüe, español + original en inglés entre paréntesis) que va en el header `## N. <nombre>` del archivo LPD. Usalo siempre así, literal, al crear el scaffold o escribir una sección — no lo traduzcas ni lo abrevies de otra forma.

| # | Nombre de sección en el archivo | Archivo de prompts | Modos disponibles |
|---|------|---------------------|--------------------|
| 1 | Enunciado del Problema de Negocio (Business Problem Statement) | `box1_business_problem_statement.md` | Generar, Seleccionar, Revisar |
| 2 | Outcomes de Negocio (Business Outcomes) | `box2_business_outcomes.md` | Generar, Seleccionar, Revisar |
| 3 | Usuarios y Clientes (Users and customers) | `box3_users_proto_personas.md` | Generar, Revisar |
| 4 | Outcomes de Usuario & Beneficios [JTBD] (User Outcomes) | `box4_user_outcomes_benefits.md` | Generar, Revisar |
| 5 | Soluciones / Features | `box5_solutions_features.md` | Generar, Seleccionar, Revisar |
| 6 | Hipótesis (Hypotheses) | `box6_hypotheses.md` | Generar, Seleccionar, Revisar |
| 7 | Lo Más Importante para Aprender (The Most Important Thing to Learn) | `box7_most_important_thing_to_learn.md` | Generar, Revisar |
| 8 | La Menor Cantidad de Trabajo para Aprenderlo (The Least Amount of Work to Learn It) | `box8_least_amount_of_work_to_learn_it.md` | Generar, Seleccionar, Revisar |

Todos los archivos están en `references/`, relativo a este archivo (SKILL.md). Las cajas 3, 4 y 7 no tienen prompt de Selección porque producen un único artefacto sintetizado, no varias opciones a comparar — si el usuario pide "seleccionar" en una de estas cajas, explicá esto y ofrecé en cambio afinar el resultado con preguntas puntuales o pasar a Revisar.

## Archivo de salida

Cada oportunidad tiene un único archivo `LPD <Oportunidad>.md` (ej. `LPD Academia S&R.md`) dentro de una carpeta de boards del proyecto actual.

### Encontrar o definir la carpeta de boards

Este skill no asume ninguna estructura de carpetas fija — se adapta al proyecto donde se lo use:

1. **Buscar una carpeta ya en uso.** Antes de preguntar nada, buscá en el proyecto actual archivos existentes con el patrón `LPD *.md` (ej. con `find . -iname "LPD *.md"`). Si encontrás alguno, la carpeta que los contiene es la carpeta de boards — usala sin volver a preguntar. Esto hace que, una vez que un proyecto ya tiene un uso previo del skill, la carpeta se seguya usando automáticamente en cualquier instalación.
2. **Si no encontrás ninguno** (primer uso del skill en este proyecto), preguntale al usuario en qué carpeta quiere guardar los archivos LPD de este proyecto (sugerí `Lean Product Canvas Boards/` como default si no tiene preferencia). Creá la carpeta si no existe.

Con la carpeta ya determinada, el archivo de cada oportunidad tiene esta estructura:

```markdown
# LPD <Oportunidad>

## 1. Enunciado del Problema de Negocio (Business Problem Statement)
_Pendiente_

## 2. Outcomes de Negocio (Business Outcomes)
_Pendiente_

## 3. Usuarios y Clientes (Users and customers)
_Pendiente_

## 4. Outcomes de Usuario & Beneficios [JTBD] (User Outcomes)
_Pendiente_

## 5. Soluciones / Features
_Pendiente_

## 6. Hipótesis (Hypotheses)
_Pendiente_

## 7. Lo Más Importante para Aprender (The Most Important Thing to Learn)
_Pendiente_

## 8. La Menor Cantidad de Trabajo para Aprenderlo (The Least Amount of Work to Learn It)
_Pendiente_
```

- **Nombre de la oportunidad:** si no está claro por el contexto de la conversación, preguntá "¿Cómo se llama la oportunidad?" antes de crear o buscar el archivo.
- **Creación:** si `LPD <Oportunidad>.md` no existe todavía en la carpeta de boards determinada arriba, crealo con el scaffold completo de arriba (las 8 cajas en `_Pendiente_`) antes de completar la primera caja.
- **Contenido de cada sección:** solo el **summary conciso** de esa caja (ver más abajo) — no el detalle completo de la conversación, no niveles de confianza, no listas de investigación pendiente. Ese detalle vive en la conversación, no en el archivo.

## Flujo general

1. **Identificar oportunidad y caja.** Si el usuario no especifica la caja, mirá el archivo LPD (si existe) y sugerí la primera caja en `_Pendiente_` como siguiente paso — pero si el usuario pide otra caja específica, atendé esa sin insistir en el orden.
2. **Preguntar por el alcance de la investigación, solo al arrancar la Caja 1 de una oportunidad nueva** (el archivo LPD no existe todavía, o existe pero la Caja 1 sigue en `_Pendiente_`). Antes de tocar el prompt de Generación, preguntale al usuario explícitamente — no asumas ninguna opción por default:
   - **Usar información relacionada del proyecto:** buscá (grep/find por el nombre de la oportunidad y términos afines) notas, canvases previos, análisis de competidores u otro material ya existente en el proyecto, y usalo como contexto/evidencia al generar, citando de dónde sale cada dato.
   - **Ir directo a la Caja 1:** no busques nada más allá de esta conversación; arrancá el prompt de Generación solo con lo que el usuario te cuente.
   Para cajas siguientes de la misma oportunidad no hace falta repetir esta pregunta — el contexto ya reunido (o la decisión de no reunirlo) aplica para toda la oportunidad, salvo que el usuario pida lo contrario.
3. **Detectar el modo** por el lenguaje del pedido (ver tabla abajo). No hace falta un comando exacto.
4. **Ejecutar el modo** siguiendo al pie de la letra las instrucciones del prompt correspondiente (ver "Cómo ejecutar cada modo").
5. **Ofrecer guardar el summary.** Cuando el usuario llegue a un resultado que lo conforma para esa caja (típicamente después de Generar+Seleccionar, o después de incorporar el feedback de Revisar), redactá un summary conciso y mostráselo antes de escribirlo en el archivo.
6. **Guardar con confirmación.** Si la caja ya tiene contenido distinto de `_Pendiente_` en el archivo, mostrá el summary viejo junto al nuevo y preguntá explícitamente si confirmás el reemplazo antes de sobrescribir. Nunca sobrescribas en silencio.
7. **Sugerir el siguiente paso.** Después de guardar, indicá cuál es la próxima caja pendiente, dejando abierto que el usuario elija otra.

### Detectar el modo pedido

| Señal en el pedido del usuario | Modo | Sección del archivo de prompts a usar |
|---|---|---|
| "ayudame a completar/pensar/armar la caja N", "no sé por dónde arrancar con...", "dame opciones para..." | **Generar** | `## PROMPT DE GENERACIÓN` |
| "tengo estas opciones, ayudame a elegir", "generé varias versiones de la caja N", "¿cuál elijo?" | **Seleccionar** | `## PROMPT DE SELECCIÓN` (si existe para esa caja) |
| "revisá mi caja N", "¿cómo quedó esto?", "dame feedback de..." | **Revisar** | `## PROMPT DE REVISIÓN` |

Si el pedido es ambiguo, preguntá cuál de los tres modos quiere antes de asumir.

### Cómo ejecutar cada modo

En todos los casos: leé el archivo `box{N}_*.md` correspondiente, ubicá la sección del modo detectado, y **actuá vos mismo siguiendo esas instrucciones** (no le muestres el prompt en crudo al usuario para que lo pegue en otro lado — vos sos la IA que ese prompt describe).

- **Generar:** el prompt trae placeholders entre corchetes (ej. `[DESCRIBE TU SITUACIÓN]`, `[INSERTA TU DECLARACIÓN DE PROBLEMA DE LA CAJA 1]`). Antes de generar, resolvé esos placeholders:
  - Si el dato ya está en el archivo LPD (ej. el summary de una caja anterior), usalo directo sin volver a preguntar.
  - Si no está disponible, preguntáselo al usuario explícitamente.
  - Con los placeholders resueltos, generá el contenido siguiendo exactamente el formato y la cantidad de opciones que pide el prompt (2-3, 5, etc.), incluyendo supuestos y evidencia de validación cuando el prompt lo pida — eso es para la conversación, no para el archivo.
- **Seleccionar:** pedí al usuario las opciones si no las generaste vos en el mismo hilo. Seguí la guía de preguntas y el marco de decisión del prompt tal cual está escrito. Regla no negociable heredada del prompt: **nunca elijas por el usuario** — guialo con preguntas y trade-offs, y esperá su decisión explícita.
- **Revisar:** pedí el contenido actual de esa caja si no está ya en el archivo LPD o en la conversación. Seguí los criterios de revisión del prompt (adherencia al formato, claridad, supuestos riesgosos, etc.). Regla no negociable heredada del prompt: **no reescribas el trabajo del usuario** — dale orientación específica para que lo mejore él mismo.

### Redactar el summary conciso

Al guardar en el archivo, condensá el resultado final acordado con el usuario en 2-6 líneas o bullets, en el formato propio de esa caja (el mismo formato requerido que usa el prompt de Generación — ej. el formato `[Nuestro servicio/producto] fue diseñado para...` para la Caja 1, o `[Quién][Hace Qué][En Qué Medida]` para la Caja 2). No incluyas niveles de confianza, listas de supuestos, ni investigación pendiente — eso quedó resuelto (o discutido) durante la conversación.

Ejemplo de summary para Caja 1 (formato objetivo en el archivo):

```markdown
## 1. Enunciado del Problema de Negocio (Business Problem Statement)
Nuestra app de gestión de gastos fue diseñada para que los usuarios registren gastos en
menos de 10 segundos. Hemos observado, a través del abandono en la pantalla de carga rápida
(60% no completa el registro), que los usuarios no están logrando ese objetivo, lo cual está
generando bajo uso recurrente de la app. ¿Cómo podríamos mejorar el flujo de carga rápida
para que los usuarios tengan más éxito registrando gastos, según lo determinado por una
reducción del abandono a menos del 20%?
```
