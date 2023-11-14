# Complejidad Económica

Desarrollo de cálculos varios de complejidad económica.


### Metodología

La metodología de este código sigue de cerca la metodolodía de complejidad económica desarrollada en la sección 3 del paper:

- [_Economic complexity and the green economy_](https://doi.org/10.1016/j.respol.2020.103948), Penny Mealy and Alexander Teytelboym, Research Policy (2022)


Cuando nos apartamos de esta metodología lo indicamos en el código, y en los casos correspondientes seguimos de cerca la metodología propuesta en:

- [The Atlas of Economic Complexity_](https://direct.mit.edu/books/oa-monograph/3014/The-Atlas-of-Economic-ComplexityMapping-Paths-to), Ricardo Hausmann, César A. Hidalgo, Sebastián Bustos, Michele Coscia, Alexander Simoes, Muhammed A. Yildirim (2014)

- [_The Product Space Conditions the Development of Nations_](https://arxiv.org/ftp/arxiv/papers/0708/0708.2090.pdf), Hidalgo, C. A., Klinger, B., Barabási, A. L., & Hausmann, R. (2007) (2007)


### Uso y descripción del código

El código debe correrse en el orden puesto en el nombre de cada _notebook_:

[`1_preprocesa_y_calcula_RCA`](https://github.com/TuQmano/complejidad-economica/blob/main/1_preprocesa_y_calcula_RCA.ipynb): Preprocesa, filtra, y ordena los datos. Para finalizar, guarda las matrices de RCA y Mcp, y el orden de los índices de productos y paises (locations).

[`2_calcula_eci_pci_proximity_density_desde_Mcp`](https://github.com/TuQmano/complejidad-economica/blob/main/2_calcula_eci_pci_proximity_density_desde_Mcp.ipynb): Siguiendo el paper de Mealy, hace el cálculo de ECI, PCI, proximidad y densidad a partir de la matriz Mcp.

[`3_calcula_indices_de_paises`](https://github.com/TuQmano/complejidad-economica/blob/main/3_calcula_indices_de_paises.ipynb): Calcula el resto de los índices para cada país: GCI, GCP, COI. Devuelve un dataframe que incluye estos índices para cada país, y sus rankings.

[`4_calcula_info_productos_y_grafos`](https://github.com/TuQmano/complejidad-economica/blob/main/4_calcula_info_productos_y_grafos.ipynb): Calcula índices para combinación de país&productos: COG. Plotea los gráficos de proximidad de productos junto con información relevante para Argentina. Luego arma los dataframes de productos con información para países que se deseen (por default para Argentina), y grafica los histogramas de distribución de PCIs. Finalmente grafica una matriz de proximidad entre países regionales (LATAM) contra una lista predefinida de países desarrollados.
