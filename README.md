# Proyecto-Integrador
Este repositorio contiene el desarrollo y los resultados del proyecto integrador para el semestre 2019-02 de la Maestria en ciencia de los datos y analítica de la universidad EAFIT.

Los estudiantes que presentan este trabajo son:

**1. Jesus Alberto Arcia**

**2. Jorge Luis Renteria**

**3. Edgar Leandro Jiménez**

## Resumén


## Descripción del problema - Contexto 

El estudio del Social Media Data Mining y el estudio de comunidades ha venido tomando cada vez más fuerza gracias a la creciente cantidad de datos que hay en internet y la cantidad de usuarios que interactúan en ella día a día. 

Por medio del Social Data Mining se abordan varios conceptos importantes hoy por hoy para las organizaciones, como lo son la publicidad y el marketing, donde por medio minería de datos a estas plataformas puede ser de gran ayuda para determinar que estrategia de publicidad funciona mejor para los usuarios y asegurarse que el público objetivo esté satisfecho, otro concepto es La lealtad de marca, por medio del constante monitoreo a las plataformas de la compañía, esta brinda a sus usuarios y clientes una sensación de ser escuchado y entendido, lo cual es un factor importante que permite la construcción de una base sólida de clientes leales y satisfechos, otro concepto es el desarrollo de productos, donde el negocio podrá hacer frente al ritmo cambiante de los usuarios hacia otros productos  u marcar de manera rápida mediante el desarrollo de nuevos productos o servicios que permitan capturar más audiencia o consolidar la que tiene. Por otra parte, el concepto de comunicación, a través de la minería de datos se pueden acercar más a los clientes y los proveedores del negocio, monitoreando las redes sociales en busca de clientes insatisfechos o que no han sido atendidos de manera satisfactoria y dirigir la fuerza de atención al servicio hacia estas personas, logrando una mejor comunicación entre el negocio y sus stakeholders. (Dataworks, 2018) 

Es así como en este trabajo se abordan los conceptos del Social Media Data Mining y el estudio de comunidades.  En primer lugar, por medio del estudio y procesamiento del lenguaje natural en las redes sociales, particularmente en Twitter. Esta red que fue creada en el 2006 inicialmente solo permitía escribir hasta 180 caracteres, hoy en día es permitido hasta 280 caracteres. Esta particularidad de restricción en la extensión de la escritura hace que los usuarios sinteticen sus ideas y utilicen un lenguaje más compacto para poder comunicarse con los otros usuarios. Twitter se encuentra presenten en los cinco continentes y tienen millones de usuarios que día a día comparten sus ideas, proyectos, pensamientos, criticas, entre otros frente a un tema particular o una marca. 


## Metodología  

La normalización del proceso de hallar conocimiento en los datos ha convocado esfuerzo desde finales de los años 90, durante este tiempo se han planteado metodologías que buscan alinear la ejecución de los proyectos analíticos con los objetivos del negocio sin descuidar los elementos técnicos que deben tenerse en cuenta. Dentro de esas metodologías se encuentra ASUM – DM planteada por IBM la cuál por medio de cinco categorías busca abordar de manera holística la salida a producción de un sistema analítico partiendo desde la necesidad del negocio. 


## Entendimiento del negocio 

En un ambiente de competencia abierta y mercados dinámicos estar a la vanguardia de las tendencias que rigen el mercado es una obligación para todas aquellas empresas que buscan sobrevivir, por ellos, conocer a sus clientes de manera integral, sus sentimientos y las comunidades con quienes interactúan son herramientas útiles de decisión para las marcas, esto junto con el uso masivo que han obtenido actualmente las redes sociales para expresar opiniones y sensaciones hacia una empresa llevan a que redes sociales como Twitter deban ser analizadas empleando métodos analíticos que permitan conocer constantemente la opinión que tienen las personas sobre una marca específica y el impacto que tiene el punto de vista de su comunidad digital sobre su opinión virtual. 

## Acercamiento analítico 

Es necesario implementar un modelo analítico tal que posterior a su entrenamiento se logre asignar un grado de “positividad” o “negatividad” a un usuario con base a la información publicada en Twitter, además, basados en la misma fuente construir clusters de relaciones que indiquen con quienes interactúa en el día a día. 

### Datos necesarios 

Para desarrollar el modelo, es necesario tener fuentes integrales que conecten de principio a fin la opinión virtual de un usuario con sus partes relacionadas. Para esto, se requiere: 

1. Tweets -> Dataframe “limpio” con información de los últimos tweets publicados haciendo referencia a la marca. 

2. Listado de seguidores -> Número de personas que siguen a la persona que publico el Tweet. 

3. Listado de seguidos -> Nùmero de personas que sigue la persona que publico el Tweet. 

4. Conjunto de palabras positivas y negativas -> Listado de palabras categorizadas por su grado de “positividad” o “negatividad” 

5. Ubicación de la persona -> Ubicación que figura en la pagina principal de la persona que publicó el tweet.


## Captura de datos 

Para obtener la información de Tweets se utilizará el servicio expuesto por Twitter inc. (https://developer.twitter.com/) utilizando el lenguaje de programación Python. De esta misma fuente es posible capturar el listado de seguidores y seguidos de quien publicó el tweet. 

Por otro lado, para nutrir el conjunto de palabras positivas y negativas se obtendrá información de primer nivel y segundo nivel, esto quiere decir que se hará uso de servicios de terceros (API de Azure como ejemplo) para categorizar los sentimientos de una palabra y también se crearán encuestas para ser diligenciadas por personas dispuestas a identificar que tan positivo o negativo es un mensaje.
