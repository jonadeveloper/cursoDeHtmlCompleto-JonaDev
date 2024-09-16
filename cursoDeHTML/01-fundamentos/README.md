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
    <p></p>
  </li>
  <li>
    <h3>Head</h3>
    <p></p>
  </li>
  <li>
    <h3>Body</h3>
    <p></p>
  </li>
</ol>
