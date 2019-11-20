# proyecto_modulo2
Proyecto 2
Objetivos específicos:
Investigar los valores accionarios del periodo 2018-2019 de empresas de celulares reconocidas.
Calcular los rendimientos porcentuales de las compañías anteriores.
Predecir precios accionarios del próximo año para cada empresa correspondiente.
Modelo del problema
Para importar los datos historícos se hará uso de una función que extraiga el cúmulo de datos del sitio web "Yahoo Finanzas". Dicha función requerirá los siguientes parámetros:
El nombre del conjunto de acciones (names).
La fecha de inicio de los datos (start).
La fecha de límite de los datos (end).
Al ejecutar dicha función se le agregará el operador ".dropna" para que las filas de valores que serán representados en una tabla de formato pandas no contengan celdas sin valores.
Más tarde, se procesaran los precios mediante una función logarítmica para calcular los rendimientos diarios.
Después se calculará la media y la desviación estandar de los rendimentos obtenidos. Esto se debe a que para calcular los rendimientos futuros por medio de un proceso probabilístico se necesita utilizar la fórmula de la densidad de la distribuición normal, la cual es:
$$1/(\sigma\sqrt(2\pi))\exp(-(x-\mu)^2)/2\sigma^2$$
En donde $\sigma$ representa la varianza, o en nuestro caso la desviación estandar; $\mu$ representa la media muestral y $x$ representa la variable del sistema. En nuestro caso, se contará con cuatro ecuaciones probabilísticas, cada una con sus respectivas desviaciones estandar y medias muestrales. La simbología que se usará sera "std" para la
