# Lean Product Canvas (skill para Claude Code)

Skill para completar, seleccionar y revisar las 8 cajas del [Lean Product Canvas](https://jeffgothelf.com/blog/the-lean-product-canvas/) conversando con Claude — sin copiar y pegar prompts a mano. Los resultados quedan guardados en un archivo `LPD <Oportunidad>.md` dentro del proyecto.

Está en **español** y es **autocontenido**: toda la lógica y los prompts viven dentro de esta carpeta, no depende de ningún otro archivo del proyecto donde se instale.

## Instalación

### Opción 1: con `npx skills` (recomendado)

Usando la CLI [`skills`](https://github.com/vercel-labs/skills), que instala en el agente que estés usando (Claude Code, Cursor, Codex, y muchos más):

```bash
npx skills add fzuppa/lean-product-canvas-claude-code
```

Para instalarlo a nivel usuario (disponible en todos tus proyectos) en vez de solo este:

```bash
npx skills add fzuppa/lean-product-canvas-claude-code -g
```

### Opción 2: manual

1. Copiá esta carpeta completa (`SKILL.md`, `README.md`, `references/` y `commands/`) a la carpeta de skills de Claude Code:
   - **Para un solo proyecto:** pegala dentro de `.claude/skills/lean-product-canvas/` en la raíz de ese proyecto.
   - **Para todos tus proyectos:** pegala dentro de `~/.claude/skills/lean-product-canvas/` (skills a nivel usuario).
2. **(Opcional) Para tener el comando `/lpd <oportunidad>`:** copiá `commands/lpd.md` a la carpeta de comandos de Claude Code:
   - **Para un solo proyecto:** `.claude/commands/lpd.md` en la raíz de ese proyecto.
   - **Para todos tus proyectos:** `~/.claude/commands/lpd.md`.
   Los comandos son un registro separado de los skills en Claude Code, así que este paso no es automático — hay que copiar el archivo aparte.
3. No hace falta ningún paso adicional de configuración ni build.

## Uso

Simplemente pedile a Claude, en lenguaje natural, algo como:

- "Ayudame a completar un Lean Product Canvas para la oportunidad X"
- "Quiero generar opciones para la caja 1"
- "Tengo varias opciones para la caja 5, ayudame a elegir"
- "Revisá mi caja 3"

O, si instalaste el comando, `/lpd <nombre-oportunidad>` crea (o retoma) el archivo LPD de esa oportunidad y arranca directo por la Caja 1.

El skill va a ir guiándote caja por caja, pidiéndote la información que necesita, mostrándote los resultados generados y pidiendo tu confirmación antes de guardar cada summary en el archivo `LPD <Oportunidad>.md`.

La primera vez que se usa en un proyecto nuevo, te va a preguntar en qué carpeta guardar los archivos LPD. Las veces siguientes reutiliza esa misma carpeta automáticamente (la encuentra buscando archivos `LPD *.md` ya existentes).

## Estructura

```
lean-product-canvas/
├── SKILL.md              # instrucciones que sigue Claude
├── README.md             # este archivo
├── commands/
│   └── lpd.md            # slash command opcional: /lpd <oportunidad>
└── references/
    ├── box1_business_problem_statement.md
    ├── box2_business_outcomes.md
    ├── box3_users_proto_personas.md
    ├── box4_user_outcomes_benefits.md
    ├── box5_solutions_features.md
    ├── box6_hypotheses.md
    ├── box7_most_important_thing_to_learn.md
    └── box8_least_amount_of_work_to_learn_it.md
```

Cada archivo en `references/` contiene los prompts de Generación, Selección (cuando aplica) y Revisión de esa caja del canvas.
