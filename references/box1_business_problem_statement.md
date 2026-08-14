# Prompts Completos de IA por Caja del Canvas
## Descubrimiento de Producto para Equipos Ágiles

Este documento organiza todos los prompts de IA (Generación, Selección y Revisión) por caja del Lean Product Canvas para fácil referencia.

---

## 🎯 Principio Fundamental

**Los resultados de IA son suposiciones que deben validarse, no hechos a aceptar.**

Usa estos prompts para acelerar tu trabajo de descubrimiento, pero siempre trata el contenido generado por IA como suposiciones que requieren validación con evidencia real.

---

## Cómo Usar Este Documento

**Tres tipos de prompts para cada caja del Canvas:**

1. **PROMPTS DE GENERACIÓN** (Opcional)
   - Usar cuando: Necesitas ideas, estás estancado, o quieres alternativas
   - La IA hace: Genera múltiples opciones
   - Tú haces: Evalúa y trata como suposiciones

2. **PROMPTS DE SELECCIÓN** (Después de Generación)
   - Usar cuando: La IA te dio demasiadas opciones
   - La IA hace: Te hace preguntas sobre las opciones
   - Tú haces: Eliges UNA para enfocarte + organizas el backlog

3. **PROMPTS DE REVISIÓN** (Recomendado)
   - Usar cuando: Después de haber completado el trabajo manualmente
   - La IA hace: Critica formato, claridad, identifica suposiciones
   - Tú haces: Revisas tu propio trabajo

---

# CAJA 1: Declaración del Problema de Negocio

## Formato Requerido

```
[Nuestro servicio/producto] fue diseñado para lograr [estos objetivos]. Hemos observado
[de esta manera] que el producto/servicio no está cumpliendo estos objetivos, lo cual está
causando [este efecto adverso/problema] a nuestro negocio. ¿Cómo podríamos mejorar el
servicio/producto para que nuestros clientes tengan más éxito según lo determinado por
[estos cambios medibles en su comportamiento]?
```

---

## PROMPT DE GENERACIÓN: Declaración del Problema de Negocio

**Cuándo usar:** Reformular soluciones como problemas, explorar declaraciones de problema alternativas

```
Estoy trabajando en definir un problema de negocio usando el Lean Product Canvas.
Esta es mi situación:
[DESCRIBE TU SITUACIÓN - ej., "Somos una empresa de aprendizaje en línea. Las personas
toman una clase y no vuelven. Nuestro CEO quiere implementar códigos de descuento."]

Ayúdame a crear Declaraciones de Problema de Negocio usando este formato EXACTO:

"[Nuestro servicio/producto] fue diseñado para lograr [estos objetivos]. Hemos observado
[de esta manera] que el producto/servicio no está cumpliendo estos objetivos, lo cual está
causando [este efecto adverso/problema] a nuestro negocio. ¿Cómo podríamos mejorar el
servicio/producto para que nuestros clientes tengan más éxito según lo determinado por
[estos cambios medibles en su comportamiento]?"

Por favor:
1. Genera 2-3 declaraciones de problema diferentes usando este formato exacto
2. Para cada declaración, identifica qué suposiciones se están haciendo
3. Nota qué evidencia validaría que este es el problema real
4. Evita saltar a soluciones - mantén el enfoque en el problema

Usa el formato exacto de arriba. Necesito declaraciones de problema, no soluciones.
```

**Validación Requerida:** Recopila evidencia (datos, aportes de stakeholders, o investigación) que pruebe qué formulación del problema refleja la realidad.

---

## PROMPT DE SELECCIÓN: Declaración del Problema de Negocio

**Cuándo usar:** Después de que el Prompt de Generación te dé 2-3 opciones de declaración de problema

```
He generado múltiples opciones de declaración de problema de negocio y necesito ayuda
para seleccionar en cuál enfocarme primero. Estas son mis opciones:

[PEGA TUS 2-3 OPCIONES DE DECLARACIÓN DE PROBLEMA]

Necesito elegir UNA en la cual enfocarme y organizar las demás como un backlog. Por favor,
ayúdame a pensar en esta decisión haciéndome preguntas y mostrando trade-offs.
NO elijas por mí.

Guíame a través de esta decisión mediante:

1. VERIFICACIÓN DE EVIDENCIA
   Para cada opción, pregunta:
   - ¿Qué evidencia tengo actualmente que respalde que este es el problema real?
   - ¿Qué necesitaría validar para confirmar esta formulación del problema?
   - ¿Qué opción tiene la mayor evidencia existente?

2. ANÁLISIS DE IMPACTO
   Para cada opción, pregunta:
   - Si resolvemos este problema, ¿qué impacto de negocio veríamos?
   - ¿Qué problema, si se resuelve, crea el mayor valor?
   - ¿Qué problema es más urgente vs. más importante?

3. VERIFICACIÓN DE VIABILIDAD
   Para cada opción, pregunta:
   - ¿Tenemos la capacidad de abordar este problema?
   - ¿Qué está bajo nuestro control vs. fuera de nuestro control?
   - ¿Qué problema podemos impactar de manera realista?

4. PRUEBA DE ENFOQUE
   Ayúdame a considerar:
   - ¿Qué problema, si me enfoco en él exclusivamente durante 3 meses, importaría más?
   - ¿Qué problemas podrían ser síntomas de otro problema?
   - ¿Qué problema es más fundamental?

5. MARCO DE DECISIÓN
   Presenta esto como una tabla comparando opciones a través de:
   - Evidencia existente (Alta/Media/Baja)
   - Impacto potencial en el negocio (Alto/Medio/Bajo)
   - Nuestra capacidad para abordarlo (Alta/Media/Baja)
   - Importancia estratégica (Alta/Media/Baja)

Luego pregúntame A MÍ: "Basado en este análisis, ¿en qué declaración de problema te
enfocarás primero y por qué?"

Después de que responda, ayúdame a organizar las otras como un backlog con notas sobre
cuándo revisar cada una.
```

---

## PROMPT DE REVISIÓN: Declaración del Problema de Negocio

**Cuándo usar:** Después de haber escrito tu declaración de problema de negocio

```
He completado la Caja 1 (Declaración del Problema de Negocio) del Lean Product Canvas.
Por favor, revisa mi trabajo y proporciona retroalimentación constructiva.

Esta es mi declaración de problema de negocio:
[PEGA TU DECLARACIÓN DE PROBLEMA COMPLETA]

El formato requerido es:
"[Nuestro servicio/producto] fue diseñado para lograr [estos objetivos]. Hemos observado
[de esta manera] que el producto/servicio no está cumpliendo estos objetivos, lo cual está
causando [este efecto adverso/problema] a nuestro negocio. ¿Cómo podríamos mejorar el
servicio/producto para que nuestros clientes tengan más éxito según lo determinado por
[estos cambios medibles en su comportamiento]?"

Por favor, proporciona retroalimentación sobre:

1. ADHERENCIA AL FORMATO
   - ¿Mi declaración sigue el formato requerido?
   - ¿Qué secciones faltan o están incompletas?
   - ¿Están presentes todos los elementos de la plantilla?

2. CLARIDAD
   - ¿El problema está claramente articulado?
   - ¿Los objetivos son específicos y comprensibles?
   - ¿Las observaciones son concretas o vagas?
   - ¿El efecto adverso es medible/tangible?
   - ¿Los cambios de comportamiento deseados son específicos?

3. SUPOSICIONES RIESGOSAS
   - Identifica 2-3 suposiciones incorporadas en esta declaración de problema
   - Para cada suposición, nota por qué es riesgosa si está equivocada
   - Sugiere qué evidencia probaría cada suposición

NO reescribas mi declaración de problema. En su lugar, proporciona orientación específica
sobre cómo puedo mejorarla yo mismo.
```
