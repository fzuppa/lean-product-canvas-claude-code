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

# CAJA 8: La Menor Cantidad de Trabajo para Aprenderlo

## Propósito

Especificar el experimento para reducir el riesgo de tu hipótesis. Enfócate en qué podrías aprender en 1 día / 1 semana / 1 mes.

---

## PROMPT DE GENERACIÓN: Experimentos (MVPs)

**Cuándo usar:** Diseñar experimentos, planificar MVPs

```
Necesito testear esta suposición: [DECLARA TU SUPOSICIÓN DE LA CAJA 7]

Contexto:
- Mi hipótesis (Caja 6): [DECLARA HIPÓTESIS]
- Lo que necesito aprender (Caja 7): [DECLARA OBJETIVO DE APRENDIZAJE]

Ayúdame a diseñar un experimento mediante:
1. Sugerir 3 enfoques de experimento diferentes (barato/rápido/métodos diferentes)
2. Para cada enfoque:
   - ¿Qué haría exactamente?
   - ¿Con quién lo haría (qué usuarios)?
   - ¿Qué mediría/observaría?
   - ¿Qué validaría la suposición?
   - ¿Qué invalidaría la suposición?
   - Línea de tiempo (1 día / 1 semana / 1 mes)
3. Para cada enfoque, identificar posibles sesgos o amenazas a la validez
4. Rankear enfoques por: velocidad al insight, costo, y calidad del aprendizaje

Enfócate en la MENOR cantidad de trabajo necesaria para aprender. ¿Cuál es el test mínimo viable?
```

**Validación Requerida:** CORRE EL EXPERIMENTO. Recolecta datos reales de usuarios reales. No racionalices resultados después del hecho.

---

## PROMPT DE SELECCIÓN: Experimentos

**Cuándo usar:** Después de que el Prompt de Generación sugiere múltiples enfoques de experimento

```
Necesito testear esta suposición: [DECLARA TU SUPOSICIÓN DE LA CAJA 7]

La IA ha sugerido múltiples enfoques de experimento:
[PEGA OPCIONES DE EXPERIMENTO]

Necesito elegir UN enfoque de experimento para correr primero. Por favor ayúdame a pensar
esta decisión. NO elijas por mí.

Guíame a través de esta decisión mediante:

1. VERIFICACIÓN DE VALIDEZ
   Para cada experimento, pregunta:
   - ¿Esto realmente testea la suposición de la Caja 7?
   - ¿Qué podríamos aprender de este experimento?
   - ¿Qué NO aprenderemos?
   - ¿Podría esto darnos resultados falsos positivos o falsos negativos?

2. REQUERIMIENTOS DE RECURSOS
   Para cada experimento, pregunta:
   - ¿Cuánto tiempo tomará esto?
   - ¿Qué acceso a usuarios/clientes necesitamos?
   - ¿Qué herramientas o materiales necesitamos?
   - ¿Tenemos estos recursos disponibles ahora?

3. VELOCIDAD AL INSIGHT
   Para cada experimento, pregunta:
   - ¿Qué tan rápido obtendremos resultados?
   - ¿Podemos correr esto en 1 día / 1 semana / 1 mes?
   - ¿Cuántos participantes necesitamos?
   - ¿Cuánto tiempo para reclutar participantes?

4. POTENCIAL DE SESGO
   Para cada experimento, pregunta:
   - ¿Qué sesgos podrían afectar los resultados?
   - ¿Estamos en riesgo de sesgo de confirmación?
   - ¿Podrían los participantes decirnos lo que piensan que queremos escuchar?
   - ¿Cómo podemos diseñar para retroalimentación honesta?

5. MARCO DE DECISIÓN
   Presenta esto como una tabla comparando experimentos a través de:
   - Testea directamente la suposición (Sí/Parcial/No)
   - Tiempo para completar (Días/Semanas/Meses)
   - Requerimientos de recursos (Bajo/Medio/Alto)
   - Riesgo de sesgo (Bajo/Medio/Alto)
   - Calidad del insight (Alta/Media/Baja)

Luego pregúntame: "Basado en este análisis, ¿qué experimento correrás primero y por qué?
Considera: el mejor experimento es el más rápido que te da resultados válidos."

Después de que responda, sugiere cómo refinar el experimento elegido para reducir sesgo y
aumentar velocidad.
```

---

## PROMPT DE REVISIÓN: Experimentos (Caja 8)

**Cuándo usar:** Después de haber diseñado tu experimento

```
He completado la Caja 8 (La Menor Cantidad de Trabajo para Aprenderlo) del Lean Product Canvas.
Por favor revisa mi trabajo y proporciona retroalimentación constructiva.

Aquí está mi diseño de experimento:
[PEGA TU DESCRIPCIÓN DE EXPERIMENTO]

Contexto de la Caja 7 - Lo que necesito aprender:
[PEGA TU CONTENIDO DE LA CAJA 7]

Recuerda: La Caja 8 debe especificar el experimento para reducir el riesgo de la hipótesis. Enfócate en
la MENOR cantidad de trabajo necesaria para aprender. Piensa: ¿qué podrías aprender en 1 día /
1 semana / 1 mes?

Por favor proporciona retroalimentación sobre:

1. ADHERENCIA AL FORMATO
   - ¿Es esto un experimento (no una construcción de feature completa)?
   - ¿Está claramente descrito con pasos concretos?
   - ¿Incluye lo que medirás/observarás?
   - ¿Hay una línea de tiempo (1 día/semana/mes)?

2. CLARIDAD
   - ¿Este experimento realmente testea la suposición de la Caja 7?
   - ¿Qué harás exactamente?
   - ¿Con quién lo harás (qué usuarios)?
   - ¿Qué observarás/medirás?
   - ¿Qué resultado validaría la suposición?
   - ¿Qué resultado invalidaría la suposición?
   - ¿Es esto realmente el MÍNIMO necesario para aprender, o podría ser más simple?

3. SUPOSICIONES RIESGOSAS
   - Identifica 2-3 suposiciones embebidas en el diseño del experimento mismo
   - ¿Qué estamos asumiendo sobre la disposición del usuario a participar?
   - ¿Qué sesgos podrían afectar los resultados?
   - ¿Qué podría darnos resultados falsos positivos o falsos negativos?
   - ¿Estamos en riesgo de confirmar lo que queremos creer?

NO reescribas mi experimento. En su lugar, proporciona orientación específica sobre cómo puedo
mejorarlo yo mismo.
```
