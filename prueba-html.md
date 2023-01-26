
# Tema 1

HTML
HTML viene de HyperText Markup Language o lenguaje de marcado hipertexto.
Es el componente más básico de la Web y define el significado y la estructura del contenido web.
Para la apariencia contamos con CSS y para la funcionalidad con JavaScript.
Utiliza marcas para etiquetar texto, imágenes y otros contenidos para mostrarlos en un navegador web.
Estas marcas incluyen elementos especiales como `<head>`, `<title>`, `<body>`, `<header>`, `<footer>`, `<article>`, `<section>`, `<p>`, `<div>`, `<span>`, etc.

## Manejo de archivos
Es importante que la estructura de los archivos en una carpeta local de tu ordenador sea la misma que después tendrá cuando se aloje en un servidor.
Esta carpeta será la raíz “/” de tu web futura.
Es importante mantener la disciplina de escribir en minúscula y sin espacios para el nombrado de archivos.
Para separar nombres se puede utilizar el guión medio  “-” pero no la barra baja ”_”


## Elementos HTML
¿Qué es un elemento HTML?


## Atributo HTML

Si queremos cambiar el estilo de todos nuestros estilo, llamando a la clase cambiará solo a los de esa clase.

## Anidar elementos

- Bien anidado
`<p>Mi gato es <strong>muy<strong> gruñón.</p>`

- Mal anidado
`<p>Mi gato es <strong>muy gruñón.</p></strong>`


## Elementos vacíos
`<img src=”https://via.placeholder.com/600x500” alt=”imagen de relleno de color rojo”>`

## Elementos en bloque VS en línea
Los elementos en bloque ocupan todo el espacio del contenedor padre y comienzan nueva línea
`<p>Este párrafo es un elemento en bloque; este fondo se ha colorado para mostrar el elemento principal (o padre) del párrafo.

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
Es importante indicar el protocolo delante: `http://` o `https://`
`<p>Encontrarás toda la información sobre el máster <a href=”https://mpvd.es”>aquí</a></p>`


## Importancia
`em`realza la importancia del texto que encierra.
`strong`realza la máxima importancia del texto que encierra.
`<p>El concierto de <em>Rock Paradise</em> tendrá lugar el día 24 de enero a las 19:30, será <strong>obligatorio presentar...

## Cita
Con <blockquote> hacemos una cita textual de otro texto externo.
Este elemento puede tener el atributo `cite="url" para enlazar la fuente.
Podemos indicar la autoría, documento o fuente de la cita con <cite>

Desde la <cite>OCU</cite> señalan lo siguiente:
<blockquote cite="https://www.ocu.org/fincas-y-casas/glosario-inmobiliario/c/cooperativas-de-vivienda">Ahora mismo hay muy...

## Abreviatura y acrónimo
Para abreviatura utilizamos `<abbr>`
Para un acrónimo o uso de siglas lo hacemos con `<acronym>`
En el atributo `title` podemos indicar el significado de esa abreviatura o acrónimo.

`<p>El <acronym title="World Wide Web Consortium">W·C</acronym> es quien define el estándar <abbr title="HyperText Markup Language">HTML</abbr>

## Definición
Para indicar una definición lo hacemos con `<dfn>`
El elemento que lo encierra es el contexto de la definición.
`<p>A <dfn id="def-validator">validator</dfn> is a program that checks for syntax errors in code or documents.</p>`

## Inserción y borrado
Cuando queremos borrar o modificar contenido en una publicación realizada.
Con `<ins>` indicamos la modificación y quedará subrayado.
Con `<del>`indicamos el borrado y quedará tachado.
En el atributo `cite` pude indicar la fuente por la que se realiza tal borrado o modificación.
Y con `datetime`la fecha de la modificación.
`<p> El origen del terremoto fue en <del>Burriana</del><ins>Lorca</ins></p>`

## Tiempo
El elemento `<time>`representa un periodo específico de tiempo.
con el atributo datetime hacemos que este elemento sea machine-readable.
Esto es una mejora para los resultados de motores de búsqueda o para funciones personalizadas como recordatorios.
[Mirar aquí](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/time#valid_datetime_values)

##Preformateado de texto
Cuando queremos mostrar el texto preformateado y escrito tal y como lo hacemos en el HTML.
Se suele renderizar en el navegador con una fuente monoespaciada.
Se respetan los espacios en blanco.
Escape de caracter: < (&lt), > (&gt), & (&amp), " (&quot) 

## Mostrar código
Para mostrar podemos hacerlo con el elemento `<code>`
Normalmente se renderiza con fuente monoespaciada
`<p> The function <code>selectAll()</code> highlights all the text in the input field so the user can, for example, copy or`

Si queremos mostrar múltiples líenas de código podemos encerrarlo dentro de `<pre>`

<pre>
   <code>
	body {
	   padding: 0;
	   margin: 0;
	   box-sizing: border-box;
	 }
   </code>
</pre>


## Otros enlaces
Para enlazar con un script de javascript por ejemplo, podemos hacerlo con el elemento `<script>`
"<head>
   <script type="text/javascript" src="http://www.ejemplo.com/ja/inicializar.js"></script>
 </head>"

Con `<script>`también podemos escribir el código JS directamente en nuestro HTML
 <script type="text/javascript">
   window.onload = function() { alert("La página se ha cargado completamente"); }

Si queremos enlazar con otros recursos, como por ejemplo una hoja de estilo CSS, podemos hacerlo con el elemento <link>

<head>
   <link rel="stylesheet" type="text/css" href="/css/style.css" />
</head>
