# Iteración 3 - Rol + contexto + formato

**Fecha de ejecución:** 25 de octubre de 2026

## Prompt

```text
Eres arquitecto junior encargado de levantar requerimientos preliminares. Tu lector es el equipo de proyecto y necesita información clara y útil.

Contexto: las descripciones provienen de clientes sin formación técnica. La ficha debe cubrir uso, superficie, ventilación, iluminación y normativa aplicable. Esta etapa es únicamente de levantamiento preliminar: no se realizan cálculos normativos ni proyecto ejecutivo y cualquier dato no indicado por el cliente debe tratarse como pendiente de verificación.

Responde únicamente con esta tabla en Markdown, sin texto adicional:

| Campo | Requerimiento |
|---|---|
| Uso | |
| Superficie | |
| Ventilación | |
| Iluminación | |
| Normativa aplicable | |
| Información faltante | |

Si un campo no puede determinarse a partir del texto, escribe `NO ESPECIFICADO`. Si hay dos datos que se contradicen, escribe `CONTRADICTORIO` y conserva ambos valores para que puedan verificarse. No agregues medidas, porcentajes, normas ni condiciones que el cliente no haya indicado.

Texto del cliente:
{ENTRADA}
```

## Entrada 1

| Campo | Requerimiento |
|---|---|
| Uso | Estudio de arquitectura para dos personas en planta baja |
| Superficie | 12 m² (3.00 m x 4.00 m) |
| Ventilación | Ventana operable de 1.50 m x 1.20 m hacia patio; requisito de desempeño NO ESPECIFICADO |
| Iluminación | Iluminación natural durante el día y luminaria artificial de apoyo para trabajo de escritorio |
| Normativa aplicable | Código Municipal de Aguascalientes y Código Urbano para el Estado de Aguascalientes, indicados por el cliente; requisitos concretos NO ESPECIFICADOS |
| Información faltante | Requisitos concretos de ventilación, iluminación y cumplimiento normativo |

**Evaluación:** C1 2/2; C2 2/2; C3 2/2. Subtotal: **6/6**.

## Entrada 2

| Campo | Requerimiento |
|---|---|
| Uso | Consultorio de nutrición para atender a una persona, con escritorio y dos sillas |
| Superficie | NO ESPECIFICADO |
| Ventilación | Se desea un espacio ventilado; dimensiones y características de ventanas NO ESPECIFICADAS |
| Iluminación | Se desea un espacio iluminado; fuente y condiciones de iluminación NO ESPECIFICADAS |
| Normativa aplicable | NO ESPECIFICADO |
| Información faltante | Medidas del cuarto, puertas y ventanas; condiciones actuales; alcance de modificaciones; normativa aplicable |

**Evaluación:** C1 2/2; C2 2/2; C3 2/2. Subtotal: **6/6**.

## Entrada 3

| Campo | Requerimiento |
|---|---|
| Uso | Taller pequeño de maquetas en una habitación existente |
| Superficie | CONTRADICTORIO: 9 m² / 12 m² |
| Ventilación | Existe una ventana; operabilidad NO ESPECIFICADA. El cliente no quiere mantenerla abierta por el polvo |
| Iluminación | Mucha luz natural, evitando entrada directa de sol sobre la mesa de trabajo |
| Normativa aplicable | NO ESPECIFICADO |
| Información faltante | Verificar superficie real, operabilidad de la ventana y normativa aplicable |

**Evaluación:** C1 2/2; C2 2/2; C3 2/2. Subtotal: **6/6**.

## Resultado

- C1: **6/6**
- C2: **6/6**
- C3: **6/6**
- **Total: 18/18**
