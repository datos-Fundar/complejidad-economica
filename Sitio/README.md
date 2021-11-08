## Sitio complejidadeconomicaverde.fund.ar

### definiciones_acronimos.csv
La totalidad de los acronimos utilizados en el sitio se encuentran en español, pero la mayoría de los archivos presentes en este repositorio utilizan los acronimos en inglés. Por lo que en este archivo se encuentran las definiciones en ambos idiomas.

### country_complexity_rank.csv
Datos de la OMC procesados por Fundar.
Se utiliza para el ranking de complejidad de paises, presente en [La Teoria](http://complejidadeconomicaverde.fund.ar/la-teoria/)

### country_complexity_rank_future.csv
Datos procesados por Fundar.
Se utiliza para el ranking de complejidad potencial, presente en [El Pasado](http://complejidadeconomicaverde.fund.ar/el-pasado/)

### country_strategies.csv
Datos procesados por Fundar.
Se utiliza para el scatter plot de estrategias de paises, presente en [El Pasado](http://complejidadeconomicaverde.fund.ar/el-pasado/)

### hist_productos_2014_2018.csv
Datos procesados por Fundar.
Se utiliza para el histograma de productos verdes, presente en [El Pasado](http://complejidadeconomicaverde.fund.ar/el-pasado/)

### green_products.ipynb
Archivos Inputs: 
- DESCRIPCION PARTIDAS Y SUBPARTIDAS - SUBPARTIDAS (6 DIGITOS).csv (Nombres de los productos en español, de la dirección de Aduanas)
- informacion_nodos_2014_2018.csv (Promedio de datos de la OMC, de 2014 a 2018, procesados por Fundar)
- Tabla 30 Productos.csv (Datos de Fundar)
- servicios.csv (generado por environmental_services.ipynb)

Archivo Output: 
- green_products.csv

El archivo output se utiliza: 
- En los Scatter Plots de [El Pasado](http://complejidadeconomicaverde.fund.ar/el-pasado/)
- En el Grafo, Scatter Plot y Tabla de [Un Plan](http://complejidadeconomicaverde.fund.ar/un-plan/)
- En el Grafo, Scatter Plot y Tabla de [Destinos Posibles](https://complejidadeconomicaverde.fund.ar/destinos-posibles)

### environmental_services.ipynb

Archivo Input:
- servicios_ambientales_sin_procesar.csv (Datos de la WTO, APEC y OECD sobre funciones ambientales de los productos)

Archivo Output: 
- servicios.csv

El archivo output se utiliza: 
- Dentro de green_products.ipynb

### green_products_edges.ipynb

Archivos Input:
- grafo_conexiones_pesos_2014_2018.pkl (tiene la relación entre dos productos con su peso)
- green_products_2014_2018.pkl (se usa para tener los códigos de producto)

Archivos Output:
- green_products_edges.csv (es un csv con todas las aristas del grafo relacionando dos productos (su código) y un peso).

Se utiliza para todos los grafos de la página.
