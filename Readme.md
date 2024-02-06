# Proyecto de Análisis de Mercado de Automóviles

## Introducción

Este proyecto tiene como objetivo realizar un análisis exhaustivo del mercado de automóviles para una importante automotriz china que planea ingresar al mercado. La consultora de ciencias de datos ha sido contratada para analizar las características de los vehículos presentes en el mercado actual y proporcionar insights valiosos para ajustar su catálogo a las demandas de los diferentes segmentos, especialmente en las gamas alta y baja.

## Objetivos del Proyecto

1. Analizar detalladamente las características de los vehículos presentes en el mercado.
2. Estratificar los datos en gamas alta y baja para comprender las diferencias clave.
3. Diseñar modelos predictivos para estimar el precio de los vehículos.
4. Crear un modelo predictivo para distinguir entre vehículos de gama alta y baja.
5. Proporcionar archivos con las predicciones en formato de texto plano.

## Metodología

### Análisis Exploratorio de Datos (EDA)

Se realizaron análisis exploratorios de datos para comprender la distribución y la relación entre las diferentes características de los vehículos. Se identificaron patrones y tendencias que son relevantes para la estrategia de mercado.

### Preprocesamiento de Datos

Los datos fueron preprocesados para manejar valores nulos, escalado de características y codificación de variables categóricas. Se utilizó la mediana de los precios como punto de corte para clasificar los vehículos en las categorías de gama alta y baja.

### Modelos Predictivos

Se diseñaron dos modelos predictivos utilizando algoritmos de aprendizaje automático:
1. **Modelo de Predicción de Precio:** Un modelo para estimar el precio de los vehículos.
2. **Modelo de Clasificación de Gama:** Un modelo para distinguir entre vehículos de gama alta y baja.

### Resultados y Conclusiones

#### Symboling
- **Alta Gama:** Los vehículos de alta gama tienden a tener un symboling más neutral (cerca de 0), indicando un menor riesgo. Esto podría sugerir que los autos de alta gama tienden a tener un perfil de riesgo más bajo.

#### Fuel Type
- **Alta Gama:** Predominancia de autos de alta gama con combustible tipo gas. La elección del tipo de combustible no parece ser un factor distintivo entre gamas.

#### Aspiration
- **Alta Gama:** La mayoría de los autos, tanto de gama alta como baja, tienen aspiración estándar (std). Esto sugiere que la presencia de turbocompresores no es distintiva en la clasificación de gama.

#### Doornumber
- **Conclusiones:** El número de puertas no parece ser un factor distintivo entre gama alta y baja.

#### Car Length and Car Width
- **Alta Gama:** Los autos de alta gama tienden a ser más largos y anchos, lo que podría contribuir a su apariencia más imponente y espaciosa.

#### Car Height
- **Conclusiones:** No se obtuvieron conclusiones claras sobre la altura de los autos en relación con la clasificación de gama.

#### Curb Weight
- **Alta Gama:** Los autos de alta gama tienden a ser más pesados, posiblemente debido a características adicionales de lujo y tecnología.

#### Engine Type and Cylinder Number
- **Alta Gama:** Los autos de alta gama suelen tener motores ohcv con más cilindros en comparación con la gama baja.

#### Engine Size
- **Alta Gama:** Los autos de alta gama tienden a tener motores más grandes. Esto es un factor determinante en la clasificación de gama.

#### Fuel System
- **Alta Gama:** Predominancia de autos de alta gama con sistema de inyección de combustible multipuerto (mpfi).

#### Horsepower
- **Alta Gama:** Los autos de alta gama tienden a tener más caballos de fuerza, contribuyendo a un mejor rendimiento.

#### Peak RPM
- **Conclusiones:** No se obtuvieron conclusiones claras sobre la velocidad máxima del motor.

#### City MPG and Highway MPG
- **Conclusiones:** Los autos de alta gama tienden a tener un menor rendimiento en términos de millas por galón, tanto en ciudad como en carretera, posiblemente debido a motores más potentes y un mayor peso.

En resumen, las conclusiones brindan una comprensión detallada de las características distintivas entre vehículos de gama alta y baja en el mercado. Estos hallazgos permitirán a la automotriz ajustar estratégicamente su catálogo para satisfacer las demandas específicas del mercado local.

## Archivos Generados

1. **Predicciones de Precio:** Archivo de texto plano con las predicciones de precio para los vehículos.
2. **Predicciones de Clasificación de Gama:** Archivo de texto plano con las predicciones de clasificación de gama para los vehículos.

## Modelo de Regresión Lineal:

- **Mean Squared Error (MSE):** 9663478.68
- **Root Mean Squared Error (RMSE):** 3108.61
- **R-squared (R2):** 0.8408

El modelo de regresión lineal proporciona una buena capacidad predictiva, con un R2 del 84.08%. Sin embargo, el RMSE indica que hay alguna variabilidad en las predicciones.

## Modelo k-NN:

- **Mean Squared Error (MSE):** 8296963.87
- **Root Mean Squared Error (RMSE):** 2880.45
- **R-squared (R2):** 0.8633

El modelo k-NN muestra un rendimiento mejorado en comparación con la regresión lineal, con un R2 del 86.33%. El RMSE más bajo sugiere una reducción en la variabilidad de las predicciones.

## Modelo de Árbol de Decisión:

- **Mean Squared Error (MSE):** 8316544.49
- **Root Mean Squared Error (RMSE):** 2883.84
- **R-squared (R2):** 0.8630

El modelo de árbol de decisión presenta resultados similares al k-NN, con un R2 del 86.30%. El RMSE también es bajo, indicando una precisión mejorada en las predicciones.

## Conclusiones Generales:

1. El modelo k-NN y el modelo de árbol de decisión superan ligeramente al modelo de regresión lineal en términos de precisión predictiva.

2. Ambos modelos no lineales (k-NN y árbol de decisión) demuestran una capacidad mejorada para capturar la complejidad en los datos de precios de vehículos.

3. Se recomienda seleccionar el modelo k-NN o el modelo de árbol de decisión para futuras predicciones de precios, considerando su menor RMSE y mayor R2 en comparación con la regresión lineal.

Estas conclusiones orientarán a nuestra automotriz cliente en la toma de decisiones estratégicas para cotizar correctamente los vehículos en el mercado, mejorando la competitividad y satisfaciendo las demandas de los diferentes segmentos de consumidores.