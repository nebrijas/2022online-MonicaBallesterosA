# AD3_Ballesteros_Mónica

En esta celda empezaría la explicación del código scraping. Primero, importamos las librerías y ponemos el código fuente. 

### [Archivo Python creado desde Jupyter:](https://github.com/nebrijas/2022online-MonicaBallesterosA/blob/86c6385da04492db5294bd480b427cb41ec9bd65/docs/AD3_Ballesteros_Angulo_M%C3%B3nica.ipynb)

## Código Fuente


```python
import requests
import time
import csv
import re
from bs4 import BeautifulSoup
import os
import pandas as pd
from termcolor import colored

resultados = []

req = requests.get("https://resultados.elpais.com")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup = BeautifulSoup(req.text, 'html.parser')

tags = soup.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req2 = requests.get("https://elpais.com/internacional")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup2 = BeautifulSoup(req2.text, 'html.parser')

tags = soup2.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req3 = requests.get("https://elpais.com/opinion")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup3 = BeautifulSoup(req3.text, 'html.parser')

tags = soup3.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req4 = requests.get("https://elpais.com/espana/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup4 = BeautifulSoup(req4.text, 'html.parser')

tags = soup4.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req5 = requests.get("https://elpais.com/economia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup5 = BeautifulSoup(req5.text, 'html.parser')

tags = soup5.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req6 = requests.get("https://elpais.com/sociedad/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup6 = BeautifulSoup(req6.text, 'html.parser')

tags = soup6.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req7 = requests.get("https://elpais.com/educacion/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup7 = BeautifulSoup(req7.text, 'html.parser')

tags = soup7.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req8 = requests.get("https://elpais.com/clima-y-medio-ambiente/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup8 = BeautifulSoup(req8.text, 'html.parser')

tags = soup8.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req9 = requests.get("https://elpais.com/ciencia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup9 = BeautifulSoup(req9.text, 'html.parser')

tags = soup9.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req10 = requests.get("https://elpais.com/cultura/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup10 = BeautifulSoup(req10.text, 'html.parser')

tags = soup10.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req11 = requests.get("https://elpais.com/babelia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup11 = BeautifulSoup(req11.text, 'html.parser')

tags = soup11.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req12 = requests.get("https://elpais.com/deportes/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup12 = BeautifulSoup(req12.text, 'html.parser')

tags = soup12.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req13 = requests.get("https://elpais.com/tecnologia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup13 = BeautifulSoup(req13.text, 'html.parser')

tags = soup13.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req14 = requests.get("https://elpais.com/tecnologia/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup14 = BeautifulSoup(req14.text, 'html.parser')

tags = soup14.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req15 = requests.get("https://elpais.com/gente/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup15 = BeautifulSoup(req15.text, 'html.parser')

tags = soup15.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req16 = requests.get("https://elpais.com/television/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup16 = BeautifulSoup(req16.text, 'html.parser')

tags = soup16.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)

req17 = requests.get("https://elpais.com/eps/")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup17 = BeautifulSoup(req17.text, 'html.parser')

tags = soup17.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)


os.system("clear")

print(colored("A continuación se muestran los titulares de las páginas principales del diario El País que contienen las siguientes palabras:", 'blue', attrs=['bold']))
print(colored("Feminismo", 'green', attrs=['bold']))

str_match = [s for s in resultados if "feminismo" in s]
print("\n".join(str_match))

print(colored("Igualdad", 'green', attrs=['bold']))

str_match = [s for s in resultados if "igualdad" in s]
print("\n".join(str_match))

print(colored("Mujeres", 'green', attrs=['bold']))

str_match = [s for s in resultados if "mujeres" in s]
print("\n".join(str_match))

print(colored("Mujer", 'green', attrs=['bold']))

str_match = [s for s in resultados if "mujer" in s]
print("\n".join(str_match))

print(colored("Brecha salarial", 'green', attrs=['bold']))

str_match = [s for s in resultados if "brecha salarial" in s]
print("\n".join(str_match))

print(colored("Machismo", 'green', attrs=['bold']))

str_match = [s for s in resultados if "machismo" in s]
print("\n".join(str_match))

print(colored("Violencia", 'green', attrs=['bold']))

str_match = [s for s in resultados if "violencia" in s]
print("\n".join(str_match))

print(colored("Maltrato", 'green', attrs=['bold']))

str_match = [s for s in resultados if "maltrato" in s]
print("\n".join(str_match))

print(colored("Homicidio", 'green', attrs=['bold']))

str_match = [s for s in resultados if "homicidio" in s]
print("\n".join(str_match))

print(colored("Género", 'green', attrs=['bold']))

str_match = [s for s in resultados if "género" in s]
print("\n".join(str_match))

print(colored("Asesinato", 'green', attrs=['bold']))

str_match = [s for s in resultados if "asesinato" in s]
print("\n".join(str_match))

print(colored("Sexo", 'green', attrs=['bold']))

str_match = [s for s in resultados if "sexo" in s]
print("\n".join(str_match))
```

## Se instalan librerías


```python
pip install requests bs4 pandas termcolor
```

    Requirement already satisfied: requests in c:\users\usuario\anaconda3\lib\site-packages (2.28.1)
    Collecting bs4
      Downloading bs4-0.0.1.tar.gz (1.1 kB)
      Preparing metadata (setup.py): started
      Preparing metadata (setup.py): finished with status 'done'
    Requirement already satisfied: pandas in c:\users\usuario\anaconda3\lib\site-packages (1.4.4)
    Collecting termcolor
      Downloading termcolor-2.1.1-py3-none-any.whl (6.2 kB)
    Requirement already satisfied: urllib3<1.27,>=1.21.1 in c:\users\usuario\anaconda3\lib\site-packages (from requests) (1.26.11)
    Requirement already satisfied: charset-normalizer<3,>=2 in c:\users\usuario\anaconda3\lib\site-packages (from requests) (2.0.4)
    Requirement already satisfied: certifi>=2017.4.17 in c:\users\usuario\anaconda3\lib\site-packages (from requests) (2022.9.14)
    Requirement already satisfied: idna<4,>=2.5 in c:\users\usuario\anaconda3\lib\site-packages (from requests) (3.3)
    Requirement already satisfied: beautifulsoup4 in c:\users\usuario\anaconda3\lib\site-packages (from bs4) (4.11.1)
    Requirement already satisfied: pytz>=2020.1 in c:\users\usuario\anaconda3\lib\site-packages (from pandas) (2022.1)
    Requirement already satisfied: numpy>=1.18.5 in c:\users\usuario\anaconda3\lib\site-packages (from pandas) (1.21.5)
    Requirement already satisfied: python-dateutil>=2.8.1 in c:\users\usuario\anaconda3\lib\site-packages (from pandas) (2.8.2)
    Requirement already satisfied: six>=1.5 in c:\users\usuario\anaconda3\lib\site-packages (from python-dateutil>=2.8.1->pandas) (1.16.0)
    Requirement already satisfied: soupsieve>1.2 in c:\users\usuario\anaconda3\lib\site-packages (from beautifulsoup4->bs4) (2.3.1)
    Building wheels for collected packages: bs4
      Building wheel for bs4 (setup.py): started
      Building wheel for bs4 (setup.py): finished with status 'done'
      Created wheel for bs4: filename=bs4-0.0.1-py3-none-any.whl size=1257 sha256=ecca57db005167c16ab6a694b5db55dafc35d583eab6e3c3809b24b64dfb117f
      Stored in directory: c:\users\usuario\appdata\local\pip\cache\wheels\73\2b\cb\099980278a0c9a3e57ff1a89875ec07bfa0b6fcbebb9a8cad3
    Successfully built bs4
    Installing collected packages: termcolor, bs4
    Successfully installed bs4-0.0.1 termcolor-2.1.1
    Note: you may need to restart the kernel to use updated packages.
    

## Se importan librerías

Primero, importamos de la librería la función `requests` para hacer peticiones de datos:


```python
import requests
```

Después, importamos de la librería la función `time` pues nos interesa el tiempo horario y hacer peticiones en tiempos determinados:


```python
import time
```

A continuación, se importa la función `csv` porque se espera que en algún momento trabaje con dicha función:


```python
import csv
```

Se importa después la libería de expresiones regulares, `re`, que puede ser usada para las coincidencias:


```python
import re
```

Se importa la librería de Python bajo la función `BeautifulSoup` para extraer datos de archivos HTML y XML.


```python
from bs4 import BeautifulSoup
```

Se importa la librería `os`para usar funcionalidades dependientes del sistema operativo. 


```python
import os
```

Lo siguiente es importar la librería `pandas` con el abreviado estándar para hacer referencia a pandas `as`:


```python
import pandas as pd
```

A continuación se importa desde el módulo `termcolor` la un función `colored` que permite imprimir texto en color:


```python
from termcolor import colored
```

## Objetos o variables

Se crea una variable en la que vacia en la que se pueden añadir los resultados del *Scrapping*:


```python
resultados = []
```

A continuación, usamos la función `Type()` para organizar los resultados obtenidos en forma de lista:


```python
type(resultados)
```




    list



## Solicitud de acceso a datos para el sitio web de El País

Agregamos una variable en la que se pueda solicitar información de la URL: req=requests.get ("https://resultados.elpais.com")


```python
req = requests.get("https://resultados.elpais.com")
```

Más tarde, escribimos la función `type()` y esa es la respuesta de la función `request`: 


```python
type(req)
```




    requests.models.Response



Después utilizamos un condicional de tipo `if`. De este modo, cuando el valor no sea 200, no se pueda leer la página. 

Si el valor es 200, la página podrá verse con éxito.


```python
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
```

## Aquí comienza a actuar el Beautiful soap

A continuación agregamos una variable que facilita extraer información de páginas web:


```python
soup = BeautifulSoup(req.text, 'html.parser')
```

Aquí agregamos la variable `tags` que permita encontrar los `h2` dentro de la página ya mencionada:


```python
tags = soup.findAll("h2")
```

Utilizamos la función `for` para encontrar todos los `h2` que se encuentran en la función anterior y que muestre el texto dentro de las etiquetas. 

Seguido a lo anterior utilizamos `resultados.append(h2.text)` para añadir todos los textos que están en las etiquetas a la lista inicial resultados:


```python
for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```

    El Mundial, en vivo
    Universo Mundial
    El calendario a seguir desde América
    ¿Quién va a ganar? Simulador y pronóstico de cada selección 
    La ‘newsletter’
    Las protestas se extienden en China contra la política de covid cero
    La gestión del frío enfrenta a Zelenski y al alcalde de Kiev
    La vida bajo los bombardeos rusos
    Así se vive en un refugio invernal durante la guerra
    Pobreza en el Olimpo académico de EE UU: la huelga que cimbra a la Universidad de California 
    El caótico primer mes de Elon Musk en Twitter
    ‘Argentina, 1985’, un debate nacional entre la ficción y la memoria
    Alemania rescata un empate contra España sobre el final del partido
    Un empate socialdemócrata
    Datos y gráficos | Alemania explota un error de España para empatar un partido equilibrado
    Croacia da vuelta el partido y elimina a Canadá (4-1)
    Marruecos da un batacazo a Bélgica sobre el final (0-2)
    Costa Rica se redime ante un Japón sin puntería (0-1)
    Madrid, la nueva Miami: así se han hecho con la capital española los ricos latinoamericanos
    López Obrador saca músculo en las calles con una manifestación masiva en México
    El Bosque, el pueblo mexicano que se tragó el mar
    Argentina contra la impunidad de los feminicidios
    Neofascistas, nacionalpopulistas, tecnosoberanistas. ¿Cómo llamamos a las nuevas derechas radicales? 
    Las abuelas que han viralizado el arte de elaborar la pasta italiana
    Pepa Bueno: “Las páginas de EL PAÍS tienen que ser el lugar donde los diferentes se encuentren”
    Videoanálisis | La FIL mastodóntica y popular está de vuelta
    La FIL de Guadalajara pone una vela al libro y otra al balón
    Concepción Company: “De todos los mexicanismos me quedo con apapachar”
    El acoso invernal de Putin 
    Por el bien de todos
    Otra forma de violencia política
    Yo te vi, papá, emocionarte con Messi
    Ideas de regalos para el jardinero
    Guía de regalos para el ‘foodie’
    Bolsonaro reaparece en una ceremonia militar tras batallar su derrota desde la trastienda
    El sueño hecho realidad del refugiado sirio del selfi con Merkel
    Crónica del asesinato de una niña en la Francia rural
    La violencia verbal de Vox desborda el Congreso español
    
    El negocio de las chicas imagen en las discotecas: “La misión es sonreír y que los hombres beban más”
    Las guatemaltecas que estudian ingeniería para llevar luz a sus comunidades
    Impresiones 3D y Telegram: el premiado proyecto de estudiantes colombianos para potabilizar agua
    La ‘ciudad esponja’: diez soluciones para resolver el problema del agua en México
    Cómic y energía nuclear: el superventas francés que sacude el debate sobre el cambio climático
    En la biblioteca de Almudena Grandes
    Otras mujeres
    Adiós a Ellen Pompeo, la funcionaria de la tele
    ¿Selfie sí o selfie no en Art Basel?
    De las galerías a las calles: así se hizo importante Miami para el arte del mundo
    La bestial tensión sexual entre Bruce Willis y Cybill Shepherd en ‘Luz de luna’, la serie en la que la actriz tuvo mucho que decir
    Confesiones de la mujer que lleva 40 años decidiendo quién será el nuevo James Bond
    Alessandro Michele, crónica de una salida anunciada
    Leonor Lavado: “Somos como hablamos: la voz es nuestro ADN psicológico”
    De la carnicería de su padre en España a la estrella Michelin en Chicago
    Macondo Inundado: el pueblo donde nunca deja de llover 
    Dormir en una caja a 200 euros la noche para asistir al Mundial de Qatar
    Retrato de Pablo Milanés a través de sus 10 canciones más decisivas
    De Honduras a Ucrania: cuando un niño crece bajo las bombas
    Qatar 2022, el único mundial donde es posible ver dos partidos en un mismo día
    ¿Qué estrella tuvo el mejor debut en el Mundial? El ‘tier list’ de Jesús Gallego, Bruno Alemany y Aritz Gabilondo
    Enredados en el Mundial | Los jugadores iraníes vuelven a cantar el himno y ha nacido una estrella en EE UU
    Al menos 500 alpacas mueren por una ola de frío en Perú
    Los partidarios de Bolsonaro utilizan sus móviles para pedir un golpe “extraterrestre” 
    Cuatro carceleros dan un brutal paliza a un hombre negro en Georgia
    Protests spread across China as anger builds over Xi Jinping’s zero-Covid policy 
    War in Ukraine: The battle to survive sub-zero temperatures 
    The story of a crypto scammer that ended in suicide
    To boost oil supplies, US looks to lift sanctions on Venezuela
    Americanas: Reportajes y noticias sobre feminismo e historias con enfoque de género de la región
    Toda la actualidad científica en el boletín de Materia
    Letras Americanas: la actualidad literaria de un continente vista por el escritor Emiliano Monge
    Ideas: reportajes y entrevistas para entender el mundo
    El Kremlin silencia el dolor de las mujeres rusas que critican la guerra de Ucrania 
    El primer ministro de Rumania: “Necesitamos un esfuerzo común en la OTAN para defender cada centímetro de territorio frente a Rusia”  
    La justicia investiga si el Gobierno de Macron favoreció a consultoras privadas en las dos últimas campañas presidenciales en Francia
    Aquí puede buscar si ha sido engañado por la estafa internacional de las criptomonedas
    El secreto de la pirámide
    El futuro de las compras: más redes sociales, pago a plazos y vuelta de la tienda física
     El Papa detecta fallos en Caritas Internationalis y cesa a sus responsables 
    La Iglesia italiana da por primera vez cifras de los abusos cometidos por el clero
    El Senado de EE UU da un paso clave para blindar el matrimonio homosexual frente al Supremo
    Muere Hans Magnus Enzensberger, gran intelectual alemán del siglo XX
    ‘Close’, una mirada conmovedora a la fragilidad de la preadolescencia
    La gran retrospectiva de Vermeer en Ámsterdam aviva la polémica sobre la autoría de ‘Muchacha con flauta’
    Vivir con un trastorno alimentario: “Me di cuenta cuando me miré al espejo y vi la muerte”
    Josefa Ros Velasco, filósofa: “Si alguien se aburre suele darse a la botella, cuando le pasa a un país suele darse una revuelta”
    La insólita historia de la mujer que descubrió el primer antibiótico español
    Canadá conquista su primera Davis a lomos de Aliassime
    La selección femenina de baloncesto se clasifica para el próximo Eurobasket
    La trituradora del Barcelona no tiene piedad con el Atlético (1-6)
    Operación ‘OS35’: cómo rescatar un gigante de 40.288 toneladas varado a la sombra de Gibraltar
    ¿Podré matar a una rata que entre en mi casa? Claves de la reforma del Código Penal para castigar más el maltrato animal
    La izquierda retira por sorpresa y a última hora la propuesta para abolir los toros en Francia 
    Mastodon: qué es y cómo funciona la red social en la que los usuarios deciden qué está permitido
    Así serán las nuevas marcas de verificación en Twitter: azul, oro y gris
    Gafas con funciones de un móvil, ‘Photoshop’ instantáneo y otros inminentes avances gracias a los nuevos chips
    Sánchez pide a la patronal que negocie con los sindicatos un acuerdo salarial
    El pasado franquista pervive en Santa Cruz de Tenerife
    La federación de la España Vaciada busca implantarse en todo el país 
    ‘The Peripheral’, realidad, ficción y un futuro ciberpunk con los creadores de ‘Westworld’
    ‘Ummo’, un guirigay intergaláctico’, por Jimina Sabadú
    El ‘bon vivant’ acorralado de la FIFA que grabó a sus amigos
    Windsor desvela su decoración navideña en las primeras festividades sin Isabel II y con Carlos III como rey
    Camila y los 1.000 osos Paddington: la reina entrega a una ONG infantil los peluches en homenaje a Isabel II
    Stallone vs. Schwarzenegger, la “competición” eterna: “Éramos antagonistas. Soñaba con pegarle y él con pegarme a mí”
    El misterio de Manuel Carrasco: cómo salir de una barriada de pescadores y acabar siendo un cantante que llena estadios
    Los guardianes de la ensaladilla rusa, la tapa popular que subió a los altares ‘gourmet’ 
    Erri De Luca, escritor: “Construir una vida es más difícil que contarla”
    Descansar está mal visto: el arte perdido del reposo
    Perdidos en el laberinto del paro
    Su vecino lo timaba con la calefacción central
    En la cuneta del sueño americano
    Descuidos de seleccionador: los lectores agregan libros de fútbol que no entraron en la lista
    Mi combate contra la ablación y el VIH en Senegal
    Masacre en Melilla: la peligrosa decisión de socialistas y populares
    Oyambre, Son Bou y otras nueve playas españolas para un baño de historia
    Cómo actuar ante el caos de los aeropuertos: qué hacer frente a retrasos y cancelaciones de un vuelo
    Samantha Hudson: “Me va bien económicamante, pero no soy Paula Echevarría. Nunca seré normativa”
    Alaska: “No entiendo la cultura de la cancelación”
    ¿Es buena idea masturbarse antes de salir? Las verdades y mentiras de la relajación posorgasmo
    El dilema Kit Connor: ¿debe conocerse la sexualidad de un actor para interpretar un papel gay?
    Vender carne... y un estilo de vida: así son las nuevas hamburgueserías
    ¿Cuál es la mejor receta de puré de patatas?
    Las nuevas jubilaciones: más retiros parciales, casi a los 65 años y cobrando 1.258 euros
    “Me rompí por dentro y hasta hoy”: desgarrador testimonio de una mujer a la que nadie creyó mientras era víctima de acoso
    Macarena Olona sorprende a todos al publicar este mensaje sobre Begoña Gómez
    Le van a llover los palos: la cantada de Courtois que mete en un lío gordo a Bélgica
    Ocho mil millones de cursis
    Las 10 mejores películas y sagas posapocalípticas
    

Realizamos los mismos pasos para todas las secciones del diario El País. Por ejemplo, así se haría con la sección **internacional**:


```python
req2 = requests.get("https://elpais.com/internacional")
# Si el estatus code no es 200 no se puede leer la página
if (req.status_code != 200):
 raise Exception("No se puede hacer Web Scraping en"+ URL)
soup2 = BeautifulSoup(req2.text, 'html.parser')

tags = soup2.findAll("h2")

for h2 in tags:
    print(h2.text)
    resultados.append(h2.text)
```

    Las protestas se extienden en China contra la política de covid cero
    Hartazgo, estragos económicos y accidentes mortales: claves para entender las protestas en China
    El último Iphone, perfumes de Chanel o un Rolex: las marcas occidentales llenan los escaparates rusos pese a las sanciones
    Publicar no es un delito
    La vida bajo los bombardeos rusos
    Democracias a la defensiva
    La UE vista desde el G-20 de Bali 
    El arte ruso de la provocación
    China y Estados Unidos, condenadas a entenderse y a rivalizar
    Lecciones en Ucrania para ser reportero de guerra: explosiones de fogueo, torniquetes y campos de minas
    De la manifestación al patíbulo: el régimen iraní amenaza con la horca para sofocar las protestas
    Publicar no es un delito
    Los medios de los cables de WikiLeaks piden a EE UU que no persiga a Assange
    La gestión del frío enfrenta a Zelenski y al alcalde de Kiev
    El sueño hecho realidad del refugiado sirio del selfi con Merkel
    Los trabajadores migrantes de provincias en China estallan contra los confinamientos por covid
    Sobrevivir bajo cero en Ucrania
    La UE teme que los ataques rusos contra la red eléctrica de Ucrania fuercen otra oleada de refugiados
    Encuentran el cadáver de una niña desaparecida en el corrimiento de tierra en la isla italiana de Ischia
    Justin Trudeau justifica el uso de la Ley de emergencia para desalojar a los camioneros antivacunas
    La nota del autor de la matanza del Walmart de Virginia: “Se reían de mí y decían que era un asesino en serie”
    La pobreza se ceba con los menores de 18 años en América Latina
    Tres horas libres en el trabajo para ver el partido… ¡Bienvenidos a Brasil!
    Petro y López Obrador estrenan un eje latinoamericano con el éxito de la negociación de Venezuela como trasfondo
    

## Titulares y estilo de las páginas principales de El País

Lo primero que se puede hacer es utilizar una función para que se haga una limpieza después de realizar el web *Scrapping*:


```python
os.system("clear")
```




    1



A continuación, con la función `print(colored)`, seguido del uso de `bold`, se pueden poner los titulares en negrita. Para probarlo, se subdividirán los títulares que digan feminismo:


```python
print(colored("A continuación se muestran los titulares de las páginas principales del diario El País que contienen las siguientes palabras:", 'blue', attrs=['bold']))
print(colored("Feminismo", 'green', attrs=['bold']))
```

    A continuación se muestran los titulares de las páginas principales del diario El País que contienen las siguientes palabras:
    Feminismo
    

Seguido de lo anterior, utilizamos la función `for` para, nuevamente, verificar que se contiene la palabra clave:


```python
str_match = [s for s in resultados if "feminismo" in s]
print("\n".join(str_match))
```

    Americanas: Reportajes y noticias sobre feminismo e historias con enfoque de género de la región
    Americanas: Reportajes y noticias sobre feminismo e historias con enfoque de género de la región
    

Se repite el mismo proceso con las demás palabras: 


```python
print(colored("Igualdad", 'green', attrs=['bold']))

str_match = [s for s in resultados if "igualdad" in s]
print("\n".join(str_match))

print(colored("Mujeres", 'green', attrs=['bold']))

str_match = [s for s in resultados if "mujeres" in s]
print("\n".join(str_match))

print(colored("Mujer", 'green', attrs=['bold']))

str_match = [s for s in resultados if "mujer" in s]
print("\n".join(str_match))

print(colored("Brecha salarial", 'green', attrs=['bold']))

str_match = [s for s in resultados if "brecha salarial" in s]
print("\n".join(str_match))

print(colored("Machismo", 'green', attrs=['bold']))

str_match = [s for s in resultados if "machismo" in s]
print("\n".join(str_match))

print(colored("Violencia", 'green', attrs=['bold']))

str_match = [s for s in resultados if "violencia" in s]
print("\n".join(str_match))

print(colored("Maltrato", 'green', attrs=['bold']))

str_match = [s for s in resultados if "maltrato" in s]
print("\n".join(str_match))

print(colored("Homicidio", 'green', attrs=['bold']))

str_match = [s for s in resultados if "homicidio" in s]
print("\n".join(str_match))

print(colored("Género", 'green', attrs=['bold']))

str_match = [s for s in resultados if "género" in s]
print("\n".join(str_match))

print(colored("Asesinato", 'green', attrs=['bold']))

str_match = [s for s in resultados if "asesinato" in s]
print("\n".join(str_match))

print(colored("Sexo", 'green', attrs=['bold']))

str_match = [s for s in resultados if "sexo" in s]
print("\n".join(str_match))

```

    Igualdad
    
    Mujeres
    Otras mujeres
    El Kremlin silencia el dolor de las mujeres rusas que critican la guerra de Ucrania 
    Otras mujeres
    El Kremlin silencia el dolor de las mujeres rusas que critican la guerra de Ucrania 
    Mujer
    Otras mujeres
    Confesiones de la mujer que lleva 40 años decidiendo quién será el nuevo James Bond
    El Kremlin silencia el dolor de las mujeres rusas que critican la guerra de Ucrania 
    La insólita historia de la mujer que descubrió el primer antibiótico español
    “Me rompí por dentro y hasta hoy”: desgarrador testimonio de una mujer a la que nadie creyó mientras era víctima de acoso
    Otras mujeres
    Confesiones de la mujer que lleva 40 años decidiendo quién será el nuevo James Bond
    El Kremlin silencia el dolor de las mujeres rusas que critican la guerra de Ucrania 
    La insólita historia de la mujer que descubrió el primer antibiótico español
    “Me rompí por dentro y hasta hoy”: desgarrador testimonio de una mujer a la que nadie creyó mientras era víctima de acoso
    Brecha salarial
    
    Machismo
    
    Violencia
    Otra forma de violencia política
    La violencia verbal de Vox desborda el Congreso español
    
    Otra forma de violencia política
    La violencia verbal de Vox desborda el Congreso español
    
    Maltrato
    ¿Podré matar a una rata que entre en mi casa? Claves de la reforma del Código Penal para castigar más el maltrato animal
    ¿Podré matar a una rata que entre en mi casa? Claves de la reforma del Código Penal para castigar más el maltrato animal
    Homicidio
    
    Género
    Americanas: Reportajes y noticias sobre feminismo e historias con enfoque de género de la región
    Americanas: Reportajes y noticias sobre feminismo e historias con enfoque de género de la región
    Asesinato
    Crónica del asesinato de una niña en la Francia rural
    Crónica del asesinato de una niña en la Francia rural
    Sexo
    
    
