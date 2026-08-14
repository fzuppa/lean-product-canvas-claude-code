# Prompts de IA Completos por Caja del Canvas
## Descubrimiento de Producto para Equipos Ágiles

Este documento organiza todos los prompts de IA (Generación, Selección y Revisión) por caja del Lean Product Canvas para fácil referencia.

---

## 🎯 Principio Central

**Los resultados de la IA son supuestos que deben validarse, no hechos que deben aceptarse.**

Usa estos prompts para acelerar tu trabajo de descubrimiento, pero siempre trata el contenido generado por IA como supuestos que requieren validación con evidencia real.

---

## Cómo Usar Este Documento

**Tres tipos de prompts para cada caja del Canvas:**

1. **PROMPTS DE GENERACIÓN** (Opcional)
   - Úsalos cuando: Necesitas ideas, estás atascado o quieres alternativas
   - La IA: Genera múltiples opciones
   - Tú: Evalúas y tratas como supuestos

2. **PROMPTS DE SELECCIÓN** (Después de Generación)
   - Úsalos cuando: La IA te dio demasiadas opciones
   - La IA: Te hace preguntas sobre las opciones
   - Tú: Eliges UNA en la que enfocarte + organizas el backlog

3. **PROMPTS DE REVISIÓN** (Recomendado)
   - Úsalos cuando: Después de haber completado el trabajo manualmente
   - La IA: Critica el formato, claridad, identifica supuestos
   - Tú: Revisas tu propio trabajo

---

# CAJA 4: Resultados y Beneficios del Usuario (JTBD)

## Propósito

Definir los resultados más importantes que los usuarios están tratando de generar. Puede usar el formato [Quién] [Hace Qué] [En Qué Medida] O el marco deJobs To Be Done.

---

## PROMPT DE GENERACIÓN: Outcomes de Usuario (JTBD)

**Cuándo usarlo:** Identificando trabajos por hacer, comprendiendo resultados del cliente

```
Estoy trabajando en comprender los outcomes de usuario para el Lean Product Canvas.

Contexto:
- Cliente objetivo: [DESCRIBE AL CLIENTE DE LA CAJA 3]
- Situación/contexto: [DESCRIBE CUÁNDO/DÓNDE USAN EL PRODUCTO]

Ayúdame a identificar potenciales "jobs to be done" mediante:
1. Generar 5-7 jobs to be done que este cliente podría estar tratando de realizar
2. Para cada jobs to be done, identificar las dimensiones funcional, emocional y social
3. Sugerir qué evidencia indicaría que este es un jobs to be done real vs. un jobs to be done asumido
4. Señalar qué jobs to be done son más probables de ser supuestos vs. necesidades validadas

Incluye jobs to be done que podrían no ser obvios pero podrían ser importantes.
```

**Validación Requerida:** Realizar conversaciones con clientes para verificar que estas son necesidades reales, no supuestos.

---

## PROMPT DE REVISIÓN: Outcomes del Usuario (JTBD)

**Cuándo usarlo:** Después de haber definido los outcomes de usuario o trabajos por hacer

```
He completado la Caja 4 (User Outcomes y Beneficios del Usuario) del Lean Product Canvas. Por favor revisa mi trabajo y proporciona retroalimentación constructiva.

Aquí están mis resultados del usuario/JTBD:
[PEGA TUS USER OUTCOMES]

Contexto: Esta caja define los outcomes más importantes que los usuarios están tratando de generar. Puede usar el formato [Quién] [Hace Qué] [En Qué Medida] O el marco de Jobs to be Done.

Por favor proporciona retroalimentación sobre:

1. ADHERENCIA AL FORMATO
   - Si usas formato de resultado: ¿Sigue [Quién] [Hace Qué] [En Qué Medida]?
   - Si usas JTBD: ¿Está formulado como un job to be done que el usuario necesita hacer?
   - ¿Son estos user outcomes o solo características disfrazadas?

2. CLARIDAD
   - ¿Están escritos desde la perspectiva del USUARIO (no la nuestra)?
   - ¿Representan lo que los usuarios están tratando de lograr?
   - ¿Son lo suficientemente específicos para guiar el diseño de la solución?
   - ¿Se tratan sobre el éxito del usuario, no sobre características del producto?
   - ¿Los usuarios se reconocerían a sí mismos en estas declaraciones?

3. SUPUESTOS RIESGOSOS
   - Identifica 2-3 supuestos sobre lo que les importa a los usuarios
   - Para cada supuesto, nota por qué es riesgoso si los usuarios en realidad no quieren esto
   - Sugiere cómo validar que estas son necesidades reales del usuario
   - Resalta brechas: ¿qué podríamos estar perdiendo sobre las necesidades del usuario?

NO reescribas mis resultados del usuario. En su lugar, proporciona orientación específica sobre cómo puedo mejorarlos yo mismo.
```
