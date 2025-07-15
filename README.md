# Medical_Cost_Personal_Dataset

## Conclusión

En este proyecto se evaluaron distintos modelos de regresión para predecir costos médicos personales, utilizando validación cruzada y técnicas de optimización de hiperparámetros (`GridSearchCV` y `RandomizedSearchCV`).

### Resultados sin optimización de hiperparámetros

| Modelo                  | CV R² Score promedio |
|-------------------------|----------------------|
| KNN Regressor           | 0.63                 |
| Regresión Lineal        | 0.73                 |
| Random Forest Regressor | 0.82                 |

### Resultados con optimización de hiperparámetros

| Modelo                                    | R² Score optimizado |
|-------------------------------------------|---------------------|
| KNN (KNeighborsClassifier) GridSearchCV    | 0.72                |
| KNN (KNeighborsClassifier) RandomizedSearchCV | 0.84                |
| Random Forest Regressor GridSearchCV        | 0.90                |
| Random Forest Regressor RandomizedSearchCV  | 0.84                |

---

**Conclusión general:**  
La optimización de hiperparámetros mejora significativamente el rendimiento de los modelos. El Random Forest Regressor con GridSearchCV presentó el mejor desempeño, alcanzando un R² de 0.90, seguido por KNN optimizado con RandomizedSearchCV. Estos resultados sugieren que para este dataset, los modelos de ensamble y la búsqueda aleatoria de parámetros son más efectivos que los métodos lineales básicos o modelos sin optimización.


