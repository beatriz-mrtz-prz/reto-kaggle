# Kaggle Challenge – House Prices

Ejercicio final de Introducción a Python para Data Science: mejorar la puntuación obtenida en clase (0.18878) en la competición [House Prices: Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques).

## Resultado

| Modelo | Puntuación Kaggle |
|---|---|
| Clase: LinearRegression, 10 variables | 0.18878 |
| Este notebook: GradientBoostingRegressor, todas las variables, log(SalePrice) | **0.12610** |

## Mejoras aplicadas

- Predicción de `log(SalePrice)`, que es la escala en la que puntúa Kaggle.
- Eliminación de outliers (casas de más de 4.000 pies² con precio anormalmente bajo).
- Uso de todas las variables, con imputación de nulos y one-hot encoding.
- Nuevas variables: superficie total, baños totales, antigüedad y porches.
- Comparación de Ridge y Gradient Boosting en validación; modelo final: Gradient Boosting.

## Datos

Los datos no se incluyen en el repositorio. Para ejecutar el notebook, descárgalos desde la pestaña *Data* de la competición y colócalos en una carpeta `data/` junto al notebook.
