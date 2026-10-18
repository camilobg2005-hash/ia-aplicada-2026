# P03 — Riesgos del asistente de presupuestos

## Objetivo
Identificar riesgos reales del proyecto y controles

## Modelo y configuración
- Modelo: ChatGPT (GPT-6).
- Temperatura: por defecto (no controlable).
- Fecha de ejecución: 2026-10-18.
- Procedencia: Prompt nuevo redactado y ejecutado en la sesión.

## Prompt (versión v1)
```text
Para el proyecto de asistencia con IA en presupuestos de obra, identifica cinco riesgos prácticos y una medida de control para cada uno. Usa exclusivamente estos hechos: se parte de planos, catálogos de conceptos, cotizaciones y hojas de cálculo; los cálculos se revisan con fórmulas; el responsable humano valida precios y alcances. No agregues cifras ni nombres de normas. Responde en tabla.
```

## Resultado obtenido
| Riesgo | Medida de control |
|---|---|
| Precios desactualizados | Comprobar con cotizaciones vigentes. |
| Cálculos equivocados | Recalcular con fórmulas. |
| Alcance mal interpretado | Comparar con plano y catálogo original. |
| Exposición de datos | Anonimizar y solicitar autorización. |
| Cambios sin seguimiento | Guardar versiones con revisión humana. |

## Verificación
| Afirmación verificable | Fuente primaria | Clasificación |
|---|---|---|
| Las cotizaciones vigentes son necesarias | https://github.com/camilobg2005-hash/ia-aplicada-2026/blob/main/proyecto/ficha_inicial.md | Correcta |
| Se revisan cálculos con fórmulas | https://github.com/camilobg2005-hash/ia-aplicada-2026/blob/main/proyecto/ficha_inicial.md | Correcta |
| Un responsable humano valida precios y alcances | https://github.com/camilobg2005-hash/ia-aplicada-2026/blob/main/proyecto/ficha_inicial.md | Correcta |

Tasa de error de esta respuesta: **0.0 %**.

## Evaluación
- Qué funcionó: Se evitó inventar estadísticas.
- Qué falló: No hay medición empírica de riesgos.
- Qué cambiaré en la siguiente versión: Añadir registro de controles aplicados.

## Historial de versiones
| Versión | Fecha | Cambio realizado | Resultado del cambio |
|---|---|---|---|
| v1 | 2026-10-18 | Versión inicial | Respuesta y verificación documentadas |

## Datos usados
Cumplimiento preventivo de la sección 5: **sí, sujeto a cotejar la política íntegra**. Se usaron datos públicos y supuestos, sin documentos confidenciales o datos personales.
