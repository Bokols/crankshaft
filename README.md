# Proyecto: Análisis de los Factores que Afectan el Precio de los Vehículos

## Introducción
Este proyecto explora los factores que influyen en los precios de los vehículos basados en un conjunto de datos de anuncios de vehículos. El objetivo es identificar los elementos clave como la edad del vehículo, el kilometraje, el estado, el tipo de combustible, la transmisión y otros atributos relevantes que contribuyen al precio de un vehículo. A través de este análisis, utilizamos métodos estadísticos y visualizaciones para proporcionar información sobre las relaciones entre estos factores y el precio de los vehículos. El análisis incluye el manejo de valores faltantes, valores atípicos y el enriquecimiento del conjunto de datos para garantizar una comprensión completa de las variables clave que afectan los precios de los vehículos.

## Resumen
El conjunto de datos contiene 51,525 filas y 13 columnas, con atributos como el año del modelo, cilindrada, odómetro (kilometraje), tipo de combustible, color de pintura y más. El análisis se centró en identificar las correlaciones entre las diferentes variables y su efecto en el precio. El conjunto de datos fue limpiado para abordar los valores faltantes y los valores atípicos, y se introdujeron características adicionales como la edad del vehículo, el kilometraje por año y el rango de condición. A continuación, se presentan los hallazgos observados:

- **Edad del vehículo** muestra una correlación negativa con el precio, ya que los vehículos más antiguos tienden a ser más baratos.
- **Kilometraje por año** presenta una correlación positiva sorprendente con el precio, lo que sugiere que los vehículos con mayor kilometraje anual pueden tener precios más altos en algunos casos.
- **Condición** tiene una correlación positiva con el precio, ya que los vehículos en mejor estado se cotizan más alto.
- **Cilindrada** tiene un impacto significativo en las camionetas, donde más cilindros resultan en precios más altos.
- **Tipo de combustible** revela que los vehículos diésel tienden a tener un precio más alto en promedio que los vehículos de gasolina.
- **Transmisión** afecta el precio, con transmisiones automáticas siendo más caras en promedio para sedanes y camionetas.
- **Color de pintura** influye en el precio, siendo el amarillo el color más caro y el morado el menos costoso.

## Hallazgos

### 1. Edad del Vehículo y Precio
- **Correlación**: Existe una correlación negativa moderada (-0.47) entre la edad del vehículo y el precio. Los vehículos más antiguos suelen tener precios más bajos, lo cual es esperado ya que los autos tienden a depreciarse con el tiempo. Sin embargo, existen excepciones, donde los vehículos antiguos bien mantenidos aún pueden tener precios altos.
- **Visualización**: El gráfico de dispersión y el análisis de regresión confirman esta relación negativa, especialmente para tipos de vehículos como las camionetas, que muestran una disminución más pronunciada en el precio con la edad.

### 2. Kilometraje por Año y Precio
- **Correlación**: Sorprendentemente, existe una correlación positiva (0.20) entre el kilometraje por año y el precio. Este hallazgo sugiere que los vehículos con mayor kilometraje por año tienden a tener precios más altos, posiblemente debido a factores como el uso aventurero o comercial que justifica un costo más alto.
- **Visualización**: El gráfico de dispersión y el análisis de regresión muestran una correlación positiva sutil, especialmente notable para las camionetas y SUVs.

### 3. Condición del Vehículo y Precio
- **Correlación**: La condición está positivamente correlacionada con el precio (0.19). Los vehículos en mejor estado, como era de esperarse, tienen precios más altos. Esto es consistente en la mayoría de los tipos de vehículos.
- **Visualización**: El gráfico de dispersión y el análisis de regresión demuestran una clara tendencia de precios más altos para los vehículos en mejor estado.

### 4. Cilindrada y Precio
- **Correlación**: Existe una correlación positiva (0.29) entre la cantidad de cilindros y el precio, particularmente en las camionetas. Los vehículos con más cilindros (6, 8, 10, 12) tienden a tener precios más altos, probablemente debido a su mayor potencia y capacidades de rendimiento.
- **Visualización**: El gráfico de barras muestra que el precio aumenta significativamente con la cantidad de cilindros, especialmente en las camionetas.

### 5. Tipo de Combustible y Precio
- **Hallazgos sobre el tipo de combustible**: Los vehículos diésel tienden a tener precios más altos en promedio en comparación con los de gasolina, especialmente cuando se comparan con vehículos de gasolina. Esto podría deberse a la mayor eficiencia de combustible y la vida útil más larga de los motores diésel.
- **Visualización**: El gráfico de barras indica que los vehículos diésel están consistentemente más caros que los de gasolina.

### 6. Transmisión y Precio
- **Hallazgos sobre la transmisión**: Los vehículos con transmisión automática tienden a ser más caros para los sedanes y camionetas, mientras que las transmisiones manuales son más comunes en los SUVs y tienden a ser más caras en esa categoría.
- **Visualización**: El gráfico de barras muestra claramente que los sedanes y camionetas con transmisión automática son más caros, mientras que los SUVs manuales tienen un precio más alto en promedio.

### 7. Color de Pintura y Precio
- **Hallazgos sobre el color de pintura**: El amarillo es el color más caro, mientras que el morado es el menos costoso. El color de un vehículo parece influir en su precio, con colores más comunes como el negro, blanco y plateado teniendo precios moderados.
- **Visualización**: El gráfico de barras indica que el color de pintura afecta el precio, con los vehículos amarillos teniendo los precios medianos más altos.

### 8. Datos Faltantes y Valores Atípicos
- **Datos Faltantes**: Cinco columnas tenían valores faltantes (NaN), incluyendo año del modelo, cilindrada, odómetro, color de pintura e información de 4WD. Estos valores faltantes fueron tratados reemplazando los NaN con valores predeterminados o utilizando correlaciones de otras columnas para imputar datos faltantes.
- **Valores Atípicos**: Los valores atípicos se identificaron utilizando cuantiles, y se aplicaron filtros para limpiar los datos, especialmente en las columnas de precio, días listados, kilometraje y condición.

## Conclusión

Este análisis confirma que múltiples factores influyen en los precios de los vehículos, con algunas variables mostrando correlaciones fuertes y otras mostrando impactos más sutiles. Los hallazgos clave incluyen:

- **La Edad del Vehículo** tiene la correlación negativa más fuerte con el precio.
- **La Condición** y **Cilindrada** contribuyen positivamente a precios más altos, especialmente para las camionetas.
- **Tipo de Combustible** y **Transmisión** también tienen un impacto significativo en el precio, con los vehículos diésel y las transmisiones automáticas comandando precios más altos.
- **Kilometraje por Año** muestra una relación positiva inesperada con el precio, sugiriendo que un mayor kilometraje a veces puede correlacionarse con precios más altos, posiblemente debido a patrones de uso del vehículo.

El conjunto de datos fue limpiado y enriquecido cuidadosamente para asegurar que el análisis se basara en datos precisos y significativos. Este estudio proporciona valiosas perspectivas para compradores, vendedores y analistas que deseen entender los factores que impulsan los precios de los vehículos en el mercado. Análisis futuros podrían explorar variables adicionales como marca, modelo y factores regionales específicos que podrían influir aún más en las tendencias de precios.
