# Iteración 2 - Rol + contexto

**Fecha de ejecución:** 25 de octubre de 2026

## Prompt

```text
Eres arquitecto junior encargado de levantar requerimientos preliminares. Tu lector es el equipo de proyecto y necesita información clara y útil.

Contexto: las descripciones provienen de clientes sin formación técnica. La ficha debe cubrir uso, superficie, ventilación, iluminación y normativa aplicable. Esta etapa es únicamente de levantamiento preliminar: no se realizan cálculos normativos ni proyecto ejecutivo y cualquier dato no indicado por el cliente debe tratarse como pendiente de verificación.

Haz la ficha de requerimientos de este espacio:

{ENTRADA}
```

## Entrada 1

- **Uso:** estudio de arquitectura para dos personas en planta baja.
- **Superficie:** 12 m² (3.00 x 4.00 m).
- **Ventilación:** ventana operable de 1.50 x 1.20 m hacia patio. No se indicó un desempeño o requisito normativo específico.
- **Iluminación:** natural durante el día y artificial de apoyo para trabajo de escritorio.
- **Normativa aplicable:** Código Municipal de Aguascalientes y Código Urbano para el Estado de Aguascalientes, conforme a lo solicitado por el cliente; los requisitos concretos deben verificarse.
- **Información pendiente:** requisitos normativos específicos de ventilación e iluminación.

**Evaluación:** C1 2/2; C2 1/2; C3 2/2. Subtotal: **5/6**.

## Entrada 2

- **Uso:** consultorio de nutrición para atención individual, con escritorio y dos sillas.
- **Superficie:** no especificada; requiere levantamiento.
- **Ventilación:** el cliente solicita un espacio ventilado, pero no hay medidas ni datos sobre ventanas.
- **Iluminación:** el cliente solicita que sea iluminado, sin indicar fuente, nivel ni condiciones de luz natural.
- **Normativa aplicable:** no especificada por el cliente.
- **Información pendiente:** dimensiones del cuarto, puertas y ventanas; condiciones actuales; alcance de modificaciones; normativa que resulte aplicable.

**Evaluación:** C1 2/2; C2 1/2; C3 2/2. Subtotal: **5/6**.

## Entrada 3

- **Uso:** taller pequeño de maquetas en habitación existente.
- **Superficie:** información contradictoria: se mencionan 9 m² y 12 m²; debe verificarse en sitio o con documentación confiable.
- **Ventilación:** existe una ventana, pero no se sabe si es operable; el cliente expresa que no quiere mantenerla abierta por el polvo. Como medida preliminar, puede considerarse ventilación mecánica mientras se verifica la condición real.
- **Iluminación:** se solicita mucha luz natural y evitar sol directo sobre la mesa de trabajo.
- **Normativa aplicable:** no especificada.
- **Información pendiente:** superficie real, operabilidad de la ventana y normativa aplicable.

**Evaluación:** C1 2/2; C2 1/2; C3 1/2. Subtotal: **4/6**.

## Resultado

- C1: **6/6**
- C2: **3/6**
- C3: **5/6**
- **Total: 14/18**
