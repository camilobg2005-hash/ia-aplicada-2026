# P02 — Apoyo de IA para presupuestos

## Objetivo
Volver a ejecutar el prompt original de semana 1 y revisar respuesta

## Modelo y configuración
- Modelo: ChatGPT (GPT-6).
- Temperatura: por defecto (no controlable).
- Fecha de ejecución: 2026-10-18.
- Procedencia: Prompt literal del repositorio semana 1; nueva salida ChatGPT.

## Prompt (versión v1)
```text
Actúa como consultor en inteligencia artificial. Trabajo en arquitectura y tengo este problema: En la elaboración manual de presupuestos de obra, el personal debe calcular cantidades de materiales, mano de obra, maquinaria y costos unitarios. El equipo que prepara presupuestos invierte tiempo en revisar hojas de cálculo y modificar numerosos datos cuando cambia el proyecto. Como estimación preliminar, esto podría ocupar entre 6 y 10 horas por semana; la cifra debe comprobarse con un registro real.

Responde en español con esta estructura:

1. Qué tipo de IA (predictiva, generativa o agente) es más adecuado para este problema y por qué.

2. Qué datos se necesitarían y de dónde saldrían.

3. Un riesgo ético o de privacidad que debería considerarse.

4. Un primer paso concreto que podría hacer esta semana sin programar.

Limita la respuesta a 250 palabras.
```

## Resultado obtenido
1. Tipo de IA: la IA generativa puede explicar cambios de partidas y ayudar a revisar inconsistencias, pero no reemplaza las fórmulas ni la revisión profesional.
2. Datos: catálogo de conceptos, cantidades de planos, cotizaciones vigentes, mano de obra, maquinaria y versiones del presupuesto.
3. Riesgo: subir a herramientas externas cotizaciones o planos identificables puede exponer información confidencial.
4. Primer paso: registrar durante una semana el tiempo real que toma actualizar partidas, con un presupuesto ficticio y autorización para el manejo de datos.

## Verificación
| Afirmación verificable | Fuente primaria | Clasificación |
|---|---|---|
| El proyecto aborda presupuestos manuales | https://github.com/camilobg2005-hash/ia-aplicada-2026/blob/main/proyecto/ficha_inicial.md | Correcta |
| Se utilizan planos y catálogos | https://github.com/camilobg2005-hash/ia-aplicada-2026/blob/main/proyecto/ficha_inicial.md | Correcta |
| Las 6–10 horas son una estimación pendiente de comprobar | https://github.com/camilobg2005-hash/ia-aplicada-2026/blob/main/laboratorios/semana01/prompt.txt | Correcta |

Tasa de error de esta respuesta: **0.0 %**.

## Evaluación
- Qué funcionó: Consistencia con la ficha original.
- Qué falló: Faltan mediciones de tiempo.
- Qué cambiaré en la siguiente versión: Registrar tiempos medidos.

## Historial de versiones
| Versión | Fecha | Cambio realizado | Resultado del cambio |
|---|---|---|---|
| v1 | 2026-10-18 | Versión inicial | Respuesta y verificación documentadas |

## Datos usados
Cumplimiento preventivo de la sección 5: **sí, sujeto a cotejar la política íntegra**. Se usaron datos públicos y supuestos, sin documentos confidenciales o datos personales.
