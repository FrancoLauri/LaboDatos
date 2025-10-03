#El Trabajo Final de la cursada de Laboratorio de Datos (UBA) consistió en armar un modelo predictivo con la idea de responder una pregunta que nos hayamos formulado en el grupo de trabajo (dos personas)
La consulta de nuestro trabajo fue "¿Es posible predecir la cantidad de NOX del aire (un contaminante) en funcion de variables climaticas y de tránsito?"

El trabajo comenzó buscando y armando un dataset acorde para responder la duda, el cual fue conformado mediante tres datasets distintos: 
i)Datos del transito del gobienrno de CABA los cuales accedimos mediante la API
ii)Datos de los medidores de calidad de aire de CABA, los cuales accedimos usando un selenium para navegar la web
iii)Un csv de datos climaticos de CABA

Una vez armado el dataset, se realizaron diversas tareas para limpiarlo y procesarlo, como restructurar las columnas, eliminar los nan, etc.
Logramos un dataset de 4400 registros aprox y 13 columnas sobre el clima, el transito, las fechas y la ubicacion de los medidores

Luego, armamos el modelo el cual consistió en construir un pipeline en Python utilizando la librería scikit-learn.  El modelo seleccionado fue un Random Forest Regressor, elegido por su capacidad para manejar relaciones no lineales y datos con diferentes escalas. El entrenamiento se realizó con un conjunto de datos compuesto por información de tráfico, clima y calidad del aire, segmentado por rango horario y ubicación. Finalmente, se evaluó el desempeño del modelo utilizando métricas como el R² y el error absoluto medio (MAE), obteniendo resultados satisfactorios para la predicción de los niveles de NOx en la CABA

Por último, evaluamos el modelo lo cual incluyó tanto métricas como visualizaciones para analizar su desempeño y la relación entre las variables. Se utilizaron el coeficiente de determinación (R²) y el error absoluto medio (MAE) como métricas principale

Para mas detalles observar la presentación o el colab donde se encuentran todas las visualizaciones ralizadas
