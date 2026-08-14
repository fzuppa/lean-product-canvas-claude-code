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

# CAJA 5: Soluciones/Features

## Propósito

Contener ideas de solución, típicamente especificadas como titulares o ideas simples de lluvia de ideas.

---

## PROMPT DE GENERACIÓN: Soluciones/Features

**Cuándo usar:** Lluvia de ideas de features, evaluación de conceptos de solución

```
Basado en mi Lean Product Canvas hasta ahora:
- Problema de Negocio (Caja 1): [RESUMEN BREVE]
- Usuarios (Caja 3): [PERSONA BREVE]
- Resultados de Usuario/JTBD (Caja 4): [QUÉ ESTÁN INTENTANDO HACER]

Genera 10 ideas de features que podrían abordar esta necesidad. Para cada una:
1. Descripción breve de la feature
2. Qué resultado de usuario aborda
3. Suposiciones clave que hace esta feature
4. Qué podría hacer fallar esta feature

Incluye ideas tanto obvias como creativas.
```

**Validación Requerida:** Testea conceptos de features con clientes antes de construir. No construyas features solo porque la IA las sugirió.

---

## PROMPT DE SELECCIÓN: Soluciones/Features

**Cuándo usar:** Después de que el Prompt de Generación te da 10+ ideas de features

```
He generado múltiples ideas de features y necesito ayuda para seleccionar cuál(es)
prototipar/testear primero. Aquí están mis opciones:

[PEGA TUS 10+ IDEAS DE FEATURES]

Contexto de mi Canvas:
- Usuarios (Caja 3): [PERSONA BREVE]
- Resultados de Usuario (Caja 4): [RESULTADOS CLAVE DE USUARIO]

Necesito elegir 1-3 features en las que enfocarme y organizar las otras como backlog.
Por favor ayúdame a pensar esta decisión. NO elijas por mí.

Guíame a través de esta decisión mediante:

1. ALINEACIÓN CON RESULTADOS DE USUARIO
   Para cada feature, pregunta:
   - ¿Qué resultado de usuario de la Caja 4 aborda esto?
   - ¿Qué tan directamente ayuda a los usuarios a lograr su objetivo?
   - ¿Hay features resolviendo problemas que los usuarios no tienen?

2. RIESGO DE SUPOSICIONES
   Para cada feature, pregunta:
   - ¿Cuál es la suposición más riesgosa que hace esta feature?
   - ¿Qué debe ser verdad sobre los usuarios para que esto funcione?
   - ¿Qué debe ser verdad sobre la tecnología/modelo de negocio?
   - ¿Qué features hacen los mayores saltos en suposiciones?

3. TESTABILIDAD
   Para cada feature, pregunta:
   - ¿Qué tan fácilmente podríamos testear esto con un MVP/prototipo?
   - ¿Cuál es la forma más barata de validar esta idea?
   - ¿Qué features podríamos testear en 1 semana vs. 1 mes?

4. VALOR VS. COMPLEJIDAD
   Para cada feature, estima:
   - Valor potencial para usuarios (Alto/Medio/Bajo)
   - Valor potencial para el negocio (Alto/Medio/Bajo)
   - Complejidad para construir (Alta/Media/Baja)
   - Complejidad para testear (Alta/Media/Baja)

5. MARCO DE DECISIÓN
   Presenta esto como una matriz 2x2:
   - Eje X: Riesgo/Incertidumbre (Bajo a Alto)
   - Eje Y: Valor Potencial (Bajo a Alto)
   Ubica cada feature e identifica cuáles están en el cuadrante "Alto Valor, Alto Riesgo"
   (testea estas primero)

Luego pregúntame: "Basado en este análisis, ¿cuáles 1-3 features testearás primero
y por qué? Recuerda: testea primero las ideas de alto valor y alto riesgo."

Después de que responda, ayúdame a organizar las otras como backlog categorizado por:
- Alta prioridad (testear a continuación)
- Prioridad media (testear más tarde)
- Baja prioridad / parking lot (quizás nunca)
```

---

## PROMPT DE REVISIÓN: Soluciones/features

**Cuándo usar:** Después de haber hecho lluvia de ideas de soluciones

```
He completado la Caja 5 (Soluciones/features) del Lean Product Canvas. Por favor
revisa mi trabajo y proporciona retroalimentación constructiva.

Aquí están mis ideas de solución:
[PEGA TU LISTA DE featureS]

Contexto: Esta caja contiene ideas de solución, típicamente como titulares o ideas
simples de lluvia de ideas.

Por favor proporciona retroalimentación sobre:

1. ADHERENCIA AL FORMATO
   - ¿Están expresadas como titulares o ideas simples?
   - ¿Están en el nivel correcto de detalle (no muy específico, no muy vago)?
   - ¿Son soluciones/features, no problemas o resultados?

2. CLARIDAD
   - ¿Puede alguien entender qué es cada solución desde el titular?
   - ¿Son distintas entre sí?
   - ¿Se conectan con los resultados de usuario en la Caja 4?
   - ¿Abordan el problema de negocio en la Caja 1?
   - ¿Hay suficiente variedad en los enfoques?

3. SUPOSICIONES RIESGOSAS
   - Identifica 2-3 suposiciones a través de estas soluciones
   - Para cada solución, ¿qué debe ser verdad para que funcione?
   - ¿Qué soluciones hacen los mayores saltos en suposiciones?
   - ¿Qué comportamientos de usuario estamos asumiendo que ocurrirán?

NO reescribas mis soluciones. En su lugar, proporciona orientación específica sobre cómo puedo
mejorarlas yo mismo.
```
