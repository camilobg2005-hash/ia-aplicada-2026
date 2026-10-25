# Análisis de resultados

| Iteración | Técnica | C1 | C2 | C3 | Total |
|---:|---|---:|---:|---:|---:|
| 0 | Línea base | 6 | 3 | 1 | 10 |
| 1 | Rol | 6 | 3 | 3 | 12 |
| 2 | Rol + contexto | 6 | 3 | 5 | 14 |
| 3 | Rol + contexto + formato | 6 | 6 | 6 | 18 |
| 4 | + ejemplo few-shot | 6 | 6 | 6 | 18 |
| 5 | + análisis previo | 6 | 3 | 6 | 15 |

## Mayor salto

La iteración 3 produjo el mayor aumento: pasó de 14 a 18 puntos, una mejora de 4 puntos. El cambio se concentró en C2 Formato (3 a 6) y C3 Manejo de incertidumbre (5 a 6).

## Descenso

La iteración 5 bajó de 18 a 15 puntos. C1 y C3 se mantuvieron al máximo, pero C2 cayó de 6 a 3 porque la nueva sección de análisis agregó texto antes de la tabla.

## Prompt adoptado

Se adopta la iteración 3, aunque la iteración 4 también obtuvo 18/18. La iteración 3 es más corta, no depende de un ejemplo y alcanzó el mismo resultado.
