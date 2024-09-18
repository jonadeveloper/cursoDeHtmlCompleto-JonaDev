![Copia de githubport (2)](https://github.com/user-attachments/assets/42f3bf81-ca19-4019-9983-32b3cbf93cc3)

<h1 align="center">Comencemos por lo escencial</h1>

<p align="center"><em>En esta primera parte vamos a ocuparnos de entender que es HTML, como funciona y todo lo elemental para comenzar a trabajar.</em></p>

<h3>Que es HTML</h3>
<p>HTML (HyperText Markup Language) es el lenguaje estándar para crear páginas web. Es importante aclarar que HTML NO es un lenguaje de programación. Aun asi, me atreveria a decir que, es el lenguaje mas importante de todos a la hora de crear proyectos web. Ya que HTML es el lenguaje estandar que se ocupa de estructurar los sitios web, mediante el uso de etiquetas o tags.</p>

<h3>Como funciona HTML</h3>
<p>Lo primero que tenemos que entender es que HTML es un lenguaje interpretado. ¿Que significa esto? Basicamente, los navegadores web (como chrome, firefox, opera,etc.) actuan como interpretes de su codigo. Esto significa que el navegador lee el archivo HTML, lo procesa y lo convierte en una representación visual en pantalla, interpretando cada etiqueta o elemento en tiempo real. Pero, ¿como logra ese proceso para interpretarlo de manera correcta? Ahi es donde entran en juegos la etiquetas, tambien conocidad como tags. Podriamos decir que las etiquetas son palabras claves encerradas entre corchetes angulares (<>). Cada etiqueta tiene un significado y proposito especifico. Mas adelante vamos a ver las diferentes etiquetas y su correcto uso. Aclarado esto, el navegador hace el proceso de interpretación de la siguiente manera:</p>
<ol>
  <li>
    <strong>Interpretar la estructura:</strong> Las etiquetas de HTML definen la estructura y el contenido de una página web, y el navegador traduce esas etiquetas en elementos visuales como encabezados, párrafos, imágenes, etc.
  </li>
  <li>
    <strong>Renderizado en tiempo real:</strong> El HTML es interpretado en el momento de ser cargado, lo que permite a los desarrolladores ver los cambios inmediatamente al actualizar la página.
  </li>
</ol>

![Copia de githubport (3)](https://github.com/user-attachments/assets/3a077dd6-cce1-4944-b294-4edda1bf2bbd)

<h1 align="center">Empecemos a trabajar</h1>

<p align="center"><em>Vamos de una vez directo a nuestro editor de codigo y pongamos manos a la obra.</em></p>

<h3>Crea tu primer archivo HTML</h3>

<p>Para empezar a trabajar con HTML, lo primero que vamos a hacer es crear un archivo al que llamaremos index.html (el nombre no es obligatorio pero se utiliza por convencion). El .html es el que indica que tipo de archivo. Al igual que una imagen puede terminar con .jpg o un archivo de texto plano con .txt. Si dentro de el archivo escribimos cualquier texto simple, como por ejemplo el tipico "Hola mundo" y lo ejecutamos en el navegador vamos a poder ver el resultado sin ningun problema. Pero, asi no es como se trabaja con HTML.</p>

<h3>Estructura basica de HTML</h3>

<p>Como dijimos anteriormente, HTML trabaja con etiquetas,algunas simples y otras compuestas(etiquetas de apertura y cierre). Cada una tiene un proposito especifico. En esta oportunidad vamos a hablar de las etiquetas que componen la estructura basica de un archivo HTML.</p>
<ol>
  <li>
    <h3>Doctype</h3>
    <p>Esta etiqueta es la declaración de version de HTML. Actualmente HTML se encuentra en la version HTML 5.</p>
    
```html  
<!DOCTYPE html>
```

  </li>
  <li>
    <h3>Html</h3>
    <p>La etiqueta html (de apertura y de cierre) es donde inicia y termina nuestro documento. Envuelve todo el contenido que compone el sitio. Por ende, las dos etiquetas faltantes que componen la estructura(head y body), se ubican dentro de esta.</p>

```html  
<html>
  
</html>
```
  </li>
  <li>
    <h3>Head</h3>
    <p>La etiqueta head es la que contiene los metadatos e información sobre la pagina. Estos datos no son visibles en la web (con una excepción), pero afectan directamente el comportamiento, la presentación y las interacciones del documento.</p>

```html
 
<head>
  <title>Bienvenidos a mi web</title>
</head>

```
    
  </li>
  <li>
    <h3>Body</h3>
    <p>Por ultimo,el body es una etiqueta que define el cuerpo del documento web, es decir, la sección donde se coloca todo el contenido visible que será mostrado en el navegador.</p>

```html
 
<body>
  <h1>Bienvenidos a mi web</h1>
</body>

```
  </li>
</ol>

<p>Llegados a este punto, la estructura <strong>básica</strong> deberia estar terminada y deberia verse de la siguiente manera:</p>

```html

<!DOCTYPE html>
<html>
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <h1>Bienvenidos a mi web</h1>
  </body>
</html>

```

<p>Pero, para continuar tenemos que ver otro concepto de HTML. <strong>Los atributos.</strong></p>

<h3>Que son los atributos</h3>

<p>Los atributos en HTML son características o propiedades que se aplican a los elementos o etiquetas para proporcionar información adicional o modificar su comportamiento. Estos atributos suelen aparecer dentro de las etiquetas de apertura de los elementos HTML y afectan cómo se muestran o funcionan los elementos en la página web. Los atributos se componen por su nombre y su valor entre comillas(""), separados por un signo igual(=). Por ejemplo, la etiqueta <html> cuenta con el atributo lang, el cual define el idioma del documento.</p>

```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <h1>Bienvenidos a mi web</h1>
  </body>
</html>

```

<p align="center">En este ejemplo, el atributo lang define el idioma español para el documento.</p><br>

![Copia de githubport (4)](https://github.com/user-attachments/assets/0c1019f9-bbf1-48b3-be65-2ce477e4f50d)

<h2 align="center">Comencemos con las primeras etiquetas</h2>

<p align="center"><em>Aunque recien estamos empezando, ya vamos incorporando conceptos. Ya tenemos claro cual es la estructura basica de un documento, que son las etiquetas y los atributos. Sigamos avanzando. Veamos algunas de las etiquetas basicas del lenguaje.</em></p>

<h2 align="center">Etiquetas de texto</h2>

<ol>
  <li>
    <h3>Etiquetas de encabezado</h3>
    <p>Estas etiquetas definen los encabezados de una página web, y su jerarquía va desde h1, el más importante, hasta h6, el menos importante.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <h1>Bienvenidos a mi web</h1>
    <h2>Bienvenidos a mi web</h2>
    <h3>Bienvenidos a mi web</h3>
    <h4>Bienvenidos a mi web</h4>
    <h5>Bienvenidos a mi web</h5>
    <h6>Bienvenidos a mi web</h6>
  </body>
</html>

```
    
  </li>
  <li>
    <h3>Etiqueta de parrafo</h3>
    <p>Se utiliza para contener bloques de texto, lo que equivale a un párrafo en un documento.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <p>Hola, esto es un parrafo</p>
  </body>
</html>

```
    
  </li>
  <li>
    <h3>Etiquetas de texto en negrita</h3>
    <p>Las dos etiquetas que veremos a continuación(b , strong), se utilizan para destacar un texto en negrita. Visualmente son iguales, pero con una diferencia semantica que veremos mas adelante.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <p>Hola, esto es un <b>parrafo</b></p>
    <p>Hola, esto es un <strong>parrafo</strong></p>
  </body>
</html>

```
    
  </li>
  <li>
    <h3>Etiquetas de texto en cursiva</h3>
    <p>Las dos etiquetas que veremos a continuación(em , i), son similares a las anteriores. Se utilizan para transformar un texto en cursiva. Visualmente son iguales, pero al igual que las anteriores,tienen una diferencia semantica que veremos mas adelante.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <p>Hola, <em>este es un texto en cursiva</em</p>
    <p>Hola, <i>este es un texto en cursiva</i></p>
  </body>
</html>

```
    
  </li>
  <li>
    <h3>Etiquetas de texto pequeño</h3>
    <p>Representa un texto de menor importancia o una nota aclaratoria.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <p>Todos los derechos reservados. <small>(c) 2024 JonaDev</small></p>
  </body>
</html>

```
    
  </li>
  <li>
    <h3>Etiqueta de cita en bloque</h3>
    <p>Indica que el contenido es una cita en bloque de otro autor.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <blockquote>
  "No se trata solo de conectar computadoras, se trata de conectar personas." - Tim Berners Lee
    </blockquote>
  </body>
</html>

```
    
  </li>
  <li>
    <h3>Etiqueta de codigo</h3>
    <p>Define fragmentos de código en el texto, mostrando el texto con una fuente monoespaciada.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <p>Para capturar un elemento HTML por su ID , utiliza la función <code>document.getElementById</code>.</p>
  </body>
</html>

```
    
  </li>
  <li>
    <h3>Etiqueta de texto formateado</h3>
    <p>Mantiene el formato original del texto, incluyendo los saltos de línea y los espacios en blanco. Ideal para mostrar bloques de código o texto con un formato específico.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <pre>
      function saludo() {
        console.log('Hola Mundo');
      }
    </pre>

  </body>
</html>

```
    
  </li>
</ol>
