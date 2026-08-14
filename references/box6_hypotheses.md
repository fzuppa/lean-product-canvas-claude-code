# Prompts Completos de IA por Caja del Canvas
## Descubrimiento de Producto para Equipos Ágiles

Este documento organiza todos los prompts de IA (Generación, Selección y Revisión) por caja del Lean Product Canvas para fácil referencia.

---

## 🎯 Principio Central

**Los outputs de IA son suposiciones que deben ser validadas, no hechos que deben ser aceptados.**

Usa estos prompts para acelerar tu trabajo de descubrimiento, pero siempre trata el contenido generado por IA como suposiciones que requieren validación con evidencia real.

---

## Cómo Usar Este Documento

**Tres tipos de prompts para cada caja del Canvas:**

1. **PROMPTS DE GENERACIÓN** (Opcional)
   - Usar cuando: Necesitas ideas, estás atascado o quieres alternativas
   - La IA hace: Genera múltiples opciones
   - Tú haces: Evalúas y tratas como suposiciones

2. **PROMPTS DE SELECCIÓN** (Después de Generación)
   - Usar cuando: La IA te dio demasiadas opciones
   - La IA hace: Te hace preguntas sobre las opciones
   - Tú haces: Eliges UN foco + organizas el backlog

3. **PROMPTS DE REVISIÓN** (Recomendado)
   - Usar cuando: Después de haber completado el trabajo manualmente
   - La IA hace: Critica formato, claridad, identifica suposiciones
   - Tú haces: Revisas tu propio trabajo

---

# CAJA 6: Hipótesis

## Formato Requerido

```
"Creemos que [nuestro resultado de negocio] puede ser logrado si [estos usuarios] pueden
lograr [este objetivo o resultado] con [esta feature]."
```

**Nota:** Cada hipótesis debe enfocarse en UNA feature solamente.

---

## PROMPT DE GENERACIÓN: Hipótesis

**Cuándo usar:** Escribir hipótesis testeables, identificar suposiciones embebidas

```
Estoy escribiendo hipótesis (Caja 6) para el Lean Product Canvas usando nuestro formato específico.

El formato de hipótesis es:
"Creemos que [nuestro business outcome] puede ser logrado si [estos usuarios] pueden
lograr [este objetivo o resultado] con [esta feature]."

Aquí está mi borrador de hipótesis:
[PEGA TU BORRADOR DE HIPÓTESIS]

Por favor:
1. Critica esta hipótesis - ¿sigue el formato? ¿Es testeable? ¿Es suficientemente específica?
2. Identifica TODAS las suposiciones embebidas (sobre usuarios, valor, factibilidad, modelo de negocio)
3. Para cada suposición, califica el riesgo si estamos equivocados (alto/medio/bajo)
4. Sugiere qué suposición es la más riesgosa para testear primero
5. Genera 2 declaraciones de hipótesis alternativas usando el mismo formato pero enfocándose
   en diferentes suposiciones

Sé crítico y específico. Cada hipótesis debe enfocarse en UNA feature solamente.
```

**Validación Requerida:** Diseña experimentos para testear tus suposiciones más riesgosas. Mejores declaraciones de hipótesis no las hacen verdaderas.

---

## PROMPT DE SELECCIÓN: Hipótesis

**Cuándo usar:** Después de escribir múltiples declaraciones de hipótesis

```
He escrito múltiples hipótesis y necesito ayuda para seleccionar cuál testear primero.
Aquí están mis opciones:

[PEGA TUS DECLARACIONES DE HIPÓTESIS]

Necesito elegir UNA hipótesis para testear primero y organizar las otras como backlog.
Por favor ayúdame a pensar esta decisión. NO elijas por mí.

Guíame a través de esta decisión mediante:

1. IDENTIFICACIÓN DE SUPOSICIONES
   Para cada hipótesis, pregunta:
   - ¿Cuáles son las 3-4 suposiciones más grandes embebidas en esta hipótesis?
   - ¿Qué suposiciones son sobre VALOR (¿los usuarios querrán esto)?
   - ¿Qué suposiciones son sobre USABILIDAD (¿los usuarios pueden usar esto)?
   - ¿Qué suposiciones son sobre FACTIBILIDAD (¿podemos construir esto)?
   - ¿Qué suposiciones son sobre VIABILIDAD (¿esto funcionará para nuestro negocio)?

2. EVALUACIÓN DE RIESGO
   Para cada hipótesis, pregunta:
   - Si esta hipótesis está EQUIVOCADA, ¿qué sucede?
   - ¿Qué hipótesis, si está equivocada, desperdiciaría más tiempo/dinero?
   - ¿Qué suposiciones, si están equivocadas, invalidarían todo el enfoque?

3. TESTABILIDAD
   Para cada hipótesis, pregunta:
   - ¿Qué tan fácilmente podemos testear esta hipótesis?
   - ¿Podemos testear las suposiciones más riesgosas sin construir la feature completa?
   - ¿Qué evidencia probaría que esto está equivocado vs. correcto?
   - ¿Cuánto tiempo tomaría reunir esa evidencia?

4. VALOR DE APRENDIZAJE
   Para cada hipótesis, pregunta:
   - ¿Qué aprenderíamos al testear esto?
   - ¿Esta hipótesis, si se valida, desbloquea otras hipótesis?
   - ¿Es esta hipótesis fundacional o dependiente de otras?

5. MARCO DE DECISIÓN
   Presenta esto como una tabla comparando hipótesis a través de:
   - Tipo de suposición más riesgosa (Valor/Usabilidad/Factibilidad/Viabilidad)
   - Impacto si está equivocada (Alto/Medio/Bajo)
   - Facilidad de testeo (Fácil/Medio/Difícil)
   - Valor de aprendizaje (Alto/Medio/Bajo)
   - Dependencias (Fundacional/Dependiente)

Luego pregúntame: "Basado en este análisis, ¿qué hipótesis testearás primero y
por qué? Recuerda: testea riesgos de valor y usabilidad antes que riesgos de factibilidad."

Después de que responda, ayúdame a organizar las otras como una secuencia de testeo:
- Testear 1ro (tu elección)
- Testear 2do (siguiente prioridad)
- Testear 3ro (después de eso)
- Parking lot (despriorizado)
```

---

## PROMPT DE REVISIÓN: Hipótesis

**Cuándo usar:** Después de haber escrito tus declaraciones de hipótesis

```
He completado la Caja 6 (Hipótesis) del Lean Product Canvas. Por favor revisa mi
trabajo y proporciona retroalimentación constructiva.

Aquí están mis hipótesis:
[PEGA TUS DECLARACIONES DE HIPÓTESIS]

El formato requerido para cada hipótesis es:
"Creemos que [nuestro resultado de negocio] puede ser logrado si [estos usuarios] pueden
lograr [este objetivo o resultado] con [esta feature]."

Nota: Cada hipótesis debe enfocarse en UNA feature solamente.

Por favor proporciona retroalimentación sobre:

1. ADHERENCIA AL FORMATO
   - ¿Cada hipótesis sigue el formato requerido?
   - ¿Cada hipótesis se enfoca en solo UNA feature?
   - ¿Están presentes los cuatro componentes (resultado de negocio, usuarios, objetivo de usuario, feature)?
   - ¿Los componentes se mapean a cajas específicas? (resultado de la Caja 2, usuarios de la Caja 3,
     objetivo de usuario de la Caja 4, feature de la Caja 5)

2. CLARIDAD
   - ¿El resultado de negocio es específico y medible?
   - ¿Los usuarios están claramente identificados?
   - ¿El objetivo/resultado de usuario está claro?
   - ¿La feature está descrita concretamente?
   - ¿Es testeable esta hipótesis?
   - ¿Sabríamos si esta hipótesis es verdadera o falsa?

3. SUPOSICIONES RIESGOSAS
   - Identifica 2-3 de las suposiciones más riesgosas en estas hipótesis
   - Para cada suposición, categoriza: valor, usabilidad, factibilidad, viabilidad de negocio
   - ¿Qué suposición, si está equivocada, invalidaría toda la hipótesis?
   - Rankea suposiciones por: nivel de riesgo y facilidad de testeo

NO reescribas mis hipótesis. En su lugar, proporciona orientación específica sobre cómo puedo
mejorarlas yo mismo.
```
