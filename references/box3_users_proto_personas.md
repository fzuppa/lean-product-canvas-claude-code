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

# CAJA 3: Usuarios (Proto-Personas)

## Propósito

Definir las personas a las que el producto debe servir/satisfacer. Pueden ser usuarios, clientes o personas impactadas por el producto. Típicamente expresados como proto-personas.

---

## PROMPT DE GENERACIÓN: Usuarios (Proto-Personas)

**Cuándo usarlo:** Creando personas, identificando usuarios objetivo

```
Estoy creando una persona (Cajas 3-4 del Lean Product Canvas) basada en lo que
sabemos sobre nuestros clientes:
[RESUME TU CONOCIMIENTO DEL CLIENTE - insights de entrevistas, datos, observaciones]

Genera una proto-persona incluyendo:
1. Demografía y antecedentes
2. Objetivos relacionados con nuestro producto
3. Trabajos que están tratando de realizar
4. Puntos de dolor y desafíos

Para cada elemento, indica:
- Nivel de confianza (alto/medio/bajo) basado en la evidencia proporcionada
- Qué está validado vs. qué es asumido
- Qué investigación adicional aumentaría la confianza

Sé honesto sobre qué es especulación vs. qué está basado en evidencia.
```

**Validación Requerida:** Realizar conversaciones con clientes para verificar que la persona refleja personas reales, no supuestos de la IA.

---

## PROMPT DE REVISIÓN: Usuarios (Proto-Personas)

**Cuándo usarlo:** Después de haber creado tus proto-personas

```
He completado la Caja 3 (Usuarios/Proto-Personas) del Lean Product Canvas. Por
favor revisa mi trabajo y proporciona retroalimentación constructiva.

Aquí está mi proto-persona:
[PEGA TU DESCRIPCIÓN DE PERSONA]

Contexto: Las proto-personas definen las personas a las que nuestro producto debe servir/satisfacer. Pueden ser usuarios, clientes o personas impactadas por el producto.

Por favor proporciona retroalimentación sobre:

1. ADHERENCIA AL FORMATO
   - ¿Esta persona incluye elementos clave (demografía, rol, contexto)?
   - ¿Es lo suficientemente concisa para una proto-persona (no excesivamente detallada)?
   - ¿Se enfoca en características relevantes para este producto?

2. CLARIDAD
   - ¿Esta persona es lo suficientemente específica para guiar decisiones?
   - ¿Puedo visualizar una persona real a partir de esta descripción?
   - ¿Las características más relevantes están enfatizadas?
   - ¿Incluye comportamientos, necesidades u objetivos relacionados con nuestro producto?
   - ¿Diferentes miembros del equipo interpretarían esta persona de la misma manera?

3. SUPUESTOS RIESGOSOS
   - Identifica 2-3 supuestos hechos en esta persona
   - Para cada supuesto, nota qué estamos asumiendo sobre esta persona
   - Distingue entre: qué está validado por investigación vs. qué es asumido
   - Sugiere cómo probar si esta persona refleja usuarios reales

NO reescribas mi persona. En su lugar, proporciona orientación específica sobre cómo
puedo mejorarla yo mismo.
```
