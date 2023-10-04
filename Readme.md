
[LogoDataistas](https://github.com/jozzrom/PGH_Googlemaps_Yelp/assets/119060723/eea55756-fa48-4abc-98c8-a86a8b93b286)



Contexto 🌍

La opinión de los usuarios se ha convertido en un dato invaluable en la planificación de estrategias comerciales. Plataformas de reseñas como Yelp y Google Maps proporcionan una gran cantidad de información sobre la percepción de los usuarios respecto a diversos negocios, incluyendo restaurantes, hoteles, esteticas y otros servicios relacionados. Esta retroalimentación es escencial para las empresas, ya que les permite evaluar su desempeño, identificar áreas de mejora y comprender cómo son percibidas por los usuarios. Como parte de una consultora de data, se nos ha contratado para realizar un análisis detallado de la opinión de los usuarios en Yelp y Google Maps sobre negocios relacionados con el cuidado personal y la estética en el mercado estadounidense. El rubro de belleza abarca una amplia gama de servicios y establecimientos relacionados con el cuidado personal y la estética. Algunos ejemplos de negocios dentro de este rubro son los salones de belleza, spas, peluquerías, barberías, salones de uñas, centros de estética, salones de masajes y tiendas de productos de belleza.

Contenidos
Descripción + Objetivo



## Reseñas y Recomendaciones Google Maps - Yelp

![Google_Maps](https://github.com/jozzrom/PGH_Googlemaps_Yelp/assets/119060723/17c7fb14-1793-400e-8ef4-03c3201bb114)

![yelp-logo](https://github.com/jozzrom/PGH_Googlemaps_Yelp/assets/119060723/fff70e2e-d8a4-4590-a902-1f41213a20fe)


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

En el documento [Análisis preliminar_del_dato](https://docs.google.com/spreadsheets/d/1YwkOk_5r0JqUkhL_tp5NHLAcaPJU1YBV/edit#gid=1462331087) anexado en la carpeta “Sprint_1” en Drive podrás encontrar un análisis detallado de cada uno de los datasets ya mencionados, este incluye: 
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
Las actividades realizadas proporcionan una comprensión profunda de la información contenida en el conjunto de datos,tanto para Yelp como para Google Maps, lo que facilita la toma de decisiones informadas y la identificación de patrones valiosos para el proyecto en cuestión.
1. Tipo de dato para cada columna: En esta etapa, se examinan todas las columnas del conjunto de datos para determinar qué tipo de datos contienen. 
2. Número de nulos por columna: Se realiza un conteo de la cantidad de valores faltantes o nulos en cada columna. 
3. Exploración de variables categóricas.
4.Análisis de relaciones: En esta etapa, se investigan las relaciones entre las diferentes variables del conjunto de datos. Esto incluye un análisis de correlación entre variables numéricas.
5. Calificaciones por restaurante: Evaluación del desempeño de cada restaurante. mediante la agrupación de datos por restaurante, cálculo de estadísticas como promedios de calificaciones y la creación de visualizaciones para comparar el rendimiento de los restaurantes.

EDA RESTAURANTES ELEGIDOS: MC Donald’s, KFC, SUBWAY, STARBUCKS, DOMINO’S PIZZA

El análisis de los datos de los restaurantes elegidos nos da un insight más produndo de la situación actual de estos. Las actividades realizadas facilitan la toma de decisiones informadas y la identificación de patrones valiosos para el proyecto en cuestión. Este análisis del dato fue realizado une vez hecho la limpieza y el ordenamiento de los datasets. A continuación se presentan las características que se tomaron en cuenta pata dicha exploración:

1.	Total de Reviews por restaurante: Este punto implica calcular la cantidad total de reseñas u opiniones que ha recibido cada restaurante en el conjunto de datos. Puede ser útil para identificar los restaurantes más y menos comentados.

![Imagen 1_joce](https://github.com/jozzrom/PGH_Googlemaps_Yelp/assets/119060723/cfd6794b-2452-4e8b-a06f-cf99a53fd5ae)

2.	Cantidad de Restaurantes por cadena: En este caso, se realiza un conteo de la cantidad de restaurantes que pertenecen a cada cadena o franquicia presente en el conjunto de datos. Esto proporciona una visión de la distribución de restaurantes entre diferentes cadenas y puede ayudar a identificar cuáles tienen una mayor presencia.

   ![Imagen 2_joce](https://github.com/jozzrom/PGH_Googlemaps_Yelp/assets/119060723/32837c4c-7774-4b97-9552-f0de7730ab7d)

3.	Cantidad de restaurantes por estado: Se realiza un conteo del número de restaurantes por cadena para cada estado.

   ![Imagen 3_Joce](https://github.com/jozzrom/PGH_Googlemaps_Yelp/assets/119060723/0d156b7e-b379-4e86-9dc4-6da096725235)

   4.	Porcentaje de restaurantes para cada cadena: Se calcula el porcentaje que representa cada cadena o franquicia en relación con el total de restaurantes en el conjunto de datos. Ayuda a entender la proporción de restaurantes que pertenecen a cada cadena en el contexto general y es útil para comprender la participación de mercado de cada una.

   <img width="248" alt="Imagen 4_joce" src="https://github.com/jozzrom/PGH_Googlemaps_Yelp/assets/119060723/30db6b63-6100-4798-b8ef-7f53288c0196">

5.	Promedio de Calificaciones por Restaurante y Estado: Esto proporciona información sobre la satisfacción promedio de los clientes en cada estado para cada restaurante individual. Es útil para identificar cómo varía la calidad de los restaurantes según su ubicación.

6.	Promedio de Calificaciones por Restaurante: Gráfico sobre la satisfacción promedio de los clientes para cada restaurante individual. Es útil para identificar cómo varía la calidad de los restaurantes.

<img width="324" alt="Imagen 5_joce" src="https://github.com/jozzrom/PGH_Googlemaps_Yelp/assets/119060723/28c126ed-552f-4a14-a969-3c819c824eac">

7.	Distribución de Calificaciones por Estado y Cadena de Restaurantes: Se examina la distribución de las calificaciones otorgadas por los clientes en relación con el estado en el que se encuentra el restaurante y la cadena a la que pertenece. Esto permite comprender cómo se distribuyen las calificaciones tanto a nivel geográfico como dentro de las diferentes cadenas. Puede ayudar a identificar tendencias regionales y evaluar el desempeño de cada cadena en diferentes ubicaciones.

8.	Relación entre calificaciones y Revisiones por Cadena (sin considerar estado): Este análisis busca examinar la relación entre las calificaciones de los restaurantes y la cantidad de revisiones o reseñas que han recibido, sin tener en cuenta la ubicación geográfica (estado). Esto para ayudar a comprender si la popularidad o la calidad de una cadena influye en la cantidad de reseñas que recibe.

![Imagen 6_joce](https://github.com/jozzrom/PGH_Googlemaps_Yelp/assets/119060723/c0a9a572-b51b-4636-a2a3-6ec3dcc96b4a)


<img width="328" alt="Imagen 17_jocepng" src="https://github.com/jozzrom/PGH_Googlemaps_Yelp/assets/119060723/b6bcee9e-1934-40b8-b372-efd22b77877f">

9.	Porcentaje de Estrellas por cadena: En este punto, se calcula el porcentaje de estrellas otorgadas a cada cadena de restaurantes en relación con el total de estrellas otorgadas en el conjunto de datos. Esto proporciona una visión de cómo se distribuyen las calificaciones por estrellas entre las diferentes cadenas, lo que puede ayudar a identificar cuáles cadenas tienen una mayor proporción de calificaciones positivas o negativas en comparación con otras.

    <img width="442" alt="Imagen 8_joce" src="https://github.com/jozzrom/PGH_Googlemaps_Yelp/assets/119060723/eaa1cf1e-d486-4d20-bec5-16cfd9afe4f0">

---
### Documentación
-Diagrama ER detallado(tablas, PK, FK y tipo de dato)

- Diccionario de datos [Diccionario_Datos
](https://docs.google.com/spreadsheets/d/1ehv-4Jk4Ng3ygzkxJHSPCKgo4I2rHmLj/edit?usp=drive_link&ouid=103990843449218512894&rtpof=true&sd=true)
    
-Workflow detallando tecnologías

---
### Análisis de datos de muestra

El código de los datos de muestra se encuentra alojado en el archivo California.ipynb en el cual se realizó la toma de una porción de los datos de la metadata de Google especificamente para este estado teniendo en cuenta California es conocida por su diversidad cultural y culinaria, lo que ha llevado a la proliferación de una amplia variedad de restaurantes que ofrecen cocinas de todo el mundo. Ciudades como Los Ángeles, San Francisco y San Diego son especialmente conocidas por sus escenas culinarias vibrantes y diversificadas.

Además, California es un importante productor de alimentos en los Estados Unidos, lo que significa que muchos restaurantes en el estado tienen acceso a ingredientes frescos y de alta calidad. 

## Outliers

![Outliers](https://github.com/jozzrom/PGH_Googlemaps_Yelp/assets/119060723/cc934181-da8d-4b2d-959a-c328a058ccff)

Podemos evidenciar que el conjunto de datos de Calificación Promedio y el Número de Reseñas se encuentra dentro del rango de 0 a 200 reseñas. Sin embargo llama la atención un punto de datos que alcanza el número de reseñas de los 600 y ubicandose dentro del rango de 4,5 y 5.0 en calificación. 

Se debe tener en cuenta que el Dataframe contiene de datos para todo tipo de de cadenas de restaurantes ubicados en estado de california por lo que es posible que este outlier se refiera a una cadena de restaurantes que tiene alta presencia de locales físicos en el estado.
Este punto lo estaremos identificando en los siguientes pasos.

![histograma](https://github.com/jozzrom/PGH_Googlemaps_Yelp/assets/119060723/88ca2785-1039-4804-af51-cebab04341c3)

Modalidad (Moda): La moda en el conjunto de datos es 5, lo que significa que 5 es la calificación más frecuente y, por lo tanto, la más común.

Sesgo a la Izquierda: La distribución muestra un sesgo hacia valores más bajos (4, 3, 2 y 1), lo que indica que la mayoría de las calificaciones tienden a estar por debajo de la calificación máxima de 5.

Tendencia Central: Aunque 5 es la moda (el valor más común), la mediana (valor en el medio cuando los valores están ordenados) podría ser menor que 5 debido al sesgo hacia valores más bajos. La mediana divide la distribución en dos mitades iguales.

En resumen, los datos tienen una distribución de calificaciones sesgada hacia valores más bajos, con 5 como la calificación más común. Esta información puede ser valiosa para comprender la satisfacción o la calidad de los elementos calificados en el conjunto de datos.

![correlacion](https://github.com/jozzrom/PGH_Googlemaps_Yelp/assets/119060723/76a033c4-8a78-4603-9653-8e734bdd0ef0)

Con la gráfica de correlación podemos identificar la relación entre las variables númericas del Dataframe, teniendo como resultado una correlación positiva entre el rating y el average rating. 
Mientras que se identifcan correlaciones negativas entre en el número de reviews y el promedio de calificación (avg_rating) lo cual nos indica que no necesariamente porque se tenga mas número de reviews se puedan llegar a tener reviews positivos.

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

- Se debe incrementar las reseñas positivas que tiene KFC ya que es una oportunidad de mejora para su posicionamiento en el mercado y ser atractivo para los consumidores.









