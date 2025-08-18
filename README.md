# clasificacion-validacion-de-modelos-y-metricas
Este repositorio corresponde al entrenamiento de Clasificación: Validación de Modelos y métricas de evaluación de Alura Latam.

## Error por corregir
Existe un **error por corregir** en el cálculo de las métricas y gráficos:
* AUC ROC score
* ROC curve
* Precision Average score
* Precision x recall curve
Al respecto, **no** se debe emplear las *predicciones de y* como parámetro de los métodos para calcular y graficar los anteriores elementos. **Sino** que se deben emplear *estimaciones de probabilidad de la clase positiva*, o *medidas de decisiones sin umbral* (como las que devuelve ```decision_function``` en algunos clasificadores). Esto según la documentación oficial y lo explicado en un foro de [Stackoverflow](https://stackoverflow.com/questions/65398299/proper-inputs-for-scikit-learn-roc-auc-score-and-roc-plot).
