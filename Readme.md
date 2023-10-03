
## ***__Proyecto Grupal__***

## Sprint # 1 Puesta en marcha del proyecto y Trabajo con Datos


## Reseñas y Recomendaciones Google Maps - Yelp

![Google_Maps](https://github.com/jozzrom/PGH_Googlemaps_Yelp/assets/119060723/17c7fb14-1793-400e-8ef4-03c3201bb114)

![yelp-logo](https://github.com/jozzrom/PGH_Googlemaps_Yelp/assets/119060723/fff70e2e-d8a4-4590-a902-1f41213a20fe)

## Nombre de la Empresa



![LogoDataistas](https://github.com/jozzrom/PGH_Googlemaps_Yelp/assets/119060723/eea55756-fa48-4abc-98c8-a86a8b93b286)

## Distribución de Roles
|Integrante|Rol|
|:-----:|:---:|
|Jorge Gómez | Data Analyst|
|Federico Gravina | Data Engineer|
Tinmar Andrade | Data Engineer|
Fanny Fitz |Data Scientist
Jocelyn Romano | Data Scientist

---

## **Planteamiento del problema**

----

El problema que abordaremos en este proyecto se relaciona con la necesidad de mejorar la visibilidad y el impacto del negocio de nuestro cliente, que opera el restaurante "KFC" en el estado de Georgia en Estados Unidos. 

Actualmente, el restaurante “KFC” desconoce la opinión general que tiene el público de la calidad de sus servicios. 

Además, la influencia de las reseñas en plataformas como Yelp en las decisiones de los consumidores se ha vuelto cada vez más importante.

La falta de una estrategia sólida de gestión de la reputación en línea y la insuficiente atención a las opiniones de los clientes pueden estar afectando negativamente la percepción del restaurante y su capacidad para atraer nuevos clientes.

---

## **Alcance del proyecto**

---
El proyecto se enfocará en restaurantes de la cadena “KFC” ubicados en las ciudades de California, Nueva York, Colorado, Texas y Georgia, dentro de los Estados Unidos. 

De igual forma se incluirán los datos de la cadena Domino 's Pizza, McDonald's, Subway, Pizza Hut  y afines localizados en los estados ya mencionados. 

Identificación de oportunidades de mejora en estados más turísticos de Estados Unidos (California, New York, Colorado, Texas y Georgia)
Análisis exhaustivo de la industria gastronómica integrando las reseñas de Google Maps y Yelp
Enfoque: _Proporcionar recomendaciones informadas y estratégicas para la toma de decisiones_

---

## **Obejtivo General**

<img width="1356" alt="Objetivo General" src="https://github.com/jozzrom/PGH_Googlemaps_Yelp/assets/119060723/0bb3608d-2ad1-4bc2-8b1f-01e1b6a45141">

---

Mejorar el posicionamiento global de los locales de la compañía KFC con respecto a sus competidores directos en los estados de Estados Unidos ubicados en  California, Nueva York, Colorado, Texas y Georgia. 

La selección de dichos estados se basa en un relevamiento de datos, que nos lleva a observar la representatividad de la muestra para luego pensar en un modelo exponencial al resto del país. Sus características diferentes en cuanto a ubicación geográfica, turismo recibido tanto interno como externo así como la diferencia del tipo de  población también nos permiten tener un mejor entendimiento de la problemática general, así como nos proporciona una mayor capacidad para realizar recomendaciones a nuestro cliente. 

Con el desarrollo del proyecto y el modelo, sería posible, en un futuro, ampliar los alcances a todo el país y también al resto de los países en donde se encuentre ubicada la cadena de comida. 

____

## **Objetivos Específicos**

---
Se recopilará información como reseñas y calificaciones provenientes de plataformas como Maps y Yelp.
Garantizar la disponibilidad de datos limpios y estructurados.

Se realizará un análisis de sentimiento sobre las reseñas de Google Maps y Yelp, esto con el fin de entender la percepción que tienen los clientes sobre el servicio en dichos restaurantes. 

_Con los resultados obtenidos se realizará una comparativa entre nuestro cliente KFC contra sus demás sucursales ubicadas en los estados ya mencionados_. 
Se comparará el desempeño entre las cadenas KFC vs su competencia a través de locales afines y el análisis de  información proveniente de las plataformas ya mencionadas. 

Crear una interfaz interactiva que visualice y explore los resultados del análisis.

---
## **Análisis Preliminar del Dato**
Se realizó un análisis preliminar de los dataset: 

Yelp:

-Business.plk

-Checkin.json

-Tip.json

-Review.json

-User.parquet

Google Maps:

-Metadata.json

-Reviews por estado.json

En el documento [analisis_preliminar_del_dato](https://docs.google.com/spreadsheets/d/1YwkOk_5r0JqUkhL_tp5NHLAcaPJU1YBV/edit#gid=1462331087) anexado en la carpeta “Sprint_1” en Drive podrás encontrar un análisis detallado de cada uno de los datasets ya mencionados, este incluye: 
- descripción general del archivo
- nombre de cada columna, tipo de dato de cada columna
- descripción de cada columna, cantidad de datos, tipo de archivo,cantidad de nulos.

De los datasets de Yelp, se plantea utilizar el archivo Business.plk,  ya que contiene información de los establecimientos,  review.json y tip.json porque contiene los reviews de cada establecimiento. 

De los datasets de Google Maps se utilizarán los archivos metadata.json y los archivos de las carpetas California, New York, Colorado, Texas y Georgia que contiene las review por estado.

-----

## **Análisis Stack Tecnológico**


<img width="1419" alt="Stack Tecnologico" src="https://github.com/jozzrom/PGH_Googlemaps_Yelp/assets/119060723/a5c4d483-1e48-4756-a9ce-955db466348a">
___

## **KPI’s**

---

*KPI 1*: _Realizar un análisis exploratorio de los datos para comparar el rendimiento en cantidad de locales, así como en promedio de estrellas recibidas, calificación general de la cadena KFC, con respecto a sus principales competidores, a saber: Subway, MacDonald´s, Domino´s Pizza y Pizza Hut._


### Promedio de estrellas para Yelp

|Compañía| Promedio Estrellas|
|:--------|:----:|
Subway|   2.6
Domino´s Pizza| 2.28
Pizza hut| 2.03
Mc Donald´s | 1.86
KFC| 1.86


### Número de locales para Yelp

|Compañía| Locales|
|:--------|:--------:|
Mc Donald´s | 703
Subway | 459
Domino´s Pizza| 295
Pizza Hut | 272
KFC | 171


---

*KPI 2*: _Mejorar para un périodo de 3 meses un porcentaje significativo, la cantidad de reseñas positivas en los estados seleccionados a través de un análisis de sentimientos de los datos provenientes de las fuentes Google Maps y Yelp._

Para lograr este objetivo se realizará un proceso de Machine Learning que permita recibir nuevos datos. 

---

*KPI 3*:  _Hacer un análisis exhaustivo de los datos de las fuentes citadas para aumentar la cantidad de reseñas recibidas para la cadena KFC enfocados en recomendaciones de mejoras en los rubros que poseen malas calificaciones_(por ejemplo: calidad de las comidas, limpieza de los locales, rapidez del servicio, etc.)

### Cantidad de Reseñas

|Compañía| Locales|
|:--------|:-------:|
|McDonald's |17359|
|Domino's Pizza |6291|
|Pizza Hut| 17359|
|Subway| 4588|
|KFC| 2923|


---

## **Diagrama de Gantt para Sprint #1**

A continuación se muestra la distribución de los tiempos que se le destinaron para cada una de las tareas establecidas


---

## Repositorio Git 
![Logo github](https://github.com/jozzrom/PGH_Googlemaps_Yelp/assets/119060723/4bee878e-bcfb-4fbc-abc9-083b17d1abaf)

[Repositorio Github]()

---

### Sprint 2 Data Engineering

---

### ETL ![ETL](https://github.com/jozzrom/PGH_Googlemaps_Yelp/assets/119060723/393f5fd1-1eb0-4094-bace-0320058f4e6f)


A continuación, se enlistan las actividades o procedimientos realizados que constituyen la etapa de Limpieza y Transformación de Datos.

1.	Eliminación de Valores Nulos en la Columna de Review de Usuario: En la primera etapa de limpieza de datos, se procedió a eliminar los valores nulos que se encontraban en la columna de "review de usuario". Esto se hizo para asegurar la integridad de los datos y evitar problemas futuros en el análisis
.
2.	Eliminación de Columnas con Altos Porcentajes de Nulos: Después de una revisión exhaustiva de los datos de Google Maps, se identificó que las columnas "pics" y "resp" contenían más del 80% de valores nulos. En consecuencia, se tomó la decisión de eliminar estas dos columnas, ya que su contribución al análisis era limitada debido a la falta de datos significativos.

3.	Conversión de la Columna 'time' en Formato de Fecha: Para facilitar el análisis temporal de las revisiones de los usuarios, se realizó la conversión de la columna 'time' al formato de fecha. Posteriormente, se crearon tres nuevas columnas que contenían la información del año, mes y día en que se registró la revisión del usuario.

4.	Selección de Datos para el Período de 2017 a 2021: Se procedió a seleccionar las reviwx de usuarios que estuvieran registradas en el período comprendido entre los años 2017 y 2021. Esto permitió enfocar el análisis en un rango de tiempo específico.

5.	Verificación de Duplicados y Eliminación: Se llevó a cabo una verificación exhaustiva de duplicados en los datos y se procedió a eliminarlos. Esto aseguró que cada revisión de usuario fuera única en el conjunto de datos.

Procesamiento de Texto en la Columna de Revisión de Usuario:
6.	Conversión del Texto a Minúsculas: Para homogeneizar el texto y facilitar el análisis de texto, se realizó la conversión de reviews a minúsculas.
7.	Eliminación de Emojis Utilizando la Librería "Demoji": Se implementó la librería "Demoji" para eliminar los emojis contenidos en el texto de las revisiones de usuario. Esto contribuyó a una limpieza adicional del contenido de texto.
8.	Verificación y Traducción a Inglés: Se verificó que todas las revisiones de usuario estuvieran en inglés. Aquellas revisiones que no estaban en este idioma fueron traducidas al inglés para mantener la consistencia en el análisis de texto.
9.	Eliminación de Signos de Puntuación: Por último, se procedió a eliminar los signos de puntuación contenidos en el texto de las revisiones de usuario. Esto simplificó el análisis de texto y facilitó la extracción de información relevante.

Estas etapas de limpieza y transformación de datos fueron esenciales para preparar los datos de manera adecuada y asegurar que estuvieran listos para el análisis posterior. La uniformidad de los datos fue mejorada significativamente a lo largo de este proceso.
![image](https://github.com/jozzrom/PGH_Googlemaps_Yelp/assets/119060723/e5261f27-8e49-4fc0-9275-9480a15f5e3e)

---
### Estructura de datos implementados (DW, DL, etc)
---
### Pipeline ETL automatizado
---
### Diseño del modelo ER
---
### Pipelines para alimentar el DW
---
### Automatización
---
### Validación de datos
---
### Documentación
    -Diagrama ER detallado(tablas, PK, FK y tipo de dato)
    -Diccionario de datos
    -Workflow detallando tecnologías
---
### Análisis de datos de muestra


---
### MVP/Proof of Concept de Dashboard

![MVP_Dashboard](https://github.com/jozzrom/PGH_Googlemaps_Yelp/assets/119060723/a5109ec9-142c-4e89-83c3-77f8329ef540)


Para el segundo sprint se avanzó en la estructuración gráfica del Dashboard del MVP a partir de los datos para el estado de California teniendo en cuenta que de los cinco estados seleccionados es el que cuenta con mayor porción de población comparado con los otros cuatro estados. 

El dasboard entonces se construyó con a partir de estos datos y luego de realizar la limpieza y transformación de los mismos, teniendo tres objetivos fundamentales.

1. Identificar la dimensionalidad del mercado de los restaurantes en el estado de California.
2. Revisar la evolución de las reseñas tanto para nuestro cliente KFC como para los competidores que venimos evaluando.
3. Establecer el posicionamiento de KFC en los consumidores a partir del análisis de sentimientos en las reviews realizadas.



## Primeras conclusiones Dashboard

- A partir del año 2018 el número de reviews para nuestro cliente KFC ha presentado una notable disminución comparado con su compentencia quienes han mantenido estables su número de reseñas

- A partir de la muestra y comparado con su competencia KFC se encuentra en un promedio de Rating por debajo de las marcas Domino´s, Subway y Mc Donalds teniendo como un 63% de reseñas negativas.

- Las reseñas negativas para KFC, a partir del análisis de sentimientos realizado se fundamentan principalmente en el precio y la comida, es decir que la percepción del precio versus la comida es observada por los consumidores como negativa.









