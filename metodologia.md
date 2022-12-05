# Metodología

**Periodismo de Datos II:** Herramientas Digitales para la Visualización y Presentacion de Datos

Durante la clase de **Periodismo de Datos II** hemos podido reconocer diferentes métodos con los que es posible acercarse a nuevos niveles de la informática con los que es posible acceder a herramientas digitales de desarrollo web y de visualización de datos. 

Con lo aprendido en la clase se han podido reforzar conocimientos que se aprendieron anteriormente en asignaturas como **Programación**. Además, se ahondó en aquellos temas que pueden ser relevantes para la visualización de datos y lo que hay detrás de los mismos (*HTML*, Python, entre otros lenguajes). 

A continuación, como trabajo final de la materia, se hace una recopilación del cómo fue posible realizar cada una de las actividades dirigidas siguiendo los pasos de una programación literaria. Es decir, un archivo que combine bloques de texto en Markdown y código de Python. 

## Actividad dirigida 1

La primera actividad de la asignatura involucró la escritura de un comentario crítico sobre un reportaje o noticia que contuviera visualización de datos. A través de máximo 500 palabras, cada estudiante analizó la noticia o artículo que le fuera de interés para la clase con conocimientos adquiridos de la asignatura de **Periodismo de Datos I**.

Para hacer correcta entrega de la también nombrada ad1, fue necesario realizar el comentario a través del editor de texto o "pad", una aplicación web que permite escribir texto plano de forma colaborativa. Es decir, que todas las personas de la clase ponían su nombre en el mismo editor junto a su comentario. 

La parte retadora de la actividad fue involucrar a la crítica el tipo de escritura **Markdown**, un lenguaje que se puede asociar al "código fuente" de un texto. Este tipo de lenguaje se utiliza, sobre todo, para realizar páginas web, cuadernos de Python y algunos gráficos de tipo interactivos.

A través de Markdown fue posible conocer, por ejemplo, como realizar encabezados de primer, segundo y tercer nivel con numerales (#), poner negritas con asteriscos, como subir imágenes y como enlazar textos. 

Así mismo, para esta actividad se conoció la plataforma [GitHub](https://github.com/), la cual, permite el desarrollo colaborativo de diversos proyectos, aloja proyectos en un servidor y crea códigos fuente, es decir, que desde GitHub también es posible, por ejemplo, escribir en lenguaje Markdown. 

Con la ad1 logramos crear, por primera vez, un documento de extensión .md a través de GitHub. Además, cada estudiante creo una página web compuesta por las carpetas de cada una de las actividades que se desarrollaron durante este curso.

Para lo anterior, accedimos a la configuración de GitHub y acitivamos su opción de Pages. Después, en la parte de *Branch* dejamos la opción *main* y como folder dejamos */root*. Toda esta configuración es un servicio de alojamiento de sitios que logra leer archivos en lenguaje HTML, CSS o JavaScript desde de un repositorio crado en la plataforma. 

Según GitHub esta opción "ejecuta los archivos a través de un proceso de compilación y publica un sitio web". Esta es la opción que logró que a través de la creación de carpetas y archivos .md (extensión de Markdown) hicieramos un reposotorio que cada una de las actividades dirigidas que después, se convertirían en una especie de [sitio web](https://nebrijas.github.io/2022online-MonicaBallesterosA/)

[Aquí es posible ver la ad1](https://github.com/nebrijas/2022online-MonicaBallesterosA/blob/a7bee14e94afeccebabb5b62049058a6e9290796/ad1.md)

## Actividad dirigida 2

Nuevamente, para esta actividad fue necesario crear un comentario de un artículo de periodismo de datos desde el cual se pudieran apreciar diversas visualizaciones. Para ello fue recomendada la página [*From data to viz*](https://www.data-to-viz.com), la cual plantea cuál sería la gráfica más adecuada de armar dependiendo la información que se tenga al respecto. 

Al igual que la ad1, esta actividad también fue escrita en Markdown y subido al repositorio de GitHub. Para esta ocasión, ya se tenía más confianza con el editor de GitHub, por lo que fue posible resolver varias dudas autónomamente como el procedimiento para enlazar correctamente una palabra. 

Para esta ocasión analicé la noticia [Following the Science](https://pudding.cool/2021/03/covid-science/), la cual, tenía como base **hablar sobre el empuje de la investigación global que se realizó hasta el año pasado para combatir la pandemia por el Covid-19**.

El comentario para la ad2 se basó en lo aprendido durante las clases de Periodismo de Datos en cuál es la forma correcta de hacer visualizaciones y el uso de los datos para que estas plasmen correctamente el mensaje que se quiere dar al usuario. 

Debido a que el propósito de esta actividad era usar Markdown, he puesto tres asteriscos antes de cada subtítulo con el fin de separar cada una de las ideas de análisis. Estos tres asteriscos se ponen solos después del párrafo deseado y forman una línea horizontal en el momento de la visualización. 

[Aquí es posible ver la ad2](https://github.com/nebrijas/2022online-MonicaBallesterosA/blob/a7bee14e94afeccebabb5b62049058a6e9290796/ad2.md)

## Actividad dirigida 3

Para la realización de esta actividad ya nos adentramos más en lenguajes programáticos como Python. Allí, fue necesario lograr el *scraping* de una web, pero, además de hacer que el código funcionara correctamente, era necesario explicar cada función de forma literaria. 

*Scraping* significa el poder extraer datos de una web y por ello, fue necesario profundizar en varios conocimientos nuevos y otros que se había aprendido en la asignatura de **Programación** para que, mediante herramientas como Jupyter de Anaconda, fuera posible realizar el ejercicio. 

Teniendo en cuenta lo anterior, lo primero que se hizo fue instalar en cada ordenador [Anaconda](https://www.anaconda.com/). Una vez este estuviera en el equipo de cada estudiante, se conoció el funcionamiento de la herramienta Jupyter. Este es un cuaderno y una aplicación web que permite generar archivos de Python y Markdown. Además, permite corroborar el correcto funcionamiento de los lenguajes. 

El *scraping* con el que se conoció a fondo Jupyter tuvo que ver con el diario español *El País*. La idea era encontrar el resultado mejor posicionado en dicha web, dependiendo la búsqueda que se hacía en ella y basándose en los `tags` que se usan al momento de publicar contenido en un medio de comunicación. 

Lo que consideré más importante y lo que me llevó más tiempo de investigación fue el descargue de las librerías, las cuales, permiten que el código se desenvuelva correctamente. Además, era el primer paso del *scraping*, por lo que era fundamental instalarlas correctamente a través de Jupyter. **A continuación el cómo se instalaron las librerías:**


~~~
pip install requests bs4 pandas termcolor
~~~
~~~
    Requirement already satisfied: requests in c:\users\usuario\anaconda3\lib\site-packages (2.28.1)
    Requirement already satisfied: bs4 in c:\users\usuario\anaconda3\lib\site-packages (0.0.1)
    Requirement already satisfied: pandas in c:\users\usuario\anaconda3\lib\site-packages (1.4.4)
    Requirement already satisfied: termcolor in c:\users\usuario\anaconda3\lib\site-packages (2.1.1)
    Requirement already satisfied: charset-normalizer<3,>=2 in c:\users\usuario\anaconda3\lib\site-packages (from requests) (2.0.4)
    Requirement already satisfied: urllib3<1.27,>=1.21.1 in c:\users\usuario\anaconda3\lib\site-packages (from requests) (1.26.11)
    Requirement already satisfied: certifi>=2017.4.17 in c:\users\usuario\anaconda3\lib\site-packages (from requests) (2022.9.14)
    Requirement already satisfied: idna<4,>=2.5 in c:\users\usuario\anaconda3\lib\site-packages (from requests) (3.3)
    Requirement already satisfied: beautifulsoup4 in c:\users\usuario\anaconda3\lib\site-packages (from bs4) (4.11.1)
    Requirement already satisfied: python-dateutil>=2.8.1 in c:\users\usuario\anaconda3\lib\site-packages (from pandas) (2.8.2)
    Requirement already satisfied: numpy>=1.18.5 in c:\users\usuario\anaconda3\lib\site-packages (from pandas) (1.21.5)
    Requirement already satisfied: pytz>=2020.1 in c:\users\usuario\anaconda3\lib\site-packages (from pandas) (2022.1)
    Requirement already satisfied: six>=1.5 in c:\users\usuario\anaconda3\lib\site-packages (from python-dateutil>=2.8.1->pandas) (1.16.0)
    Requirement already satisfied: soupsieve>1.2 in c:\users\usuario\anaconda3\lib\site-packages (from beautifulsoup4->bs4) (2.3.1)
    Note: you may need to restart the kernel to use updated packages.
~~~
 
Después de lo anterior, fue necesario crear y conocer el concepto de variable. En este caso, a la variable se le llamó resultado, sin embargo, teniendo en cuenta que esta puede cambiar, podía tener el nombre que se quisiera. El paso siguiente fue indicar que se requería de un `(requests.get)`, una función que permite arrastrar los resultados de *El País*. 

Según el portal [W3School](https://www.w3schools.com/python/module_requests.asp), esta función "le permite enviar solicitudes HTTP usando Python". Cuando se hace dicha solicitud HTTP, se devuelve una respuesta determinada que contiene los datos pedidos.

Finalmente, usamos la librería **Beautiful Soup**, la cual contribuye a extraer datos de archivos como HTML y XML. Además, proporciona formas de navegar, buscar y modificar la información obtenida si es instalada correctamente en nuestro documento Python. 

Dicha librería se ejecutó con la función `findAll` para los `h2`, pues así *El País* denomina sus titulares. Este proceso se realizó con la sección internacional, conociendo de antemano que era posible realizar la misma operación con secciones como deportes, salud, entre otras.

[Aquí es posible ver la ad3](https://github.com/nebrijas/2022online-MonicaBallesterosA/blob/a7bee14e94afeccebabb5b62049058a6e9290796/ad3.md)

## Actividad dirigida 4

La última actividad de la asignatura fue una de las más interesantes, pues, fue posible conocer como se extraen y visualizan datos de una web. En ella pudimos conocer formas, a través de la programación, del cómo visualizar los datos de una tabla con una gran cantidad de variables. 

Esta actividad consistió en conectar desde Jupyter a la **API de datos del COVID19**. La mayor parte de este ejercicio fue explicado en clase. Allí pudimos ver el trabajo que se puede hacer con la librería Pandas de Python. Al igual que con la actividad anterior, se realizó una explicación literaria de cada una de las funciones necesarias para desarrollar el código correctamente. 

Teniendo en cuenta que Pandas era la librería principal, el primer paso fue instalarla. Se creó una breve ación para llamarla y después se creó la variable `miurl`. Este último era importante para que Pandas detectara de donde sacar la información que después se solicitaría. A continuación se muestra el cómo instalar la librería:


~~~
!pip install pandas
~~~
~~~
    Requirement already satisfied: pandas in c:\users\usuario\anaconda3\lib\site-packages (1.4.4)
    Requirement already satisfied: python-dateutil>=2.8.1 in c:\users\usuario\anaconda3\lib\site-packages (from pandas) (2.8.2)
    Requirement already satisfied: numpy>=1.18.5 in c:\users\usuario\anaconda3\lib\site-packages (from pandas) (1.21.5)
    Requirement already satisfied: pytz>=2020.1 in c:\users\usuario\anaconda3\lib\site-packages (from pandas) (2022.1)
    Requirement already satisfied: six>=1.5 in c:\users\usuario\anaconda3\lib\site-packages (from python-dateutil>=2.8.1->pandas) (1.16.0)
~~~    

Más adelante, en el código, se aprendió a crear **dataframes**, un marco de datos que sirve para organizar la información. Los dataframes se pueden explorar de diversas maneras con las funciones correctas. Por ejemplo, para ver el inicio de la tabla extraída en la actividad se podía ver con la función `head` y para ver el final, con la función `tail`. 

Además, como se indicó al principio, fue posible crear gráficas con la función `plot`. A continuación, dejo una imagen ejemplo de las gráficas creadas:

![Ejemplo de gráfica de la ad4](https://nebrijas.github.io/2022online-MonicaBallesterosA/output_60_1.png)

[Aquí es posible ver la ad4](https://github.com/nebrijas/2022online-MonicaBallesterosA/blob/a7bee14e94afeccebabb5b62049058a6e9290796/ad4.md)
