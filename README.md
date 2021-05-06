# Complejidad Económica

Desarrollo de cálculos varios de complejidad económica.

La metodología de este código sigue de cerca la metodolodía de complejidad económica desarrollada en la sección 3 del paper:

Economic complexity and the green economy, Penny Mealy and Alexander Teytelboym, Research Policy, https://doi.org/10.1016/j.respol.2020.103948

Cuando nos apartamos de esta metodología lo indicamos en el código, y en los casos correspondientes seguimos de cerca la metodología propuesta en:

The Atlas of Economic Complexity, Hausmann et al (2014)
The Product Space Conditions the Development of Nations, Hidalgo et al (2007)


El código debe correrse en el orden puesto en el nombre de cada notebook:

1_preprocesa_y_calcula_RCA: Preprocesa, filtra, y ordena los datos. Para finalizar, guarda las matrices de RCA y Mcp, y el orden de los índices de productos y paises (locations).

2_calcula_eci_pci_proximity_density_desde_Mcp: Siguiendo el paper de Mealy, hace el cálculo de ECI, PCI, proximidad y densidad a partir de la matriz Mcp.

3_calcula_indices_de_paises: Calcula el resto de los índices para cada país: GCI, GCP, COI. Devuelve un dataframe que incluye estos índices para cada país, y sus rankings.

4_calcula_info_productos_y_grafos: Calcula índices para combinación de país&productos: COG. Plotea los gráficos de proximidad de productos junto con información relevante para Argentina. Luego arma los dataframes de productos con información para países que se deseen (por default para Argentina), y grafica los histogramas de distribución de PCIs. Finalmente grafica una matriz de proximidad entre países regionales (LATAM) contra una lista predefinida de países desarrollados.