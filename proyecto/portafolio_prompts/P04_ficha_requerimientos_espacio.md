# P04 — Ficha preliminar de requerimientos de espacio

## Objetivo
Convertir una descripción libre de cliente en una ficha uniforme que pueda alimentar etapas posteriores del asistente de presupuestos, sin completar datos que no fueron proporcionados.

## Versión adoptada
La versión adoptada fue la **iteración 3: rol + contexto + formato**.

## Resultado
- Línea base: 10/18.
- Iteración adoptada: 18/18.
- Iteración 4 con ejemplo: 18/18.
- Iteración 5 con análisis previo: 15/18 por romper el formato exclusivo de tabla.
- Prueba de robustez: 6/6.

## Prompt

```text
Eres arquitecto junior encargado de levantar requerimientos preliminares. Tu lector es {ROL_LECTOR}.

Contexto: {CONTEXTO_PROYECTO}. La ficha debe cubrir uso, superficie, ventilación, iluminación y normativa aplicable. Esta etapa es únicamente de levantamiento preliminar: no se realizan cálculos normativos ni proyecto ejecutivo y cualquier dato no indicado por el cliente debe tratarse como pendiente de verificación.

Responde únicamente con esta tabla en Markdown, sin texto adicional:

| Campo | Requerimiento |
|---|---|
| Uso | |
| Superficie | |
| Ventilación | |
| Iluminación | |
| Normativa aplicable | |
| Información faltante | |

Si un campo no puede determinarse a partir del texto, escribe `{MARCADOR_FALTANTE}`. Si hay dos datos que se contradicen, escribe `CONTRADICTORIO` y conserva ambos valores para que puedan verificarse. No agregues medidas, porcentajes, normas ni condiciones que el cliente no haya indicado.

Texto del cliente:
{ENTRADA}
```

## Evaluación
La mejora decisiva apareció al fijar una estructura de salida exacta y una regla explícita para datos faltantes o contradictorios. El ejemplo few-shot no produjo mejora adicional en la muestra probada.

## Limitaciones
La plantilla no sustituye levantamiento, medición ni revisión normativa. Solo estructura la información disponible y marca faltantes.

## Historial de versiones
| Versión | Fecha | Cambio | Resultado |
|---|---|---|---|
| v1 | 2026-10-25 | Rol + contexto + formato y reglas de incertidumbre | 18/18; robustez 6/6 |
