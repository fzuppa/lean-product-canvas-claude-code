# Prompts de IA Completos por Caja del Canvas
## Descubrimiento de Producto para Equipos Ágiles

Este documento organiza todos los prompts de IA (Generación, Selección y Revisión) por caja del Lean Product Canvas para fácil referencia.

---

## 🎯 Principio Central

**Los resultados de la IA son suposiciones que deben ser validadas, no hechos para ser aceptados.**

Usa estos prompts para acelerar tu trabajo de descubrimiento, pero siempre trata el contenido generado por IA como suposiciones que requieren validación con evidencia real.

---

## Cómo Usar Este Documento

**Tres tipos de prompts para cada caja del Canvas:**

1. **PROMPTS DE GENERACIÓN** (Opcional)
   - Usar cuando: Necesitas ideas, estás atascado, o quieres alternativas
   - La IA: Genera múltiples opciones
   - Tú: Evalúas y tratas como suposiciones

2. **PROMPTS DE SELECCIÓN** (Después de Generación)
   - Usar cuando: La IA te dio demasiadas opciones
   - La IA: Te hace preguntas sobre las opciones
   - Tú: Eliges UNA prioridad + organizas el backlog

3. **PROMPTS DE REVISIÓN** (Recomendado)
   - Usar cuando: Después de haber completado el trabajo manualmente
   - La IA: Critica formato, claridad, identifica suposiciones
   - Tú: Revisas tu propio trabajo

---

# CAJA 2: Business Outcomes

## Definición Clave

**Un business outcome es "un cambio medible en el comportamiento humano que crea valor"**

## Formato Requerido

```
[Quién] [Hace Qué] [En Qué Medida]

Donde:
- Quién = la persona que realiza el comportamiento
- Hace Qué = el comportamiento específico
- En Qué Medida = el cambio medible en cantidad/número
```

---

## PROMPT DE GENERACIÓN: Resultados de Negocio

**Cuándo usar:** Lluvia de ideas de resultados medibles, definición de métricas de éxito

```
Nuestro problema de negocio es: [INSERTA TU DECLARACIÓN DE PROBLEMA DE LA CAJA 1]

Ayúdame a definir business outcomes (Caja 2) usando el formato del Lean Product Canvas.

Recuerda: Un business outcome es "un cambio medible en el comportamiento humano que crea valor."

Genera 5 business outcomes potenciales usando este formato EXACTO:
[Quién] [Hace Qué] [En Qué Medida]

Donde:
- Quién = la persona que realiza el comportamiento
- Hace Qué = el comportamiento específico
- En Qué Medida = el cambio medible en cantidad/número

Para cada resultado:
1. Escríbelo en el formato anterior
2. Identifica qué suposiciones hace
3. Anota qué datos necesitaríamos para medir esto
4. Indica si es un leading indicator o lagging indicator
Ejemplo: "Los nuevos usuarios completan la incorporación 40% más frecuentemente"
(Quién: nuevos usuarios | Hace Qué: completan la incorporación | En Qué Medida: 40% más frecuentemente)
```

**Validación Requerida:** Confirma que realmente puedes medir estas métricas y documenta las líneas base actuales.

---

## PROMPT DE SELECCIÓN: Resultados de Negocio

**Cuándo usar:** Después de que el Prompt de Generación te da 5+ opciones de resultados

```
He generado múltiples opciones de business outcomes y necesito ayuda para seleccionar
en cuál(es) enfocarme primero. Aquí están mis opciones:

[PEGA TUS 5+ OPCIONES DE BUSINESS OUTCOMES]

Necesito elegir 1-3 business outcomes en los que enfocarme y organizar los demás como backlog.
Por favor ayúdame a pensar en esta decisión haciéndome preguntas. NO elijas por mí.

Guíame a través de esta decisión mediante:

1. VERIFICACIÓN DE MEDIBILIDAD
   Para cada resultado, pregunta:
   - ¿Podemos medir esto hoy?
   - Si no, ¿qué tan difícil sería comenzar a medirlo?
   - ¿Tenemos datos de baseline?
   - ¿Cuáles business outcomes son más fáciles de rastrear?

1. LEADING VS. LAGGING
   Para cada business outcome, pregunta:
   - ¿Es este un indicador leading (predice el éxito futuro) o indicador lagging
     (muestra resultados pasados)?
   - ¿Qué tan rápido veríamos movimiento en esta métrica?
   - ¿Cuáles resultados nos dan la retroalimentación más rápida?

3. CONEXIÓN CON EL PROBLEMA
   Para cada resultado, pregunta:
   - ¿Qué tan directamente indica este resultado que hemos resuelto nuestro problema de negocio (Caja 1)?
   - ¿Cuáles business outcomes son más relevantes para nuestro problema específico?
   - ¿Hay algún business outcomes demasiado alejado del problema?

4. ENFOQUE EN EL COMPORTAMIENTO
   Para cada resultado, verifica:
   - ¿Es esto realmente un cambio de comportamiento o solo una métrica?
   - ¿De quién debe cambiar el comportamiento?
   - ¿Está el cambio de comportamiento dentro de nuestra influencia?

5. MARCO DE DECISIÓN
   Presenta esto como una tabla comparando resultados a través de:
   - Actualmente medible (Sí/No)
   - Indicador leading o lagging
   - Vínculo directo con el problema (Alto/Medio/Bajo)
   - Cambio de comportamiento real (Sí/No)
   - Velocidad de retroalimentación (Rápida/Media/Lenta)

Luego pregúntame A MÍ: "Basado en este análisis, ¿en qué 1-3 resultados te enfocarás y por qué?
Considera: necesitas al menos un leading indicator."

Después de que responda, ayúdame a organizar los demás como backlog.
```

---

## PROMPT DE REVISIÓN: Resultados de Negocio

**Cuándo usar:** Después de haber escrito tus business outcomes

```
He completado la Caja 2 (business outcomes) del Lean Product Canvas. Por favor revisa
mi trabajo y proporciona retroalimentación constructiva.

Aquí están mis resultados de negocio:
[PEGA TU LISTA DE RESULTADOS]

El formato requerido para cada resultado es:
[Quién] [Hace Qué] [En Qué Cantidad]

Donde:
- Quién = la persona que realiza el comportamiento
- Hace Qué = el comportamiento específico
- En Qué Cantidad = el cambio medible en cantidad/número

Recuerda: Un business outcome es "un cambio medible en el comportamiento humano que crea valor"

Por favor proporciona retroalimentación sobre:

1. ADHERENCIA AL FORMATO
   - ¿Cada resultado sigue el formato [Quién] [Hace Qué] [En Qué Cantidad]?
   - ¿A cuáles business outcomes les faltan componentes?
   - ¿Los componentes están claramente separados?

2. CLARIDAD
   - ¿Es "Quién" lo suficientemente específico? (no solo "usuarios" sino ¿qué usuarios?)
   - ¿Es "Hace Qué" un comportamiento claro y observable?
   - ¿Es "En Qué Cantidad" medible y realista?
   - ¿Cada business outcome representa un cambio de comportamiento (no solo una característica)?
   - ¿Son estos indicadores leading o lagging?

3. SUPOSICIONES RIESGOSAS
   - Identifica 2-3 suposiciones a través de todos estos resultados
   - Para cada suposición, anota por qué es riesgoso si está equivocada
   - Sugiere qué datos o evidencia probaría cada suposición

NO reescribas mis business outcomes. En su lugar, proporciona orientación específica sobre cómo
puedo mejorarlos yo mismo.
```
