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
