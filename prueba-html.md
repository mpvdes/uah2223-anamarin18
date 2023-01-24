
# Tema 1

HTML
HTML viene de HyperText Markup Language o lenguaje de marcado hipertexto.
Es el componente más básico de la Web y define el significado y la estructura del contenido web.
Para la apariencia contamos con CSS y para la funcionalidad con JavaScript.
Utiliza marcas para etiquetar texto, imágenes y otros contenidos para mostrarlos en un navegador web.
Estas marcas incluyen elementos especiales como <head>, <title>, <body>, <header>, <footer>, <article>, <section>, <p>, <div>, <span>, etc.

## Manejo de archivos
Es importante que la estructura de los archivos en una carpeta local de tu ordenador sea la misma que después tendrá cuando se aloje en un servidor.
Esta carpeta será la raíz “/” de tu web futura.
Es importante mantener la disciplina de escribir en minúscula y sin espacios para el nombrado de archivos.
Para separar nombres se puede utilizar el guión medio  “-” pero no la barra baja ”_”

miproyectoweb/
|- assets
|     |- css
|     |    |- custom.css
|     |    |_style.css
|     |_js
|         |_custom.js
|
|- img
|     |_paisaje.jpg
|_index.html


## Elementos HTML
¿Qué es un elemento HTML?


## Atributo HTML

Si queremos cambiar el estilo de todos nuestros estilo, llamando a la clase cambiará solo a los de esa clase.

## Anidar elementos

- Bien anidado
<p>Mi gato es <strong>muy<strong> gruñón.</p>

- Mal anidado
<p>Mi gato es <strong>muy gruñón.</p></strong>


## Elementos vacíos
<img src=”https://via.placeholder.com/600x500” alt=”imagen de relleno de color rojo”>

## Elementos en bloque VS en línea
Los elementos en bloque ocupan todo el espacio del contenedor padre y comienzan nueva línea
<p>Este párrafo es un elemento en bloque; este fondo se ha colorado para mostrar el elemento principal (o padre) del párrafo.

p { background-color: #8ABB55}

Los elementos en línea van en línea del anterior y no comienzan nueva línea
            <p>Este <span>span</span> es un elemento en línea; este fondo se ha coloreado para mostrar el principio y fin de la influencia
	span { background-color: #8ABB55}


## Identificadores
Permite identificar un elemento único en una página HTML.
Solo se permite un único elemento por ID.
Sirven para hacer marcadores y saltar a esa parte de la página.
0 para dar estilos desde CSS o tareas desde JS a un único elemento.
<p id=”mi-id”>Esta frase tiene un ID único</p>

## Elementos no semánticos
- Elemento en línea <span>
Se utiliza cuando no se nos ocurre el uso de ningún otro elemento semántico de texto en el que incluir el contenido.
0 si no se desea añadir ningún significado específico
<p>El carbunco <span class=”nota-traductor”>(Nota del traductor: erróneamente llamado ántrax)</span> es una enfermedad causada por las esporas de una bacteria llamada Bacillus anthracis.</span>

- Elemento de bloque <div>
Sirve para crear secciones o agrupar contenidos.
<div style="color: blue;">
<h2> Ejemplo de div y span </h2>
 <p>
   Esto es un párrafo dentro de un div,
   <span style="color: red;"> y esto un span dentro de un párrafo.</span>
 </p>
</div>


## Estructura documento HTML
<!DOCTYPE html> Tipo de documento: HTML
<html></html> Encapsula todo el contenido de la página.
	Elemento raíz
<head></head> Contenedor de todo aquello que no es contenido visible
<meta charset=”utf-8”> Juego de carácteres
<title></title> Título de la página
<body</body> El contenido a mostrar a usuarios




## Encabezados
Hay 6 niveles de encabezado que van de <h1> a <h6>
<h1>Mi título principal</h1>
<h2>Mi título de nivel superior</h2>
<h3> Mi subtítulo</h3>
<h4>Mi  sub-subtítulo</h4>


## Vínculos
Los vínculos son los que hacen de la web, la web. Se usan con <a> que viene de anchor.
Para convertir texto dentro de un párrafo en un vínculo
Para especificar a dónde va el vínculo se hace con el atributo href:”url”
Es importante indicar el protocolo delante: http:// o https://
<p>Encontrarás toda la información sobre el máster <a href=”https://mpvd.es”>aquí</a></p>
