# Prototipado y conceptos básicos de HTML
------
# El papel

## Sketch
Es un dibujo rápido o bosquejo guía, que produce de manera muy sencilla un concepto, una idea o generalidad de un proyecto.
![Pin en Wireframes](http://webdesdecero.com/wp-content/uploads/2015/03/wireframe-en-papel-e1427730160670.jpg)

## Wireframe
Es la representación estática, en baja calidad, de un diseño. Se definen, para una mejor compresión, los siguientes aspectos:
- ¿Qué? Los principales grupos de contenido.
- ¿Dónde? La estructura de la información.
- ¿Cómo? La descripción y visualización básica del usuario - interacción de la interfaz
![Wireframes: Que son y como crearlos | Web desde cero](https://webdesdecero.com/wp-content/uploads/2015/03/wireframing-a-maquina.jpg)

## Mockup
Es la representación estática de un diseño, en calidad media o alta.
![▷ Mockup sitio web | Actualizado noviembre 2022](https://agencia13.es/wp-content/uploads/2021/08/mockup-sitio-web.jpg)

## Prototipo
Es la representación navegable del producto final.
- Invision
- Axure RP
- Just in mind
- POP

## Tips para armar un buen prototipo
- **Trabaja primero en la arquitectura de la información
	- **Agrupa:** qué contenidos están relacionados entre sí.
	- **Jerarquza:** cuáles contenidos están subprdinados.
	- **Rotula:** cómo se nombran los grupos de contenidos.
- **Testea tu prototipo:** una vez que tengas el prototipo de baja fidelidad (sketch), pruébalo con alguien, para conocer si es claro y funciona la forma de navegarlo.
- **Elige la tipografía correcta:** te recomendamos trabajar con Google Fonts. Evitar mezclar familias tipográficas, es mejor trabajar con una o dos que tengan muchas variables (regular / bold / black / extrablack, etc). Para que una fuente se lea en la web de forma clara tiene que tener alrededor de 16px de tamaño. Los párrafos optimizados para lectura suelen tener alrededor de 10 palabras por línea de texto.
- **Arma tu propia plate cromática:** existen muchas páginas que pueden ayudarte a armar una paleta optimizada. Te recomendamos visitar:
	- [colorlouvers](https://www.colourlovers.com/)
	- [color adobe](https://color.adobe.com/es/create/color-wheel)
- **Releva sitios Webs:** en la primera etapa, es fundamental entrenar el ojo y mirar los sitios Webs que ya conoces, así como descubrir nuevos con ojos de diseñador/a. Te recomendamos visitar [awwwards](https://www.awwwards.com/), que reúne y premia los mejores sitios de la red.

---------

# Archivos
## Convenio de archivos
- No deben tener **espacios, acentos, eñes, ni símbolos** o si son palabras **usar guiones"**
- Tiene que estar escritors en **minúsculas.**
- Deben tener la etensión **".html"** (es la forma en que el servidor Web sabe que se trata un documento Web).

## Documento predeterminado
- root
	- pages
	- index.html
	- images
	- css
	- scripts
-----
# Etiquetas HTML
Las etiquetas HTML están delimitadas por un inicio y un final de cada elemento. Lo que se encuentra dentro de la etiqueta (el contenido) es lo que estás formateando.
~~~
	<etiqueta>
		Contenido
	</etiqueta>
~~~

Toda etiqueta es un juego de pares: una etiqueta abre, otra cierra.

## Atributo de las etiquetas
Todas las etiquetas aceptan atributos:
Cualquier característica que pueda ser diferente entre una etiqueta y la otra.
El valor que tendrá va entre comillas y cada una puede tener más de un atributo, separados entre sí por espacios. Los mismos sólo van en la de apertura
~~~
		<etiqueta atributo="valor">
			Contenido
		</etiqueta>
~~~
## Anidar etiquetas
Es posible meter una etiqueta dentro de la otra, de hecho, esto es más común de lo que parece. Lo más importante es tener presente que:
- Siempre se cierran en orden inverso a la apertura.
~~~
	<elemento>
		<subelemento>
		</subelemento>
	</elemento>
~~~
## Sintanxis del código
Es importante mantener el orden dentro del código e incorporar buenas prácticas:
- Manejo de tabulaciones.
- Bloques de código.

## Etiquetas cerradas y abiertas
**Las etiquetas cerradas** encierran un contenido, por lo general texto.
**Las etiquestas abiertas** sirven, entre otras cosas, para incluir elementos como imágenes, líneas, entre otros.

En el ejemplo tenemos una etiqueta cerrada llamada Párrafo ```
~~~
<p></p>
~~~
que engloba un texto y una etiqueta abierta 
~~~
<hr>
~~~
para incluir una línea horizontal. El signo "/" se utiliza para las etiquetas de cierre. En estas últimas se ponen a continuación del signo "<", mientras que en las abiertas delante del signo ">".
~~~
<p>Este es un párrafo con testo en su interior -  Etiqueta Cerrada</p>
<hr/> <!-- Esto es una línea horizontal - Etiqueta abierta -->
~~~

## Etiquetas abiertas en HTML5
Ya no es una obligación poner el signo "/". Por ejemplo:
~~~
<img src="">
~~~
Funcionará correctamente, y lo mismo sucederá con:
~~~
<br>
<hr>
~~~
los meta tag.


## Estructura básica
~~~
<head>
~~~
Es la parte privada del documento, que se utiliza como un espacio de comunicación entre el sitio Web y el navegador. Esta etiqueta envuelve otras importantes como:
~~~
<title>
<meta>
~~~
y aquellas relacionadas con la importación de documentos CSS y JS.

~~~
<body>
~~~
Encierra el contenido propiamente dicho del sitio.

**Ambos deben estar dentro de un elemento principal:** la etiqueta
~~~
<html>
~~~
