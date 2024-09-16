Esta práctica emplea un conjunto de datos sobre los precios de viviendas en California, basado en la información del censo de 1990. 
Dicho conjunto de datos es proporcionado por el libro <i>Aprende Machine Learning con Scikit-Learn, Keras y TensorFlow</i>. 
En este data frame, cada fila representa un bloque que consiste en un conjunto de viviendas. Inicialmente, 
el data frame cuenta con las siguientes características: longitude, latitude, housing_median_age, total_rooms, total_bedrooms, 
population, households, median_income, ocean_proximity y  median_house_value, esta última es la variable objetivo.

En el análisis exploratorio, se podrá observar que la variable que mejor explica el "precio mediano de las viviendas" en California ("median_house_value")
es el "ingreso mediano"("median_income"). Además, se generarán nuevas variables que muestran una buena correlación con el objetivo (target).

El conjunto de datos se prepara para los algoritmos de machine learning mediante la incorporación de nuevas variables, la transformación de distribuciones, 
el escalado y la imputación de valores en las variables numéricas. Para las variables categóricas, se crearán variables ficticias (dummies), y 
se utilizará un algoritmo de similitud para manejar la ubicación.

Se seleccionarán diversos algoritmos de regresión, como la regresión lineal, los árboles de decisión, los bosques aleatorios y las máquinas de soporte vectorial, 
con el objetivo de minimizar la raíz del error cuadrático medio, que actúa como función de pérdida.
Por último, se empleará el conjunto de prueba con el mejor algoritmo, en este caso, las máquinas de soporte vectorial, para verificar su rendimiento y estimar un intervalo de confianza
