# Comandos de la Práctica 03
## Nora Hilda Hernández Luna

$mkdir nhernandez_p03
$cd nhernandez_p03
$touch comandos_p03.md
$mkdir data
$cd data
$mkdir filtered  
$mkdir raw_data 
$cd .. 
$mkdir meta 
$mkdir scripts  
$mkdir figures  
$mkdir archive

&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&
# Parte I. 

Responde: 
1.1 ¿A qué organismo pertenece? 
Mycoplasma genitalium
1.2 ¿Es un gen o una región genómica de importancia? 
Es un gen, el gen 16s de RNA ribosomal.
1.3 ¿Qué es un marcador molecular? 
Los marcadores moleculares son biomoléculas que se pueden relacionar con un rasgo genético. Las biomoléculas que pueden ser marcadores moleculares son las proteínas (antígenos e isoenzimas) y el DNA (genes conocidos o fragmentos de secuencia y función desconocida). 
1.4 ¿Cuál es la importancia de este tipo de marcador en particular?
El DNA ribosomal 16s se encuentra en todos los organismos. Este gen contiene regiones de alta variabilidad, que permiten clasificar a nivel de especie y cepa.


2.

Tipo: BLASTN	
Definición: Comparar secuencias de nucleótidos con secuencias de nucleótidos	
Aplicación: Análisis filogenético

Tipo:BLASTP	
Definición: Comparar secuencias de aminoácidos, con secuencias proteicas de la base de datos
Aplicación: Para realizar los alineamientos, aunque puede usar una matriz definida por el usuario

Tipo:BLASTX	
Definición: Comparar secuencias de nucleótidos con secuencias proteícas	
Aplicación: Busca las proteínas que codifican una secuencia

Tipo:TBLASTX	
Definición: Comparar todos los marcos de lectura de una secuencia respecto a los marcos de lectura de una base de datos	
Aplicación: Verificar el efecto de mutaciones en el marco de lectura.

Tipo:TBLASTN	
Definición: Comparar secuencias proteicas con secuencias de nucelótido de la base de datos	
Aplicación: Buscar secuencias de nucleótidos que codifiquen para esa proteína.

&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

# Parte II.

Explica:¿En qué consiste el problema de los puentes de la ciudad de Königsberg?

La ciudad de Kaliningrado, antiguamente llamada Königsberg, es un bonito lugar situado en la desembocadura del río Pregolya, en la antigua Prusia Oriental. Este río atravesaba la ciudad, dividiendo la zona en varias partes. Para no perder la comunicación, ésta estaba llena de un sistema de puentes conectores.

En total, había siete grandes puentes en Kaliningrado: el puente del herrero, el puente conector, el puente verde, el puente del mercado, el puente de madera, el puente alto y el puente de la miel.

Los ciudadanos se sentían muy orgullosos de esta gran red de comunicación, y entre ellos surgió un pequeño juego para entretenerse en los momentos de aburrimiento. Solo consistía en una sola pregunta:

¿Se pueden atravesar todos los puentes pasando sólo una vez por cada puente?


¿Por qué no tiene solución?
Para poder recorrer un sistema de este tipo, los vértices «intermedios» deben tener un número par de aristas. Es decir, deben tener una vía para entrar y una vía para salir. Sólo los puntos de inicio y salida pueden tener un número impar de aristas, porque, evidentemente, nunca «entramos» al punto de inicio y nunca «salimos» del punto de llegada.


Explica: tres problemáticas comunes en la aplicación de las gráficas de Bruijin a genomas.

En primer lugar las tecnologías de secuenciación generan miles de lecturas, en las gráficas de Bruijin estas lecturas se fragmentan en pedazos que van a representar los nodos, dando como resultado billones de estos.
En segundo lugar regiones no secuenciadas y errores de secuenciación dividen más los cromosomas en contigs y huecos, con una ruta para cada contig.
En tercer lugar los cromosomas múltiples y lineales, en esta parte se tiene que buscar un camino euleriano, que no es necesario que termine en el nodo donde comienza; entonces se tiene una ruta para cada cromosoma.

Explica: Las estadísticas N50 y L50. 
¿qué son? Son estadísticas de un conjunto de longitudes. 
¿en qué consisten? N50 da la longitud del conting menor de los mayores. L50 es el número de cotings cuya suma de su longitud es N50.
¿para qué se usan? Se usan para hacer comparaciones entre ensamblajes de genomas de diferentes tamaños.

&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&6&&&&&&
#Referencias
http://www.encuentros.uma.es/encuentros49/marcadores.html
Valenzuela-González, F., Casillas-Hernández, R., Villalpando, E. y Vargas-Albores, F. (2015). El gen ARNr 16S en el estudio de comunidades microbianas marinas. Ciencias marinas, 41(4), 297-313.

https://es.wikipedia.org/wiki/BLAST

https://aprendiendomatematicas.com/los-puentes-de-konigsberg/
Aguilar-Bultet, L. y Falquet, L. (2015) Secuenciación y ensamblaje de novo de genomas bacterianos: una alternativa para el estudio de nuevos patógenos.Revista de Salud Animal, 37(2).

Garcia Navarrete, L. T. (2018). Estrategia computacional para detección y caracterización de bloques microsíntenicos relacionados a regiones genómicas asociadas a domesticación en frijol Lima. Departamento de Ingeniería de Sistemas e Industrial.