# Transformaciones y auditoría de accesos — semana 3

**Datos:** 42 registros de ejemplo, enteramente ficticios. El conjunto limpio tiene 38: se eliminaron 3 duplicados exactos (id 4, 38 y 39) y 1 duplicado tras normalización (id 40). El CSV seudonimizado tiene 38.

## Columnas y tratamiento

| Columna original | Acción | Técnica | Razón |
|---|---|---|---|
| id | Eliminar | Supresión | El número original permitiría vincular ambos CSV. |
| nombre | Sustituir por id_persona | Seudonimización con código estable P001… | Permite contar visitas de una misma persona sin mostrar su nombre. La llave queda solo en el libro privado. |
| correo | Eliminar | Supresión | No es necesario para estudiar accesos. Se calculó correo_enmascarado en una columna auxiliar y se descartó del CSV. |
| telefono | Eliminar | Supresión | No aporta al análisis y revela contacto. |
| fecha_acceso | Sustituir por semana | Generalización, WEEKNUM con semana iniciada en domingo | Conserva patrones semanales sin día exacto; fechas irrecuperables pasan a Sin fecha. |
| hora_entrada | Sustituir por franja | Generalización de seis horas | Conserva la detección de madrugada y noche. |
| area | Conservar | Normalización de espacios y capitalización | Permite analizar el lugar; sigue siendo cuasiidentificador. |
| empresa | Sustituir por tipo_empresa | Generalización por giro | Reduce precisión del empleador. Los faltantes quedan No registrada. |
| motivo | Conservar | Normalización de texto | Permite interpretar accesos; no se infiere un motivo faltante. |

**Nota sobre la semana:** se aplicó la convención `WEEKNUM(fecha,1)` de Excel, en que la semana empieza el domingo. Los registros con fecha imposible conservaron la etiqueta «Sin fecha», no un número inventado.

## Clave de errores introducidos

La fila de hoja cuenta la cabecera como fila 1. Un registro puede figurar en más de una categoría.

| id | Fila de hoja | Error o dato inusual introducido |
|---:|---:|---|
| 2 | 3 | Fecha dd/mm/aaaa; Correo con mayúsculas o espacios; Teléfono con espacios; Área con distinta capitalización; Motivo con distinta capitalización |
| 3 | 4 | Teléfono vacío |
| 4 | 5 | Duplicado exacto |
| 5 | 6 | Correo sin dominio completo; Hora fuera de horario válida |
| 6 | 7 | Empresa vacía |
| 7 | 8 | Fecha inválida |
| 9 | 10 | Hora fuera de horario válida |
| 13 | 14 | Fecha dd/mm/aaaa |
| 14 | 15 | Correo con mayúsculas o espacios; Área con distinta capitalización |
| 16 | 17 | Teléfono vacío |
| 17 | 18 | Hora fuera de horario válida |
| 18 | 19 | Teléfono con espacios |
| 22 | 23 | Área con distinta capitalización |
| 23 | 24 | Fecha dd/mm/aaaa |
| 24 | 25 | Correo sin dominio completo |
| 26 | 27 | Teléfono corto |
| 27 | 28 | Correo con mayúsculas o espacios; Hora fuera de horario válida |
| 28 | 29 | Teléfono vacío |
| 29 | 30 | Empresa vacía |
| 30 | 31 | Fecha inválida |
| 31 | 32 | Teléfono con espacios |
| 33 | 34 | Fecha dd/mm/aaaa |
| 35 | 36 | Empresa vacía |
| 37 | 38 | Hora fuera de horario válida |
| 38 | 39 | Duplicado exacto |
| 39 | 40 | Duplicado exacto |
| 40 | 41 | Duplicado tras normalización; Correo con mayúsculas o espacios; Área con distinta capitalización; Motivo con distinta capitalización |

## Comparación de detección

| Tipo de error | Introducidos | Detectados | Faltaron | Explicación |
|---|---:|---:|---:|---|
| Correo con mayúsculas o espacios | 4 | 4 | 0 | Detectado y tratado; los valores imposibles o irrecuperables quedaron vacíos. |
| Correo sin dominio completo | 2 | 2 | 0 | Detectado y tratado; los valores imposibles o irrecuperables quedaron vacíos. |
| Duplicado exacto | 3 | 3 | 0 | Detectado y tratado; los valores imposibles o irrecuperables quedaron vacíos. |
| Duplicado tras normalización | 1 | 1 | 0 | Detectado y tratado; los valores imposibles o irrecuperables quedaron vacíos. |
| Empresa vacía | 3 | 3 | 0 | Detectado y tratado; los valores imposibles o irrecuperables quedaron vacíos. |
| Fecha dd/mm/aaaa | 4 | 4 | 0 | Detectado y tratado; los valores imposibles o irrecuperables quedaron vacíos. |
| Fecha inválida | 2 | 2 | 0 | Detectado y tratado; los valores imposibles o irrecuperables quedaron vacíos. |
| Hora fuera de horario válida | 5 | 5 | 0 | Se conservó deliberadamente: es un acceso inusual válido. |
| Motivo con distinta capitalización | 2 | 2 | 0 | Detectado y tratado; los valores imposibles o irrecuperables quedaron vacíos. |
| Teléfono con espacios | 3 | 3 | 0 | Detectado y tratado; los valores imposibles o irrecuperables quedaron vacíos. |
| Teléfono corto | 1 | 1 | 0 | Detectado y tratado; los valores imposibles o irrecuperables quedaron vacíos. |
| Teléfono vacío | 3 | 3 | 0 | Detectado y tratado; los valores imposibles o irrecuperables quedaron vacíos. |
| Área con distinta capitalización | 4 | 4 | 0 | Detectado y tratado; los valores imposibles o irrecuperables quedaron vacíos. |

## Incidencias no imputadas

| id | Campo | Decisión |
|---:|---|---|
| 3 | telefono | vacío; no imputado |
| 5 | correo | vacío; no imputado |
| 6 | empresa | vacío; no imputado |
| 7 | fecha_acceso | vacío; no imputado |
| 16 | telefono | vacío; no imputado |
| 24 | correo | vacío; no imputado |
| 26 | telefono | vacío; no imputado |
| 28 | telefono | vacío; no imputado |
| 29 | empresa | vacío; no imputado |
| 30 | fecha_acceso | vacío; no imputado |
| 35 | empresa | vacío; no imputado |

## Fórmulas auditables del libro privado

- Correo: `=LOWER(TRIM(accesos_crudo!C2))`
- Área y motivo: `=PROPER(TRIM(accesos_crudo!G2))` y `=PROPER(TRIM(accesos_crudo!I2))`
- Teléfono: `=SUBSTITUTE(accesos_crudo!D2," ","")`
- Enmascaramiento ilustrativo: `=IFERROR(LEFT(TRIM(accesos_crudo!C2),1)&"***"&MID(LOWER(TRIM(accesos_crudo!C2)),SEARCH("@",accesos_crudo!C2),99),"")`

## Prueba de combinaciones

Se agruparon `tipo_empresa + area + franja` en el CSV final. Cinco combinaciones aparecen una sola vez; por ejemplo:
- Constructora + Obra Norte + Tarde: 1 registro.
- Constructora + Obra Sur + Mañana: 1 registro.
- Diseño + Oficina Central + Madrugada: 1 registro.
- Diseño + Oficina Central + Noche: 1 registro.
- No registrada + Sala De Servidores + Noche: 1 registro.

Esto es un riesgo residual de vinculación si alguien conoce los horarios y el entorno. **No debe afirmarse anonimización irreversible**: además existe una tabla privada de seudónimos. El archivo contiene solo personas inventadas. Con datos reales se necesitaría separar la llave, controlar accesos y evaluar supresión o agrupación adicional antes de compartir.

**No se versionaron** `accesos_limpio`, `tabla_seudonimos` ni el libro privado.
