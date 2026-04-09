<img src="https://mauricixx.github.io/multimedial/img/Multimedial_gif.gif" width="auto" height="auto" />

#### Exploración creativa de arte, tecnología y medios digitales interactivos.

#### Cultura web y arte digital.

## Índice:
1. [Semana 1](#semana-1) <br>
2. [Semana 2](#semana-2-enlaces-links) <br>
3. [Semana 3](#semana-3-mini-sitio-3-páginas-conectadas) <br>
4. [Semana 4](#semana-4-css-intermedio-interacción-y-layout) <br>

## Semana 1:
``` html
<!DOCTYPE html>
<!-- Indica al navegador que este documento usa HTML5 -->

<html>
<!-- Inicio del documento HTML -->

<head>
<!-- Sección donde van metadatos, título y estilos -->

<meta charset="UTF-8">
<!-- Define la codificación de caracteres para que se vean bien tildes y símbolos -->

<title>Multimedial</title>
<!-- Título de la página que aparece en la pestaña del navegador -->

<style>
/* Aquí comienza la sección de estilos CSS que define la apariencia visual */

body{
/* "body" se refiere a todo el contenido visible de la página */

  background-color: white;
  /* Define que el fondo de toda la página sea blanco */

  color: black;
  /* Define que el color del texto sea negro */

  margin: 0;
  /* Elimina los márgenes que los navegadores agregan por defecto */

  height: 100vh;
  /* Hace que el alto del cuerpo sea igual al 100% de la altura de la pantalla */

  display: flex;
  /* Activa el sistema Flexbox para organizar y centrar elementos */

  justify-content: center;
  /* Centra el contenido horizontalmente */

  align-items: center;
  /* Centra el contenido verticalmente */

  font-family: Arial, sans-serif;
  /* Define la tipografía del texto */

  font-size: 60px;
  /* Define el tamaño grande del texto */

}
/* Fin de las reglas de estilo del body */

</style>
<!-- Fin de la sección de estilos -->

</head>
<!-- Fin de la sección head -->

<body>
<!-- Inicio del contenido visible de la página -->

MULTIMEDIAL
<!-- Texto que aparece en el centro de la pantalla -->

</body>
<!-- Fin del contenido visible -->

</html>
<!-- Fin del documento HTML -->
```

## Semana 2: Enlaces (links)
#### Ejemplo 1 básico:
```html
<a href="pagina2.html">Ir a la página 2</a>
```
#### Explicación:
<a> → etiqueta de enlace.
href → atributo que indica a qué página se va a enlazar.
"pagina2.html" → archivo o dirección a la que se va.
Ir a la página 2 → texto visible del enlace.
</a> → cierre de la etiqueta.

#### Cuando una persona hace clic en “Ir a la página 2”, el navegador abre pagina2.html.

### Ejemplo 2 con dos páginas:
##### index.html

```html
<!DOCTYPE html>
<html>
<head>
<title>Mi sitio</title>
</head>

<body>

<h1>Página principal</h1>

<a href="pagina2.html">Ir a la segunda página</a>

</body>
</html>
```
##### pagina2.html

```html
<!DOCTYPE html>
<html>
<head>
<title>Página 2</title>
</head>

<body>

<h1>Esta es la segunda página</h1>

<a href="index.html">Volver a la página principal</a>

</body>
</html>
```
##### Aquí ocurre algo importante:
index.html → enlaza a pagina2.html
pagina2.html → vuelve a index.html

##### Esto crea una navegación simple entre páginas.

### Ejemplo 3: Abrir el link en otra pestaña
   qué es href?
es un atributo de HTML que significa Hypertext Reference (Referencia de Hipertexto). Se utiliza principalmente dentro de la etiqueta de anclaje <a> para definir el destino de un enlace o hipervínculo, indicando al navegador la URL o archivo al que debe dirigirse al hacer clic.
```html
<a href="https://www.wikipedia.org" target="_blank">Ir a Wikipedia</a>
```
##### target="_blank" significa que el enlace se abre en una nueva pestaña.

##### Concepto clave para recordar.
##### HTML usa esta estructura:
```html
<a href="direccion">texto del enlace</a>
```
### Ejercicio extra: insertar imagenes en una página.

##### Sintaxis básica:
```html
<img src="imagen.jpg" alt="descripción">
```
##### Explicación:
src → ruta de la imagen
alt → texto alternativo (muy importante, describe la imagen)

## Semana 3: Mini sitio (3 páginas conectadas)
Objetivo: pensar en estructura + narrativa.

#### Crear 3 páginas:
index.html
obra.html
contacto.html

##### index.html:
```html
<h1>Mi sitio</h1>

<a href="obra.html">Obra</a><br>
<a href="contacto.html">Contacto</a>
```
obra.html
```html
<h1>Mi obra</h1>

<p>Descripción de mi trabajo artístico</p>

<a href="index.html">Inicio</a><br>
<a href="contacto.html">Contacto</a>
```

##### contacto.html:
```html
<h1>Contacto</h1>

<p>email@email.com</p>

<a href="index.html">Inicio</a><br>
<a href="obra.html">Obra</a>
```

### Ejercicio insertar imágenes en cada página.


##### Supongamos que tienes estas imágenes en la misma carpeta:
obra.jpg
contacto.jpg
inicio.jpg

##### Ejemplo:
##### index.html:
```html
<!DOCTYPE html>
<html>
<head>
<title>Inicio</title>
</head>

<body>

<h1>Mi sitio</h1>

<img src="inicio.jpg" alt="Imagen de inicio" width="300">

<br><br>

<a href="obra.html">Obra</a><br>
<a href="contacto.html">Contacto</a>

</body>
</html>
```
##### obra.html:
```html
<!DOCTYPE html>
<html>
<head>
<title>Obra</title>
</head>

<body>

<h1>Mi obra</h1>

<img src="obra.jpg" alt="Imagen de la obra" width="300">

<p>Descripción de mi trabajo artístico</p>

<a href="index.html">Inicio</a><br>
<a href="contacto.html">Contacto</a>

</body>
</html>
```
##### contacto.html:
```html
<!DOCTYPE html>
<html>
<head>
<title>Contacto</title>
</head>

<body>

<h1>Contacto</h1>

<img src="contacto.jpg" alt="Imagen de contacto" width="300">

<p>email@email.com</p>

<a href="index.html">Inicio</a><br>
<a href="obra.html">Obra</a>

</body>
</html>
```
##### Cosas importantes (errores comunes)
La imagen debe estar en la misma carpeta o usar rutas correctas
El nombre debe coincidir exactamente:

X Obra.jpg ≠ obra.jpg
Siempre usar alt (accesibilidad + buenas prácticas)

##### Bonus: Hacer la imagen clickeable (como link)
  ```html
<a href="obra.html">
  <img src="inicio.jpg" alt="Ir a obra" width="300">
</a>
```
Esto transforma la imagen en un botón visual.

#### Modelo a seguir con explicación línea por línea:
```html
<!DOCTYPE html> <!-- Indica al navegador que este documento usa HTML5 -->

<html> <!-- Inicio del documento HTML -->

<head> <!-- Sección de configuración (no visible en la página) -->

<title>Inicio</title> <!-- Título que aparece en la pestaña del navegador -->

</head> <!-- Cierre de la sección head -->

<body> <!-- Inicio del contenido visible de la página -->

<h1>Mi sitio</h1> <!-- Título principal grande -->

<img src="inicio.jpg" alt="Imagen de inicio" width="300"> 
<!-- Inserta una imagen:
     src = archivo de imagen
     alt = descripción de la imagen
     width = ancho en píxeles -->

<br><br> <!-- Saltos de línea para generar espacio -->

<a href="obra.html">Obra</a><br> 
<!-- Enlace a otra página llamada "obra.html" -->
<!-- <br> agrega un salto de línea -->

<a href="contacto.html">Contacto</a> 
<!-- Enlace a otra página llamada "contacto.html" -->

</body> <!-- Cierre del contenido visible -->

</html> <!-- Fin del documento HTML -->
```

#### Estructura básica de html.
##### ejemplo: Estructura usando divisiones (div) pensada para trabajar con imágenes + texto (encabezados y párrafos).

```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>Estructura con Divisiones</title>

    <style>
        /* Estilo general del cuerpo */
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            margin: 0;
        }

        /* Contenedor principal */
        .contenedor {
            width: 80%;
            margin: auto;
        }

        /* Sección o bloque */
        .bloque {
            background-color: white;
            margin: 20px 0;
            padding: 20px;
            border-radius: 10px;
        }

        /* Imagen */
        .bloque img {
            width: 100%;
            height: auto;
        }

        /* Encabezado */
        .bloque h2 {
            margin-top: 10px;
        }

        /* Texto */
        .bloque p {
            line-height: 1.5;
        }
    </style>
</head>

<body>

    <!-- Contenedor principal -->
    <div class="contenedor">

        <!-- BLOQUE 1 -->
        <div class="bloque">
            <img src="imagen1.jpg" alt="Descripción de la imagen">
            <h2>Título 1</h2>
            <p>
                Este es un texto de ejemplo. Aquí puedes escribir contenido descriptivo,
                reflexivo o informativo sobre la imagen.
            </p>
        </div>

        <!-- BLOQUE 2 -->
        <div class="bloque">
            <img src="imagen2.jpg" alt="Descripción de la imagen">
            <h2>Título 2</h2>
            <p>
                Otro texto que acompaña la imagen. Puedes trabajar narrativa,
                análisis visual o cualquier tipo de contenido.
            </p>
        </div>

        <!-- BLOQUE 3 -->
        <div class="bloque">
            <img src="imagen3.jpg" alt="Descripción de la imagen">
            <h2>Título 3</h2>
            <p>
                Este es un tercer bloque. Puedes repetir esta estructura
                tantas veces como quieras.
            </p>
        </div>

    </div>

</body>
</html>
```
```
<div> → sirve para organizar contenido en bloques
.contenedor → agrupa todo
.bloque → cada unidad de contenido (imagen + texto)
<img> → imagen
<h2> → título
<p> → párrafo
```
Es una estructura modular: puedes copiar y pegar bloques para construir una página completa.

#### Definiciones tecnicas:
```
<h2> Encabezado de nivel 2
<h2> es una etiqueta HTML de tipo heading (encabezado) que define un título jerárquico dentro del documento.
```

##### HTML tiene 6 niveles de encabezados:
```
<h1> → nivel más importante
<h2>
<h3>
<h4>
<h5>
<h6> → nivel menos importante
```
  
#### Qué significa técnicamente:
Forma parte de la estructura semántica del documento
Indica jerarquía de información
Es interpretado por:
Navegadores
Motores de búsqueda (SEO)
Lectores de pantalla (accesibilidad)

#### Comportamiento por defecto:
Se muestra en negrita
Tiene mayor tamaño que el texto normal
Genera un salto de línea antes y después (es un elemento de bloque)

#### Ejemplo:

```html
<h2>Capítulo 1</h2>
```
#### <p>: Párrafo
Definición técnica: <p> es una etiqueta HTML que define un párrafo de texto.

##### Qué significa técnicamente:
Es un elemento de tipo bloque
Agrupa contenido textual en una unidad semántica de lectura
Se usa para contenido narrativo o descriptivo

##### Comportamiento por defecto:
Agrega espacio arriba y abajo (margen)
El texto fluye en líneas automáticamente
Se adapta al ancho del contenedor

##### Ejemplo:
```html
<p>Este es un párrafo de texto.</p>
```
Esto le dice al navegador: Esto es contenido textual continuo.

##### Diferencia técnica clave:

```
--------------------------------------------------------
|  Elemento  | Tipo     |  Función                      |
--------------------------------------------------------
|  <h2>      | Heading  |  Define estructura jerárquica |
--------------------------------------------------------
|  <p>       | Texto    |  Define contenido narrativo   |
--------------------------------------------------------
```

#### Cómo trabajan juntos:

```html
<h2>El cuerpo y la máquina</h2>
<p>
Este proyecto explora la relación entre sistemas biológicos
y procesos computacionales.
</p>
```
##### Interpretación:
  
```
<h2> → introduce una idea
<p> → la desarrolla
```

####  .contenedor

Qué es técnicamente:

.contenedor es una clase de CSS.
El punto . indica que es una clase
Se aplica a uno o más elementos HTML
  ```html
   .contenedor {
    width: 80%;
    margin: auto;
  ```
##### Qué hace cada propiedad:
width: 80%; El contenedor ocupa el 80% del ancho de la pantalla
margin: auto; Centra el contenedor horizontalmente

##### Cómo se usa en HTML:
```html
<div class="contenedor">
```
##### Esto significa: “Este div va a usar los estilos definidos en .contenedor”
Interpretación conceptual

El .contenedor es como:
un marco
una caja principal
una estructura base que organiza todo
Contiene todos los bloques internos

#### .bloque

Qué es técnicamente:

También es una clase de CSS, pero pensada para repetirse.
```html
.bloque {
    background-color: white;
    margin: 20px 0;
    padding: 20px;
    border-radius: 10px;
}
```
#### Qué hace cada propiedad:
background-color: white: Fondo blanco
margin: 20px 0: Espacio arriba y abajo entre bloques
padding: 20px: Espacio interno entre el contenido y el borde
border-radius: 10px: Bordes redondeados

##### Cómo se usa en HTML:
```html
<div class="contenedor">

    <div class="bloque">
        <!-- contenido -->
    </div>

    <div class="bloque">
        <!-- contenido -->
    </div>

</div>
```
#### Diferencia Clave:
```
--------------------------------------------------------
|   Clase         |   Función                           |
--------------------------------------------------------
|   .contenedor   |   Organiza el espacio general       |
--------------------------------------------------------
|   .bloque       |   Define cada pieza de contenido    |
--------------------------------------------------------
```

 
##### .contenedor → el lienzo
##### .bloque → las composiciones

#### Punto técnico importante
Una clase (.bloque) se puede usar muchas veces
Un div puede tener varias clases:

#### Ejercicio 1:
1.	Cambiar imágenes por fotos propias
2.	Escribir un relato corto en cada bloque
3.	Modificar colores de fondo
4.	Agregar un cuarto bloque
5.	Probar cambiar el orden (texto arriba, imagen abajo)

#### Ejercicio 2:
1.	Cambien el color de .bloque
2.	Aumenten el padding a 50px
3.	Cambien el width del .contenedor a 60%
4.	Agreguen otro .bloque


## Semana 4. CSS Intermedio (Interacción y Layout)
#### Objetivo general
- Introducir hover (interacción)
- Entender flexbox (alineación)
- Controlar imágenes y proporciones
- Empezar a pensar en diseño más dinámico

#### Ejercicio 1: Efecto Hover (interacción)
##### Objetivo: Que los elementos reaccionen al mouse

##### Instrucciones:
- Crear un botón o bloque
- Cambiar su color cuando el mouse pasa encima
- Agregar una transición suave

##### Código base:
```html
<style>
.boton { /* Define una clase llamada "boton" */
  background-color: blue; /* Color de fondo del botón */
  color: white; /* Color del texto */
  padding: 15px; /* Espacio interno (arriba, abajo, izquierda, derecha) */
  width: 150px; /* Ancho fijo del botón */
  text-align: center; /* Centra el texto horizontalmente */
  transition: 0.3s; /* Hace que los cambios (como color) sean suaves en 0.3 segundos */
}

.boton:hover { /* Se activa cuando el mouse pasa sobre el elemento */
  background-color: red; /* Cambia el color de fondo al pasar el mouse */
}
</style>

<a href="https://google.com" class="boton">Ir a Google</a>
```

#### Ejercicio 2: Flexbox (alineación horizontal)

#### Objetivo: Ordenar elementos en fila

#### Instrucciones:
- Crear 3 bloques
- Alinearlos horizontalmente
- Separarlos de forma uniforme

##### Código base:
```html
<style>
.contenedor { /* Clase contenedora */
  display: flex; /* Activa flexbox: organiza los hijos en fila */
  justify-content: space-around; /* Distribuye los elementos con espacio alrededor */
}

.caja { /* Clase para cada bloque */
  background-color: lightgreen; /* Color de fondo */
  padding: 20px; /* Espacio interno */
}
</style>

<div class="contenedor"> <!-- Contenedor flex -->
  <div class="caja">1</div> <!-- Primer bloque -->
  <div class="caja">2</div> <!-- Segundo bloque -->
  <div class="caja">3</div> <!-- Tercer bloque -->
</div>
```

#### Ejercicio 3: Flexbox (centrado total)

#### Objetivo: Centrar elementos en pantalla (muy útil)

##### Instrucciones:
- Centrar un elemento en el medio exacto de la pantalla (horizontal y vertical)

##### Código base:
```html
<style>
body { /* Aplica estilos al cuerpo completo de la página */
  display: flex; /* Activa flexbox */
  justify-content: center; /* Centra horizontalmente */
  align-items: center; /* Centra verticalmente */
  height: 100vh; /* Altura total de la pantalla (viewport height) */
}

.caja { /* Elemento que será centrado */
  background-color: black; /* Fondo negro */
  color: white; /* Texto blanco */
  padding: 30px; /* Espacio interno */
}
</style>

<div class="caja">Centro</div> <!-- Elemento centrado en pantalla -->
```
#### Ejercicio 4: Imágenes controladas

#### Objetivo: Manejar imágenes correctamente

#### Instrucciones:
- Insertar una imagen
- Ajustarla para que no se deforme
- Agregar borde y estilo

##### Código base:
```html
<style>
img { /* Aplica a todas las imágenes */
  width: 300px; /* Ancho fijo */
  height: 200px; /* Alto fijo */
  object-fit: cover; /* Ajusta la imagen sin deformarla (recorta si es necesario) */
  border: 5px solid black; /* Borde negro de 5px */
}
</style>

<img src="https://upload.wikimedia.org/wikipedia/commons/8/80/Wikipedia-logo-v2.svg" /> <!-- Imagen de ejemplo -->
```
### Ejercicio 5: Composición con flex

#### Objetivo: Crear una composición visual tipo obra

##### Instrucciones:
- Crear una grilla simple usando flex
- Combinar distintos tamaños de bloques
- Usar colores como lenguaje visual

Idea:
- 1 bloque grande
- 2 medianos
- 3 pequeños

#### Barra de navegación HORIZONTAL.
```html
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<title>Navbar Horizontal</title>

<style>
body {
  margin: 0;
  font-family: Arial, sans-serif;
}

.navbar {
  background-color: #333;
  overflow: hidden;
}

.navbar a {
  float: left;
  color: white;
  text-align: center;
  padding: 14px 20px;
  text-decoration: none;
}

.navbar a:hover {
  background-color: red;
}
</style>
</head>

<body>

<div class="navbar">
  <a href="#">Inicio</a>
  <a href="#">Proyectos</a>
  <a href="#">Contacto</a>
</div>

</body>
</html>
```

#### Barra de navegación VERTICAL.
```html
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<title>Navbar Vertical</title>

<style>
body {
  margin: 0;
  font-family: Arial, sans-serif;
}

.sidebar {
  width: 200px;
  height: 100vh;
  background-color: #333;
}

.sidebar a {
  display: block;
  color: white;
  padding: 15px;
  text-decoration: none;
}

.sidebar a:hover {
  background-color: red;
}
</style>
</head>

<body>

<div class="sidebar">
  <a href="#">Inicio</a>
  <a href="#">Proyectos</a>
  <a href="#">Contacto</a>
</div>

</body>
</html>
```

##### Versión moderna (recomendada): usando FLEXBOX
```css
.navbar {
  display: flex;
  background-color: #333;
}
```
##### Vertical con Flex:
```css
.sidebar {
  display: flex;
  flex-direction: column;
}
```

#### 1. Centrar texto horizontalmente
```html
<div style="text-align: center;">
  Este texto está centrado horizontalmente
</div>
```

#### 2. Centrar texto vertical y horizontalmente (flexbox)
```html
<div style="
  display: flex;
  justify-content: center; 
  align-items: center; 
  height: 200px;
  border: 1px solid black;
">
  Texto completamente centrado
</div>
```
##### Explicación rápida:
- display: flex → activa flexbox
- justify-content: center → centra horizontal
- align-items: center → centra vertical
- height → necesario para ver el centrado vertical

#### 3. Centrar con grid (otra opción moderna).
```html
<div style="
  display: grid;
  place-items: center;
  height: 200px;
  border: 1px solid black;
">
  Texto centrado con grid
</div>
```
#### 4. Centrar usando position (más clásico).
```html
<div style="position: relative; height: 200px; border: 1px solid black;">
  <p style="
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  ">
    Texto centrado absoluto
  </p>
</div>
```





















































<!--
### MÓDULO 1: INTRODUCCIÓN Y FUNDAMENTOS (Clases 1-3)

#### Clase 1: Bienvenida a [TouchDesigner](https://derivative.ca).

**Objetivos:**
- Entender qué es TouchDesigner y sus aplicaciones
- Conocer la interfaz y navegación básica
- Crear el primer proyecto.

**Contenidos:**
- ¿Qué es TouchDesigner? Historia y usos profesionales
- Instalación y configuración inicial
- Tour por la interfaz: Network Editor, Palette, Parameters
- Conceptos: Operators (OPs), familias de operadores
- Navegación: zoom, pan, conexiones
- Proyecto práctico: "Hola Mundo" visual

**Tarea:**
Explorar la interfaz y crear 3 pequeñas redes usando diferentes familias de OPs

#### - Qué es TouchDesigner? 
> Es un lenguaje de programación visual basado en nodos para contenido multimedia interactivo en tiempo real . Desarrollado por la empresa  ["Derivative"](https://derivative.ca) de Toronto, es utilizado frecuentemente por artistas, programadores, codificadores creativos, diseñadores de software y artistas para crear performances, instalaciones y obras multimedia fijas. [1](https://en.wikipedia.org/wiki/TouchDesigner)

### Clase 2: Las Familias de Operadores
**Duración:** 90 minutos

**Objetivos:**
- Comprender las 6 familias de operadores
- Entender el flujo de datos en TouchDesigner
- Crear conexiones básicas

**Contenidos:**
- TOPs (Texture Operators) - Procesamiento de imágenes 2D
- CHOPs (Channel Operators) - Datos numéricos y animación
- SOPs (Surface Operators) - Geometría 3D
- MATs (Materials) - Shaders y texturas
- DATs (Data Operators) - Texto y datos
- COMPs (Components) - Contenedores y componentes
- Conectar diferentes familias
- Ejercicio: Cadena simple con cada familia

**Tarea:**
Crear un diagrama de red usando al menos 4 familias diferentes

---
-->


