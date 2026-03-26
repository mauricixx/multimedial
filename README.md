<img src="https://mauricixx.github.io/multimedial/img/Multimedial_gif.gif" width="auto" height="auto" />

#### Exploración creativa de arte, tecnología y medios digitales interactivos.

#### Cultura web y arte digital.

##### Ejercico 1, semana 1:
``` 
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

## Ejercico 2, semana 2: Enlaces (links)
### Ejemplo 1 básico:
```
<a href="pagina2.html">Ir a la página 2</a>
```
### Explicación:
<a> → etiqueta de enlace.
href → atributo que indica a qué página se va a enlazar.
"pagina2.html" → archivo o dirección a la que se va.
Ir a la página 2 → texto visible del enlace.
</a> → cierre de la etiqueta.

#### Cuando una persona hace clic en “Ir a la página 2”, el navegador abre pagina2.html.

### Ejemplo 2 con dos páginas:
##### index.html
```
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
```
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
```
<a href="https://www.wikipedia.org" target="_blank">Ir a Wikipedia</a>
```
##### target="_blank" significa que el enlace se abre en una nueva pestaña.

##### Concepto clave para recordar.
##### HTML usa esta estructura:
```
<a href="direccion">texto del enlace</a>
```
### Ejercicio insertar imagenes en una página.

##### Sintaxis básica:
```
<img src="imagen.jpg" alt="descripción">
```
##### Explicación:
src → ruta de la imagen
alt → texto alternativo (muy importante, describe la imagen)

### Ejercicio: Mini sitio (3 páginas conectadas)
Objetivo: pensar en estructura + narrativa.

#### Crear 3 páginas:
index.html
obra.html
contacto.html

##### index.html:
```
<h1>Mi sitio</h1>

<a href="obra.html">Obra</a><br>
<a href="contacto.html">Contacto</a>
```
obra.html
```
<h1>Mi obra</h1>

<p>Descripción de mi trabajo artístico</p>

<a href="index.html">Inicio</a><br>
<a href="contacto.html">Contacto</a>
```

##### contacto.html:
```
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
```
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
```
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
```
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
  ```
<a href="obra.html">
  <img src="inicio.jpg" alt="Ir a obra" width="300">
</a>
```
Esto transforma la imagen en un botón visual.

#### Modelo a seguir con explicación línea por línea:
```
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


