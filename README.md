# CSS: 1-Intro

# 1 Conectar HTML Y CSS
- Primera opción:
Esta es la mejor opción.
Crear carpeta `css` y dentro de ella archivo `styles.css` y conectamos la hoja `sytles.css` en el archivo `index.html` con la etiqueta `link`.
~~~html
<head>
    <link rel="stylesheet" href="./css/styles.css">
    <title>Conectar HTML y CSS</title>
</head>
~~~

- Segunda opción:
Con la etiqueta `sytle`.
~~~html
     <style>
        body{
            background-color: red;
        }
    </style>
~~~
- Tercera opción:
Esta opción no es nada recomendable.
~~~html
<h1 style='background-color: blue;'>Conectar HTML y CSS</h1>
~~~
- Cuarta opción:
Tampoco es recomendable. 
Es usando `@import`.
No usar nunca, si se puede evitar. Porque tiene un retardo a la hora de cargar los estilos.


~~~html
    <style>
      @import url(./css/styles.css);
    </style>
~~~

# 2 Sintaxis de CSS
Selector: Elemento al que le vamos aplicar la propiedad.

Propiedad: lo que vamos a cambiar

Valor: El nuevo valor que va a tener

Propiedad Valor: -> Se le denomina declaración

Al conjunto de selector: Declaraciòn(es) se le denomina regla.

~~~html
body{
    background-color:aqua;
}
~~~

# 3 Tipos de selectores
Selectores simples
- selectores elementales
  - Selector universal -> `*`
  - Selector de tipo o de etiqueta -> Nombre de la etiqueta
- selectores de atributo
  - id -> id del elemento
  - clase -> clase del elemento
  - otros atributos.
       [atributo]
       [atributo=valor]
       [atributo^=valor]
       [atributo*=valor]
       [atributo$=valor]
       [atributo|=valor]

Selectores compuestos
- selectores agrupados
- selectores combinadores
- Pseudoclaases

## Selectores elementales
### Selector universal `*`
~~~css
*{
    background-color: blue;
}
~~~
### Selector de etiqueta
~~~css
h1 {
    background-color: green;
}
p {
    background-color: lightcoral;
}
~~~
### Selector de Id y selectores de clase
- id
Le damos un identificador a una etiqueta en el archivo `index.html` 
~~~html
<h1 id="title">Conectar HTML y CSS</h1>
~~~
Y en el archivo `styles.css` con la  `#` y el nombre del indentificador cambiamos la propiedades.
~~~css
#title{
    background-color: blueviolet;
}
~~~
- clase

~~~html
<h1 class="title">Tipo de Selectores</h1>
~~~
`.title` es como se especifica en css que es una clase
~~~css
.title{
    background-color: cyan;
}
~~~
### Selector de atributo
~~~html
<a href="https://www.youtube.com/">youtube</a>
    <a href="color-modo-random">color random</a>
    <a href="#seccion-verde">color verde</a>
    <a href="color-rojo">color rojo</a>
    <p lang="es">Lorem ipsum</p>
~~~
~~~css
[href]{
    background-color: gray;
}
[href="https://www.youtube.com/"]
{
    background-color: darkorange;
}
[href^="color"]{
    background-color:greenyellow;
}
[href*="modo"]{
    background-color:green;
}
[href$="rojo"]{
    background-color:red;
}
[lang|="es"]{
    background-color:blue;
}

~~~