![HenryLogo](https://d31uz8lwfmyn8g.cloudfront.net/Assets/logo-henry-white-lg.png)
​
# Proyecto individual 2
​
Segundo proyecto sobre habilidades en el campo de la predicción. Se usa la metrica considerada para dar el mejor resultado
​
## Información relevante
​
Se siguen las intrucciones requeridas para poder enviar el mejor modelo de prediccion requerido

## Mercado inmobiliario
​
Dentro de la sociedad globalizada e industrializada, es sabido que los precios de los inmuebles han presentado un constante cambio, por lo que quienes deseen invertir o vender una propiedad se enfrentan al fenómeno especulativo existente en la valorización de éstos. Esto, debido a la constante tendencia de las ciudades a crecer demográfica y comercialmente, llegando a un punto en donde no se tiene certeza de la valorización real dentro del sector en donde se desee invertir. 
​
Pese a que el precio depende, en cierta medida, de las tendencias que esté teniendo el mercado inmobiliario en un determinado tiempo, poder estimar adecuadamente el valor de una propiedad es una referencia clave para entender si es una buena oportunidad, ya sea de compra o de venta.
​
## Descripción del problema
​
Se intenta implementar un modelo que permita clasificar el precio de las propiedades en venta, utilizando los datos que se han puesto disposición correspondientes al año 2020.
​
Se realiza la **categorización** de las propiedades entre baratas o caras, considerando como criterio el valor promedio de los precios (la media). 
​
## Entrega
​
Se entrega el código en Jupyter Notebook .ipynb, Incluyendo el EDA, feature engineerging y procesamiento de datos que se consideraron necesario. Se explican claramente cada paso realizado mediante comentarios en el Notebook, 
​
Se envia el repositorio con el proyecto
​
Se generea un archivo .csv sólo con las predicciones, teniendo únicamente **una sola columna** (sin index) llamada 'pred' conteniendo todos los valores de las predicciones, con un valor por fila. 


## Descripción de las dimensiones
- id - Identificador del aviso. No es único: si el aviso es actualizado por la inmobiliaria (nueva versión del aviso) se crea un nuevo registro con la misma id pero distintas fechas: de alta y de baja.
- ad_type - Tipo de aviso (Propiedad, Desarrollo/Proyecto).
- start_date - Fecha de alta del aviso.
- end_date - Fecha de baja del aviso.
- created_on - Fecha de alta de la primera versión del aviso.
- lat - Latitud.
- lon - Longitud.
- l1 - Nivel administrativo 1: país.
- l2 - Nivel administrativo 2: usualmente provincia.
- l3 - Nivel administrativo 3: usualmente ciudad.
- l4 - Nivel administrativo 4: usualmente barrio.
- l5 - Nivel administrativo 5.
- l6 - Nivel administrativo 6.
- rooms - Cantidad de ambientes.
- bedrooms - Cantidad de dormitorios (útil en el resto de los países).
- bathrooms - Cantidad de baños.
- surface_total - Superficie total en m².
- surface_covered - Superficie cubierta en m².
- price - Precio publicado en el anuncio.
- currency - Moneda del precio publicado.
- price_period - Periodo del precio (Diario, Semanal, Mensual)
- title - Título del anuncio.
- description - Descripción del anuncio.
- property_type - Tipo de propiedad (Casa, Departamento, PH).
- operation_type - Tipo de operación (Venta).
- geometry - Puntos geométricos formados por las coordenadas latitud y longitud. 
​

## Metodologia utlizada 
​
- Se Explora el dataset.
- Se aplica un model de K-vecinos despues de probar varias alternativas considerando esta la mejor opción
- Se Busca información sobre la métrica aplicada
- Al tener coordenadas geoespaciales, revisamos que las mismas corresponden en el mapa al lugar que deberían.
- Se crea el archivo con las condiciones requeridas y se envia
