# Reflexión final

1. **Si tuviera que quitar una técnica, ¿cuál sería y cuántos puntos perdería?**  
   Quitarías los **ejemplos few-shot**. La iteración 3 obtuvo 18/18 y la iteración 4, que añadió el ejemplo, también obtuvo 18/18. En esta prueba la pérdida sería de **0 puntos**.

2. **¿Qué tendría que cambiar para que otra persona obtenga los mismos puntajes?**  
   Los criterios tendrían que convertirse en una rúbrica operativa con reglas de conteo y ejemplos de casos límite. Además, dos evaluadores deberían calificar de forma independiente las mismas respuestas y comparar discrepancias antes de fijar el puntaje final.

3. **Si el modelo cambia de versión el próximo mes, ¿qué seguiría siendo útil y qué habría que repetir?**  
   Seguirían siendo útiles las entradas de prueba, la rúbrica, la plantilla, el CSV y la lógica de evaluación. Habría que repetir las seis ejecuciones y la prueba de robustez con la nueva versión, porque el comportamiento y los puntajes pueden cambiar aunque el prompt sea idéntico.
