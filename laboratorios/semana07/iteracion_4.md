# Iteración 4 - Anterior + ejemplos (few-shot)

**Modelo usado:** ChatGPT (GPT-5.6 Sol)  
**Fecha de ejecución:** 25 de octubre de 2026

## Cambio aplicado

Se conservó rol, contexto y formato de la iteración 3 y se añadió un ejemplo completo distinto a las tres entradas de prueba.

### Ejemplo de entrada
“Se requiere una pequeña bodega para maquetas terminadas. Superficie disponible: 8 m². No tiene ventana y el cliente no pide ventilación natural; solicita conservar la extracción mecánica existente. Iluminación: solo artificial, con las luminarias de techo existentes. No se indicó ubicación del inmueble ni normativa.”

### Ejemplo de salida
| Campo | Requerimiento |
|---|---|
| Uso | Bodega para maquetas terminadas |
| Superficie | 8 m² |
| Ventilación | Conservar la extracción mecánica existente; no se solicita ventilación natural |
| Iluminación | Artificial con luminarias de techo existentes |
| Normativa aplicable | NO ESPECIFICADO |
| Información faltante | Ubicación del inmueble y normativa aplicable |

## Entrada 1

| Campo | Requerimiento |
|---|---|
| Uso | Estudio de arquitectura para dos personas en planta baja |
| Superficie | 12 m² (3.00 m x 4.00 m) |
| Ventilación | Ventana operable de 1.50 m x 1.20 m hacia patio; requisito de desempeño NO ESPECIFICADO |
| Iluminación | Iluminación natural durante el día y luminaria artificial de apoyo para trabajo de escritorio |
| Normativa aplicable | Código Municipal de Aguascalientes y Código Urbano para el Estado de Aguascalientes, indicados por el cliente; requisitos concretos NO ESPECIFICADOS |
| Información faltante | Requisitos concretos de ventilación, iluminación y cumplimiento normativo |

**Evaluación:** 6/6.

## Entrada 2

| Campo | Requerimiento |
|---|---|
| Uso | Consultorio de nutrición para atender a una persona, con escritorio y dos sillas |
| Superficie | NO ESPECIFICADO |
| Ventilación | Se desea un espacio ventilado; dimensiones y características de ventanas NO ESPECIFICADAS |
| Iluminación | Se desea un espacio iluminado; fuente y condiciones de iluminación NO ESPECIFICADAS |
| Normativa aplicable | NO ESPECIFICADO |
| Información faltante | Medidas del cuarto, puertas y ventanas; condiciones actuales; alcance de modificaciones; normativa aplicable |

**Evaluación:** 6/6.

## Entrada 3

| Campo | Requerimiento |
|---|---|
| Uso | Taller pequeño de maquetas en una habitación existente |
| Superficie | CONTRADICTORIO: 9 m² / 12 m² |
| Ventilación | Existe una ventana; operabilidad NO ESPECIFICADA. El cliente no quiere mantenerla abierta por el polvo |
| Iluminación | Mucha luz natural, evitando entrada directa de sol sobre la mesa de trabajo |
| Normativa aplicable | NO ESPECIFICADO |
| Información faltante | Verificar superficie real, operabilidad de la ventana y normativa aplicable |

**Evaluación:** 6/6.

## Resultado

- C1: **6/6**
- C2: **6/6**
- C3: **6/6**
- **Total: 18/18**
- Observación: el ejemplo confirmó el patrón esperado, pero no mejoró el puntaje respecto a la iteración 3.
