# Complejidad Económica

[![](https://fund.ar/wp-content/uploads/2021/09/DesarrolloVerde2.jpg)](https://www.fund.ar/wp-content/uploads/2021/09/El-Potencial-Productivo-Verde-de-la-Argentina.pdf)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%20NC%20SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.13931731.svg)](https://zenodo.org/doi/10.5281/zenodo.13931731)

### Fundar + _El Gato y La Caja_

_Una agenda para el crecimiento verde en la Argentina precisa identificar hacia qué sectores y productos deben dirigirse las decisiones de política pública: el análisis basado en los conceptos de complejidad económica y espacio de productos es una herramienta capaz de ofrecer respuestas a esa necesidad, a partir del uso de evidencia cuantitativa_. 

Este repositorio, que incluye cálculos varios de complejidad económica, forma parte del proyecto **Complejidad Económica Verde** desarrollado por las áreas de [Datos](https://fund.ar/area/datos/) y [Politica Productiva](https://fund.ar/area/politica-productiva/) de [Fundar](https://fund.ar/). 

El [proyecto digital](https://complejidadeconomicaverde.fund.ar/sobre-el-proyecto/), diseñado en colaboración con [El Gato y La Caja](https://elgatoylacaja.com/), es una puerta de acceso para que la mayor cantidad de personas puedan conocer el marco teórico y las posibilidades materiales de esa propuesta. 


## Metodología

Este código sigue de cerca la metodología de complejidad económica desarrollada en la sección 3 del paper:

- [Economic complexity and the green economy_](https://doi.org/10.1016/j.respol.2020.103948), Penny Mealy and Alexander Teytelboym, Research Policy (2022)

Cuando nos apartamos de esta metodología lo indicamos en el código, y en los casos correspondientes seguimos de cerca la metodología propuesta en:

- [The Atlas of Economic Complexity_](https://direct.mit.edu/books/oa-monograph/3014/The-Atlas-of-Economic-ComplexityMapping-Paths-to), Ricardo Hausmann, César A. Hidalgo, Sebastián Bustos, Michele Coscia, Alexander Simoes, Muhammed A. Yildirim (2014)

- [_The Product Space Conditions the Development of Nations_](https://arxiv.org/ftp/arxiv/papers/0708/0708.2090.pdf), Hidalgo, C. A., Klinger, B., Barabási, A. L., & Hausmann, R. (2007) 


## Uso y descripción del código

El código debe correrse en el orden puesto en el nombre de cada _notebook_:

[`1_preprocesa_y_calcula_RCA`](https://github.com/TuQmano/complejidad-economica/blob/main/1_preprocesa_y_calcula_RCA.ipynb): Preprocesa, filtra, y ordena los datos. Para finalizar, guarda las matrices de RCA y Mcp, y el orden de los índices de productos y paises (locations).

[`2_calcula_eci_pci_proximity_density_desde_Mcp`](https://github.com/TuQmano/complejidad-economica/blob/main/2_calcula_eci_pci_proximity_density_desde_Mcp.ipynb): Siguiendo el paper de Mealy, hace el cálculo de ECI, PCI, proximidad y densidad a partir de la matriz Mcp.

[`3_calcula_indices_de_paises`](https://github.com/TuQmano/complejidad-economica/blob/main/3_calcula_indices_de_paises.ipynb): Calcula el resto de los índices para cada país: GCI, GCP, COI. Devuelve un dataframe que incluye estos índices para cada país, y sus rankings.

[`4_calcula_info_productos_y_grafos`](https://github.com/TuQmano/complejidad-economica/blob/main/4_calcula_info_productos_y_grafos.ipynb): Calcula índices para combinación de país&productos: COG. Plotea los gráficos de proximidad de productos junto con información relevante para Argentina. Luego arma los dataframes de productos con información para países que se deseen (por default para Argentina), y grafica los histogramas de distribución de PCIs. Finalmente grafica una matriz de proximidad entre países regionales (LATAM) contra una lista predefinida de países desarrollados.

## El potencial productivo verde de la Argentina - Evidencias y propuestas para una política de desarrollo

1. [Documento Técnico](https://www.fund.ar/wp-content/uploads/2021/09/El-Potencial-Productivo-Verde-de-la-Argentina.pdf)
2. [Policy brief](https://www.fund.ar/wp-content/uploads/2021/09/El-Potencial-Productivo-Verde-de-la-Argentina_PB.pdf)  
3. [Micrositio](https://complejidadeconomicaverde.fund.ar/)
4. [Glosario](https://fund.ar/publicacion/glosario-ppv/)


## Relacionado

1. [**Panorama de la Complejidad Económica de la Provincia de Córdoba**](https://fund.ar/wp-content/uploads/2023/04/Fundar_Panorama_Complejidad_Economica_Cordoba-1.pdf). Feole, M.; Gutman, M.; Lema Cuesta, C.; y Pezzarini, L. (2023)
2. [**Panorama de la Complejidad Económica del Municipio de Córdoba**](https://fund.ar/wp-content/uploads/2023/05/Fundar_Panorama_Complejidad_Economica_Municipio_Cordoba-2.pdf)  . Luvini, P.; Martin, R.; Cejas, C. y Sbodio, J. M. (2023)



---
<div>&nbsp;</div>
<div>&nbsp;</div>
<div>
  &nbsp;
  <a href="https://fund.ar">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github.com/datos-Fundar/fundartools/assets/86327859/6ef27bf9-141f-4537-9d78-e16b80196959">
    <source media="(prefers-color-scheme: light)" srcset="https://github.com/datos-Fundar/fundartools/assets/86327859/aa8e7c72-4fad-403a-a8b9-739724b4c533">
    <img src="fund.ar"></img>
  </picture>
</a>
</div>

