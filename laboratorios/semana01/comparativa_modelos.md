# Comparativa de modelos semana 1

Se envió el mismo texto de `prompt.txt` en conversaciones nuevas el 23 de septiembre de 2026. DeepSeek exige iniciar sesión, Copilot indicó que no estaba disponible en la región y Claude presentó una verificación de seguridad. La tercera comparación sigue pendiente.

| Punto comparado | ChatGPT | Gemini | Tercer modelo |
|---|---|---|---|
| Tipo de IA que recomendó | Agente con apoyo generativo | Híbrido generativa + agentes | Pendiente |
| Datos que dijo que se necesitan | Planos BIM/CAD, conceptos, precios, rendimientos, históricos | Presupuestos históricos, precios locales y bitácora de cambios | Pendiente |
| Riesgo ético que mencionó | Confidencialidad comercial de precios y márgenes | Errores numéricos y posible filtración de datos financieros | Pendiente |
| Primer paso que propuso | Medir tiempos en 2 o 3 presupuestos y documentar una partida | Registrar tiempos y crear matriz de variables críticas | Pendiente |
| ¿Respetó la estructura de 4 puntos? | Sí | Sí; añadió pregunta final | Pendiente |
| ¿Respetó el límite de 250 palabras? | Sí, aproximadamente 242 | Sí, aproximadamente 202 | Pendiente |
| Afirmación incorrecta o dudosa | Supone que un agente puede leer planos y recalcular cantidades: requiere comprobar formatos, integración y exactitud | Supone que agentes actualizarían automáticamente fórmulas y celdas: no conoce la estructura real del Excel | Pendiente |

## Respuestas completas

### ChatGPT

1. Tipo de IA más adecuado
IA agente, complementada con IA generativa. Un agente podría leer los datos del proyecto, recalcular cantidades y costos, actualizar el presupuesto y señalar cambios o inconsistencias. La IA generativa ayudaría a interpretar planos, partidas y especificaciones. La cifra de 6–10 horas semanales debe validarse con registros reales antes de cuantificar el beneficio.

2. Datos necesarios y origen
Planos y modelos BIM/CAD: superficies, volúmenes, elementos y dimensiones.
Catálogo de conceptos: partidas, unidades, rendimientos y fórmulas; de presupuestos históricos.
Precios unitarios: materiales, mano de obra y maquinaria; de bases internas y cotizaciones de proveedores.
Factores de productividad y desperdicio: históricos de obra y criterios del equipo.
Presupuestos anteriores: para comparar resultados y detectar desviaciones.

3. Riesgo ético o de privacidad
Los presupuestos pueden contener información comercial confidencial, como precios negociados, márgenes y condiciones de proveedores. Si se utilizan servicios externos de IA, debe verificarse dónde se almacenan los datos, quién puede acceder a ellos y si se usan para entrenar modelos. También conviene establecer controles de acceso y anonimización cuando sea posible.

4. Primer paso esta semana, sin programar
Realizar un piloto manual de medición: elegir 2–3 presupuestos recientes y registrar durante una semana cuánto tiempo dedica cada persona a revisar datos, calcular cantidades, actualizar precios y corregir cambios. Después, seleccionar una partida repetitiva y documentar su proceso paso a paso. Esto proporciona una línea base para decidir qué automatizar primero y medir posteriormente el ahorro real.

### Gemini

1. Tipo de IA adecuado
El más idóneo es un sistema híbrido (IA Generativa + Agentes de IA). La IA generativa permite interpretar los cambios de diseño en lenguaje natural, mientras que los agentes autónomos ejecutan tareas encadenadas para actualizar automáticamente las fórmulas y celdas interdependientes en las hojas de cálculo.

2. Datos necesarios y fuentes
Presupuestos históricos: Archivos Excel o bases de datos de obras pasadas.
Precios unitarios: Catálogos locales de materiales, mano de obra y maquinaria.
Bitácora de cambios: Registro estructurado de las modificaciones solicitadas por los clientes.

3. Riesgos éticos y de privacidad
El mayor riesgo es la alucinación de datos o errores numéricos en los costos, lo que podría derivar en presupuestos erróneos y pérdidas financieras. Además, existe un riesgo de filtración si se suben datos financieros confidenciales de la constructora a plataformas públicas.

4. Primer paso concreto (sin programar)
Esta semana, implementa una bitácora de tiempo real para medir con precisión las horas que el equipo dedica a los ajustes (verificando la estimación de 6-10 horas) y diseña una "matriz de variables críticas" en Excel que aísle los datos que cambian con mayor frecuencia en tus proyectos.

¿Te gustaría que profundicemos en cómo estructurar esa matriz de variables?

### Tercer modelo

Pendiente de ejecutar una conversación nueva y anexar captura original.

## Evidencia

Las capturas de ChatGPT y Gemini están conservadas junto con el reporte. La interfaz despliega el prompt y la respuesta en distintas posiciones de desplazamiento, por lo que la transcripción íntegra se incluye arriba.
