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


