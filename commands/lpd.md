---
description: Crea (o retoma) el Lean Product Canvas de una oportunidad y arranca completando la Caja 1
argument-hint: <nombre-oportunidad>
---

Quiero trabajar el Lean Product Canvas de la oportunidad "$ARGUMENTS" usando el skill `lean-product-canvas`.

- Si el skill aparece en tu lista de skills invocables, usalo con `Skill({skill: "lean-product-canvas", args: "$ARGUMENTS"})`, pidiendo explícitamente: crear o retomar el archivo LPD de esta oportunidad y arrancar por la Caja 1.
- Si no aparece invocable pero está instalado como carpeta, buscalo (`find . -iname "SKILL.md" -path "*lean-product-canvas*"`, tanto a nivel proyecto como en `~/.claude/skills` o `~/.agents/skills`), leé ese `SKILL.md` y seguí vos mismo sus instrucciones al pie de la letra.

En cualquiera de los dos casos, el flujo a ejecutar es el que describe el skill:

1. **Ubicar la carpeta de boards** del proyecto actual: buscá archivos `LPD *.md` ya existentes y usá esa carpeta. Si no encontrás ninguno, preguntá dónde guardar los LPD de este proyecto (sugerí `Lean Product Canvas Boards/` como default).
2. **Crear el archivo si no existe.** Si `LPD $ARGUMENTS.md` no existe en esa carpeta, crealo con el scaffold completo de las 8 cajas en `_Pendiente_` (formato exacto del `SKILL.md`).
3. **Si ya existe:**
   - Si la Caja 1 ya tiene contenido (no está en `_Pendiente_`), mostralo y preguntá si se quiere revisarla (modo Revisar) o pasar directo a la próxima caja pendiente — no regenerarla en silencio.
   - Si la Caja 1 sigue en `_Pendiente_`, continuar con el paso 4.
4. **Arrancar la Caja 1.** Antes de generar contenido, preguntar por el alcance de la investigación (usar información relacionada del proyecto vs. ir directo a la Caja 1), tal como pide el flujo general del skill. Con eso resuelto, ejecutar el **PROMPT DE GENERACIÓN** de `box1_business_problem_statement.md` resolviendo sus placeholders con lo que cuente el usuario.

Respetá el resto de las reglas no negociables del skill: nunca sobrescribir en silencio, ofrecer el summary conciso antes de guardar, y pedir confirmación explícita para reemplazar contenido existente.
