# Análisis de la Población Mundial, Mortalidad Infantil y Esperanza de Vida

En él informe primer Población Mundial, se cargan 3 archivos .xlsx

-**Population**, contiene un listado de países y cantidad de habitantes.
-**Countries**, contiene listado de países, código del país y su respectivo continente.
-**Países**, es el símil de Countries pero en español.
Al querer trabajar los datos en idioma español, se ocultan todos los datos que no se van a utilizar, en este caso la tabla Countries y la columna Country de la tabla Population.

En el segundo Mortalidad y Esperanza de Vida, se cargan 2 archivos .xlsx adicionales

Infant+death+rate, contiene un listado de países y el promedio de muertes infantiles por cada 1000 decesos.
Life+expectancy, contiene un listado de países y el promedio de esperanza de vida.

En el modelo de datos se generan las siguientes relaciones:

![1-poblacion](https://github.com/user-attachments/assets/2af16a5a-c6dd-4775-b36e-36031e3865af)

# Informe Población Mundial

Un Treemap con la cantidad de habitantes por país
Una Matriz donde podemos ver el detalle de habitantes por continente y país
Un Mapa donde se puede observar la distribución de países por continente, las burbujas están condicionas al tamaño de la población de cada país
Adicional al filtro segmentado la cantidad de habitantes se agregó uno por continente.


![2-poblacion](https://github.com/user-attachments/assets/b33e2ca6-dc84-470d-bb42-bbf36c533a05)

# En Power Query se genera una columna condicional para segmentar los países en 4 categorías:

0 - 1M
1M - 10M
10M - 100M
100M >

Con esta segmetación se agrega un filtro.

![3-Poblacion](https://github.com/user-attachments/assets/c385385d-eb60-40e0-839d-46fa25424959)

# Informe Mortalidad Infantil y Esperanza de Vida

Una Matriz donde podemos ver el detalle de habitantes por continente y país, promedio de Esperenza de Vida y promedio de Mortalidad Infantil
Gráfico de dispersión, estudiando la relación entre la esperanza de vida y la mortalidad infantil
Un Mapa donde se puede observar la distribución de países por continente, las burbujas están condicionas al tamaño de la Mortalidad Infantil.

![4-Poblacion](https://github.com/user-attachments/assets/3ee19d15-2b9b-4c81-bb36-cbbf95dd37e1)

# En Power Query se genera una columna condicional en cada tabla para segmentar:

# Mortalidad Infantil
0 a 10
10 a 25
25 0 50
50 >

![5-Poblacion](https://github.com/user-attachments/assets/e6d92255-3d0b-40b8-a17c-668488611883)

# Esperanza de Vida
0 a 60
60 a 70
70 a 80
80 >

![6-Poblacion](https://github.com/user-attachments/assets/8c63a90f-4aae-4701-b7c5-7df98c5d6bbf)

Estos dos segmetaciones se usan como filtro sumadas a los dos anteriores.

# Algunas conclusiones que se pueden sacar de este informe.

A menor esperanza de vida mayor es la mortalidad infantil, siendo el continente africano el más afectado por esta tendencia.
Angola representa el país más afectado ya que su esperanza de vida promedio es de 56 años y una mortalidad infantil de 191 por cada 1000 decesos.
El país menos afectado en Mónaco perteneciente al continente Europeo con una esperanza de vida promedio de 89 años y una mortalidad infantil de 5 por cada 1000 decesos.





