## Observatorio de la evolución de los locales de apuestas en la ciudad de Madrid
En este proyecto voy a analizar la situación actual y las variaciones que se produzcan en el futuro en el número de locales de apuestas en la ciudad de Madrid

La idea para este proyecto surge trás las últimas elecciones municipales de 28 de mayo, en las que uno de los candidatos advertía del peligro de este tipo de establecimientos y su relación con el desarrollo de ludopatía, especialmente en los jóvenes procedentes de familias con rentas bajas.

Más en el mismo sentido: Vázquez-Fernández, M. J., & Barrera-Algarín, E. (2020). El juego on-line en España y las apuestas deportivas: Los jóvenes como nuevos perfiles con ludopatía. Health and Addictions/Salud Y Drogas, 20(2), 61–69. [https://doi.org/10.21134/haaj.v20i2.500](https://doi.org/10.21134/haaj.v20i2.500)

### Situación actual
Voy a utilizar como fuente principal el [repositorio de datos abiertos del ayuntamiento](https://datos.madrid.es/portal/site/egob/), que publica mensualmente un censo de locales, alimentado por las licencias de actividad que la institución concede y el estudio de [Renta Media del INE](https://www.ine.es/uc/jp1AHTuh).

Filtrando por el tipo de licencia y por el estatus de la misma obtenemos que en Junio 2023 hay un total de 374 licencias activas en el municipio para el epígrafe 920002: “JUEGOS DE AZAR Y APUESTAS DE GESTION PRIVADA (BINGOS, CASINOS, MAQUINAS TRAGAPERRAS)”

[![Mapa locales apuestas junio 2023!](./mapa_junio23.png)](https://www.google.com/maps/d/edit?mid=1XRuIM_dxDUN_FDHkY3wOC5iE17RRnOg&usp=sharing)

También voy a utilizar los datos de renta media por unidad de consumo del Instituto Nacional de Estadística (La renta por unidad de consumo se obtiene, para cada hogar, dividiendo los ingresos netos totales del hogar entre el número de unidades de consumo. Se toma la distribución de personas).

#### Conclusiones iniciales

Del filtrado de los datos iniciales, cruzados con la renta media, podemos observar que, efectivamente, el grueso de los locales de apuestas se concentran en lo que podríamos considerar barrios populares, hay una clara relación por la que a menor la renta mayor número de estos locales por barrio.

![Distribución por barrios!](./distri_barrios.png)

En este gráfico de dispersión se cruzan la variable renta media por unidad de consumo con número de locales por barrio, la forma resultante es un tríangulo con el vértice máximo en rentas más bajas decrediente a rentas más altas.

![Distribución por tiers!](./chart.png)

Quizás en este segundo gráfico quede más claro, he agrupado los barrios en 5 tiers iguales y lo que se ve es una distribución por este parámetro.


## Filtrado de los datos
### Herramientas
Acabo de terminar un curso de análisis de datos con Cloudera y me apetecía desarrollar un proyecto con **SQL**, he utilizado este lenguaje para limpiar y preparar los datos y realizar todos los cálculos

El primer mapa está realizado con **Google Maps** a partir de un volcado de SQL

**Google Looker Studio** para el resto de los gráficos
### Metodología
Durante los próximos cuatro años analizaré la variación de los presentes datos, en qué barrios se centra este fenómeno y si efectivamente hay una relación con la renta.
