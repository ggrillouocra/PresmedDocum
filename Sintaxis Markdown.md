# **Sintaxis Markdown**
En este apartado descubrirás la sintaxis Markdown y los conceptos básicos para escribir utilizando este lenguaje de marcado. De hecho, al final del mismo estarás perfectamente capacitado para empezar a utilizar este lenguaje en tus escritos y publicaciones.  
Fuente: https://markdown.es/sintaxis-markdown/#parrafos

La mejor manera de hacerse una idea de la sintaxis de Markdown es simplemente echar un vistazo a un escrito formateado como tal.

## Título
### Subtítulo
Este es un ejemplo de texto que da entrada a una lista genérica de elementos:

- Elemento 1
- Elemento 2
- Elemento 3

Este es un ejemplo de texto que da entrada a una lista numerada:

1. Elemento 1
2. Elemento 2
3. Elemento 3

Al texto en Markdown puedes añadirle formato como **negrita** o *cursiva* de una manera muy sencilla.

Como ves, se cumple perfectamente uno de los objetivos para los que Markdown fue diseñado, y es hacer las publicaciones lo más legibles posible.

Otro de los objetivos de Markdown, es que puedas publicar los documentos “como están”. No importa si el resultado final que necesitas es HTML, un PDF o texto en formato enriquecido (RTF); ya que siempre podrás obtener estos formatos a través de un conversor, o a través de aplicaciones compatibles con Markdown.

# Índice de sintaxis Markdown
En el lenguaje Markdown encontrarás tres tipos de elementos básicos que a su vez engloban el resto de la sintaxis. Considera esto una cheat sheet con la que guiarte.

Elementos de bloque  
Párrafos y saltos de línea  
Encabezados  
Citas  
Listas  
Códigos de bloque  
Reglas horizontales  
Elementos de línea  
Énfasis  
Links o enlaces  
Código  
Imágenes  
Elementos varios  
Links automáticos  
Omitir Markdown  

# Elementos de bloque

## Párrafos y saltos de línea
Para generar un nuevo párrafo en Markdown simplemente separa el texto mediante una línea en blanco (pulsando dos veces intro)

Al igual que sucede con HTML, Markdown no soporta dobles líneas en blanco, así que si intentas generarlas estas se convertirán en una sola al procesarse.

Para realizar un salto de línea y empezar una frase en una línea siguiente dentro del mismo párrafo, tendrás que pulsar dos veces la barra espaciadora antes de pulsar una vez intro.
 
Por ejemplo si quisieses escribir un poema Haiku quedaría tal que así:

«Andando con sus patitas mojadas,  
el gorrión  
por la terraza de madera»  

Donde cada verso tiene dos espacios en blanco al final.  


# Encabezados
Las # almohadillas son uno de los métodos utilizados en Markdown para crear encabezados. Debes usarlos añadiendo uno por cada nivel.

Es decir,
# Encabezado 1
## Encabezado 2
### Encabezado 3
#### Encabezado 4
##### Encabezado 5
###### Encabezado 6


Subrayar

Esto sería un encabezado 1
===
Esto sería un encabezado 2
---


Citas
Las citas se generar utilizando el carácter mayor que > al comienzo del bloque de texto.

> Un país, una civilización se puede juzgar por la forma en que trata a sus animales.  — Mahatma Gandhi



Incluso puedes concatenar varios >> para crear citas anidadas.

> Esto sería una cita como la que acabas de ver.
> 
> > Dentro de ella puedes anidar otra cita.
> 
> La cita principal llegaría hasta aquí. 


Listas
A diferencia de lo que ocurre en HTML, generar listas en Markdown es tremendamente sencillo. Puedes encontrarte con dos tipos.

Listas desordenadas
Para crear listas desordenadas utiliza * asteriscos, - guiones, o + símbolo de suma.

- Elemento de lista 1
- Elemento de lista 2
* Elemento de lista 3
* Elemento de lista 4
+ Elemento de lista 5
+ Elemento de lista 6

Para generar listas anidadas dentro de otras, simplemente tendrás que añadir **cuatro espacios en blanco antes del siguiente *, - o +.

- Elemento de lista 1
- Elemento de lista 2
    - Elemento de lista 3
    - Elemento de lista 4
        - Elemento de lista 5
        - Elemento de lista 6



Listas ordenadas
Para crear listas ordenadas debes utilizar la sintaxis de tipo: «número.» 1.. Al igual que ocurre con las listas desordenadas, también podrás anidarlas o combinarlas.

1. Elemento de lista 1
2.  Elemento de lista 2
    - Elemento de lista 3
    - Elemento de lista 4
        1. Elemento de lista 5
        2. Elemento de lista 6
        

Códigos de bloque
Si quieres crear un bloque entero que contenga código. Lo único que tienes que hacer es encerrar dicho párrafo entre dos líneas formadas por tres ~ virgulillas.

Tal que así:



 

~~~
Creando códigos de bloque.
Puedes añadir tantas líneas y párrafos como quieras.  
~~~
De esta forma, obtendrás el siguiente 


## Reglas horizontales
Las reglas horizontales se utilizan para separar secciones de una manera visual. Las estás viendo constantemente en este artículo ya que las estoy utilizando para separar los diferentes elementos de sintaxis de Markdown.

Para crearlas, en una línea en blanco deberás incluir tres de los siguientes elementos: asteriscos, guiones, o guiones bajos.

Es decir

***
---
___
También puedes separarlos mediante un espacio en blanco por pura estética.

* * *
- - -
_ _ _




Elementos de línea
Énfasis (negritas y cursivas)
Markdown utiliza asteriscos o guiones bajos para enfatizar.

Simplemente tendrás que envolver palabras o textos en éstos símbolos para conseguir cursivas o negritas.

MARKDOWN

*cursiva*

_cursiva_

**negrita**

__negrita__

Links o enlaces
Añadir enlaces a una publicación, más que común, hoy en día es algo casi obligatorio. Con Markdown tendrás varias formas de hacerlo.
***
Links o enlaces en línea
Son los enlaces de toda la vida. Como su nombre indica, se encuentran en línea con el texto.

Se crean escribiendo la palabra o texto enlazada entre [] corchetes, y el link en cuestión entre () paréntesis.

MARKDOWN	RESULTADO
[enlace en línea](http://www.limni.net)

***
Links o enlaces como referencia
La desventaja del método anterior, es que si utilizas links demasiado complejos o largos pueden dificultarte la lectura de tu texto.

Para solucionarlo y crear tu contenido de una manera más ordenada puedes generar enlaces de referencia.

Esto quiere decir que en tu texto enlazarás palabras o códigos concretos (formados por letras y/o números), que en otro lugar más apartado de tu documento tendrás definidos como determinadas URL.

[nombre que quieres darle a tu enlace][nombre de tu referencia]

[nombre de tu referencia]: http:www.tuenlace.com
Esto se ve más claro con un ejemplo.

Me llamo Javier Cristóbal y tengo un blog sobre [productividad mac][blog].

En dicha [web][blog] recopilo artículos sobre todo lo relacionado con automatización, gestión y eficiencia.

[blog]: http://limni.net/blog/
La referencia [blog] puede estar incluida en cualquier parte del documento, así puedes organizarte mejor y de una manera más limpia, recopilando todas tus referencias en un mismo lugar.

Además como ves a continuación, esta referencia no se incluye en el resultado final, sino que desaparece.

«Me llamo Javier Cristóbal y tengo un blog sobre productividad mac.

En dicha web recopilo artículos sobre todo lo relacionado con automatización, gestión y eficiencia.»

Links automáticos
Verás esta forma dentro de elementos varios: links automáticos

***
Sintaxis Markdown
En este apartado descubrirás la sintaxis Markdown y los conceptos básicos para escribir utilizando este lenguaje de marcado. De hecho, al final del mismo estarás perfectamente capacitado para empezar a utilizar este lenguaje en tus escritos y publicaciones.



La mejor manera de hacerse una idea de la sintaxis de Markdown es simplemente echar un vistazo a un escrito formateado como tal.

## Título
### Subtítulo
Este es un ejemplo de texto que da entrada a una lista genérica de elementos:

- Elemento 1
- Elemento 2
- Elemento 3

Este es un ejemplo de texto que da entrada a una lista numerada:

1. Elemento 1
2. Elemento 2
3. Elemento 3

Al texto en Markdown puedes añadirle formato como **negrita** o *cursiva* de una manera muy sencilla.

 
Como ves, se cumple perfectamente uno de los objetivos para los que Markdown fue diseñado, y es hacer las publicaciones lo más legibles posible.

Otro de los objetivos de Markdown, es que puedas publicar los documentos “como están”. No importa si el resultado final que necesitas es HTML, un PDF o texto en formato enriquecido (RTF); ya que siempre podrás obtener estos formatos a través de un conversor, o a través de aplicaciones compatibles con Markdown.

Índice de sintaxis Markdown
En el lenguaje Markdown encontrarás tres tipos de elementos básicos que a su vez engloban el resto de la sintaxis. Considera esto una cheat sheet con la que guiarte.

Elementos de bloque
Párrafos y saltos de línea
Encabezados
Citas
Listas
Códigos de bloque
Reglas horizontales
Elementos de línea
Énfasis
Links o enlaces
Código
Imágenes



 
Elementos varios
Links automáticos
Omitir Markdown
Elementos de bloque
Párrafos y saltos de línea
Para generar un nuevo párrafo en Markdown simplemente separa el texto mediante una línea en blanco (pulsando dos veces intro)

Al igual que sucede con HTML, Markdown no soporta dobles líneas en blanco, así que si intentas generarlas estas se convertirán en una sola al procesarse.

Para realizar un salto de línea y empezar una frase en una línea siguiente dentro del mismo párrafo, tendrás que pulsar dos veces la barra espaciadora antes de pulsar una vez intro.


 
Por ejemplo si quisieses escribir un poema Haiku quedaría tal que así:


 
«Andando con sus patitas mojadas,
el gorrión
por la terraza de madera»

Donde cada verso tiene dos espacios en blanco al final.

Encabezados
Las # almohadillas son uno de los métodos utilizados en Markdown para crear encabezados. Debes usarlos añadiendo uno por cada nivel.

Es decir,

# Encabezado 1
## Encabezado 2
### Encabezado 3
#### Encabezado 4
##### Encabezado 5
###### Encabezado 6
Se corresponde con

Encabezado 1
Encabezado 2
Encabezado 3
Encabezado 4
Encabezado 5
Encabezado 6
También puedes cerrar los encabezados con el mismo número de almohadillas, por ejemplo escribiendo ### Encabezado 3 ###. Pero la única finalidad de esto es un motivo estético.

Existe otra manera de generar encabezados, aunque este método está limitado a dos niveles.


 
Consiste en subrayar los encabezados con el símbolo = (para el encabezado 1), o con guiones - para el encabezado 2.

Es decir,

Esto sería un encabezado 1
===
Esto sería un encabezado 2
—-
No existe un número concreto = o - que necesites escribir para que esto funcione, ¡incluso bastaría con uno!

Citas
Las citas se generar utilizando el carácter mayor que > al comienzo del bloque de texto.

> Un país, una civilización se puede juzgar por la forma en que trata a sus animales.  — Mahatma Gandhi
Un país, una civilización se puede juzgar por la forma en que trata a sus animales. — Mahatma Gandhi

Si la cita en cuestión se compone de varios párrafos, deberás añadir el mismo símbolo > al comienzo de cada uno de ellos.

> Creo que los animales ven en el hombre un ser igual a ellos que ha perdido de forma extraordinariamente peligrosa el sano intelecto animal.

> Es decir, que ven en él al animal irracional, al animal que ríe, al animal que llora, al animal infeliz. — Friedrich Nietzsche

 
Creo que los animales ven en el hombre un ser igual a ellos que ha perdido de forma extraordinariamente peligrosa el sano intelecto animal.

Es decir, que ven en él al animal irracional, al animal que ríe, al animal que llora, al animal infeliz. — Friedrich Nietzsche

Incluso puedes concatenar varios >> para crear citas anidadas.

> Esto sería una cita como la que acabas de ver.
> 
> > Dentro de ella puedes anidar otra cita.
> 
> La cita principal llegaría hasta aquí. 
Esto sería una cita como la que acabas de ver.

Dentro de ella puedes anidar otra cita.

La cita principal llegaría hasta aquí.

Recuerda separar los saltos de línea con >, o >> si te encuentras dentro de la cita anidada; para crear párrafos dentro del mismo bloque de cita.

Listas
A diferencia de lo que ocurre en HTML, generar listas en Markdown es tremendamente sencillo. Puedes encontrarte con dos tipos.

Listas desordenadas
Para crear listas desordenadas utiliza * asteriscos, - guiones, o + símbolo de suma.

- Elemento de lista 1
- Elemento de lista 2
* Elemento de lista 3
* Elemento de lista 4
+ Elemento de lista 5
+ Elemento de lista 6
Da igual qué elemento escojas, incluso puedes intercambiarlos. Todos se verán igual al procesarse.

Elemento de lista 1
Elemento de lista 2
Elemento de lista 3
Elemento de lista 4
Elemento de lista 5
Elemento de lista 6
Para generar listas anidadas dentro de otras, simplemente tendrás que añadir **cuatro espacios en blanco antes del siguiente *, - o +.

- Elemento de lista 1
- Elemento de lista 2
    - Elemento de lista 3
    - Elemento de lista 4
        - Elemento de lista 5
        - Elemento de lista 6
Elemento de lista 1
Elemento de lista 2
Elemento de lista 3
Elemento de lista 4
Elemento de lista 5
Elemento de lista 6
Listas ordenadas
Para crear listas ordenadas debes utilizar la sintaxis de tipo: «número.» 1.. Al igual que ocurre con las listas desordenadas, también podrás anidarlas o combinarlas.

1. Elemento de lista 1
2.  Elemento de lista 2
    - Elemento de lista 3
    - Elemento de lista 4
        1. Elemento de lista 5
        2. Elemento de lista 6
Elemento de lista 1
Elemento de lista 2
Elemento de lista 3
Elemento de lista 4
Elemento de lista 5
Elemento de lista 6
Códigos de bloque
Si quieres crear un bloque entero que contenga código. Lo único que tienes que hacer es encerrar dicho párrafo entre dos líneas formadas por tres ~ virgulillas.

Tal que así:



 

~~~
Creando códigos de bloque.
Puedes añadir tantas líneas y párrafos como quieras.  
~~~
De esta forma, obtendrás el siguiente resultado:

Creando códigos de bloque.
Puedes añadir tantas líneas y párrafos como quieras.
Reglas horizontales
Las reglas horizontales se utilizan para separar secciones de una manera visual. Las estás viendo constantemente en este artículo ya que las estoy utilizando para separar los diferentes elementos de sintaxis de Markdown.

Para crearlas, en una línea en blanco deberás incluir tres de los siguientes elementos: asteriscos, guiones, o guiones bajos.

Es decir

***
---
___
También puedes separarlos mediante un espacio en blanco por pura estética.

* * *
- - -
_ _ _
Elementos de línea
Énfasis (negritas y cursivas)
Markdown utiliza asteriscos o guiones bajos para enfatizar.

Simplemente tendrás que envolver palabras o textos en éstos símbolos para conseguir cursivas o negritas.

MARKDOWN	RESULTADO
*cursiva*	cursiva
_cursiva_	cursiva
**negrita**	negrita
__negrita__	negrita
Por supuesto si quieres utilizar los dos tipos de énfasis no tienes más que combinar la sintaxis, envolviendo la palabra entre tres asteriscos o tres guiones bajos.

MARKDOWN	RESULTADO
***cursiva y negrita***	cursiva y negrita
___cursiva y negrita___	cursiva y negrita
Links o enlaces
Añadir enlaces a una publicación, más que común, hoy en día es algo casi obligatorio. Con Markdown tendrás varias formas de hacerlo.

Links o enlaces en línea
Son los enlaces de toda la vida. Como su nombre indica, se encuentran en línea con el texto.

Se crean escribiendo la palabra o texto enlazada entre [] corchetes, y el link en cuestión entre () paréntesis.

MARKDOWN	RESULTADO
[enlace en línea](http://www.limni.net)	enlace en línea
Links o enlaces como referencia
La desventaja del método anterior, es que si utilizas links demasiado complejos o largos pueden dificultarte la lectura de tu texto.

Para solucionarlo y crear tu contenido de una manera más ordenada puedes generar enlaces de referencia.

Esto quiere decir que en tu texto enlazarás palabras o códigos concretos (formados por letras y/o números), que en otro lugar más apartado de tu documento tendrás definidos como determinadas URL.

[nombre que quieres darle a tu enlace][nombre de tu referencia]

[nombre de tu referencia]: http:www.tuenlace.com
Esto se ve más claro con un ejemplo.

Me llamo Javier Cristóbal y tengo un blog sobre [productividad mac][blog].

En dicha [web][blog] recopilo artículos sobre todo lo relacionado con automatización, gestión y eficiencia.

[blog]: http://limni.net/blog/
La referencia [blog] puede estar incluida en cualquier parte del documento, así puedes organizarte mejor y de una manera más limpia, recopilando todas tus referencias en un mismo lugar.

Además como ves a continuación, esta referencia no se incluye en el resultado final, sino que desaparece.

«Me llamo Javier Cristóbal y tengo un blog sobre productividad mac.

En dicha web recopilo artículos sobre todo lo relacionado con automatización, gestión y eficiencia.»

Links automáticos
Verás esta forma dentro de elementos varios: links automáticos

Código
En según que tipo de publicaciones (sobre todo las de carácter técnico), necesitarás añadir pequeñas secciones donde mostrar código de otro lenguaje, atajos de teclado, o demás contenido que no debería ser tratado como tal.

Para ello tienes disponible dos alternativas.

Código puro 

`Esto es una línea de código`

Se convierte en

Esto es una línea de código

## Texto preformateado <pre>

La otra manera de añadir código en Markdown es comenzar el párrafo con cuatro espacios en blanco. Esto se corresponde con la etiqueta  HTML <>

    Esto es una línea de código    

 


Ojo, ¡estos espacios deberás incluirlos en cada línea que escribas! Para añadir código en bloque es mejor utilizar la sintaxis que viste anteriormente: códigos de bloque.

## Imágenes
Insertar una imagen con Markdown se realiza de una manera prácticamente idéntica a insertar links.

Solo que en este caso, deberás añadir un símbolo de ! exclamación al principio y el enlace no será otro que la ubicación de la imagen.

## [Texto alternativo](/ruta/a/la/imagen.jpg)

El texto alternativo es lo que se mostraría si la carga de la imagen fallase.

También podrás añadir un título alternativo entrecomillándolo al final de la ruta. Esto sería el título mostrado al dejar el cursor del ratón sobre la imagen.

![Texto alternativo](/ruta/a/la/imagen.jpg "Título alternativo")
Ya que al añadir imágenes también estás tratando con URLs, puedes utilizar el método que viste anteriormente para incluir links mediante referencias, solo que en este caso los enlaces de referencia serán aquellos donde se encuentre tu imagen.


De esta forma podrías insertar una imagen
![nombre de la imagen][img1]

O dos, sin ensuciar tu espacio de escritura.
![nombre de la imagen2][img2] 

[img1]: /ruta/a/la/imagen.jpg "Título alternativo"
[img2]: /ruta/a/la/imagen2.jpg "Título alternativo"


## Elementos varios
Links automáticos
Cuando viste los tipos de links te comenté que había un tipo más: los automáticos.

Estos son necesarios cuando lo que quieres es mostrar una URL completa, y no un enlace enmascarado bajo una palabra o frase como ocurre con los links en línea.

Para generar links automáticos tan solo tendrás que rodearlos con los símbolos < >

<http://www.limni.net>

## Omitir Markdown
Si has llegado hasta aquí es probable que te estés preguntando cómo he conseguido escribir ciertos símbolos como * asteriscos o _ guiones bajos, sin que Markdown los interprete para convertirlos en negritas, cursivas…

Esto es muy sencillo, ya que en este lenguaje existe un elemento estrella para especificar que todo lo que escribas a continuación, no se interprete como Markdown.

Se trata de la barra invertida \.

Escribiéndola justo delante de cualquiera de los elementos que verás a continuación, los mismos no tendrán efecto a la hora de convertirse en negritas, cursivas, links… 
</br>
</br>
\  barra invertida  
\`  acento invertido  
\*  asterisco  
\_  guión bajo  
\{} llaves  
\[] corchetes  
\() paréntesis  
\#  almohadilla

\+  símbolo de suma

\-  guión

\.  punto

\!  exclamación

Ahora que ya conoces todas las bondades de Markdown y has descubierto lo sencillo que resulta, seguro que quieres echarle el guante a alguna aplicación para empezar a escribir más cómodamente.