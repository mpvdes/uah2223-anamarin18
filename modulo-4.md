# CSS
- CSS (hoja de estilo en cascada) es el código que utilizamos para dar estilo a la web.
- Podemos dar color, tamaño al texto o el fondo de elementos, la maquetación de los mismos, etc.
- No es un lenguaje de programación ni de marcado. Es un lenguaje de hojas de estilo.
- Permite aplicar estilos de manera selectiva o "en cascada" a elementos en el HTML.


Si queremos cambiar el color de texto a todos los párrafos:
`p {
   color: red;
 }`

## Configuración
- Para que tengan efectos estos estilos tenemos que guardarlo en un archivo `.css`.
- Y además tendremos que vincular este archivo desde el html entr las etiquetas `<head>`y `</head>`.

`<link href="assets/css/style.css" rel="stylesheet" type="text/css">`

## Sintaxis
- Cada una de las reglas deben estar encapsuladas entre llavesm"{}".
- Usar los dos puntos ":" para separar la propiedad de su valor.
- Usar el punto y coma ";" para separar una declaración de la siguiente.

`p {
   color: red;
   width: 500px;
   border: 1px solid black;
 }`


## Cajas
- Podemos pensar los elemento HTML como cajas apiladas una sobre otra.
- Cada caja tiene una serie de propiedades como estas:
	- padding (relleno), el espacio alrededor del contenido	
	- border (marco), la línea que se encuentra fuera del relleno
	- margin (margen), el espacio fuera del elemento que lo separa de los demás


## Fuentes
- Para dar estilo al texto también podemos hacerlo utilizando diferentes fuentes o tipografías.
- Para utilizar una fuente desde css lo podemos hacer con la propiedad `font-family`.
- El navegador sólo podrá utilizar las tipografías que tengamos instaladas en el sistema
- Existe un listado de fuentes web seguras

`p {
   font-family: arial;

}`


## Webfonts
Si queremos 
googlefonts por ejemplo, otro fontlibrary, 
