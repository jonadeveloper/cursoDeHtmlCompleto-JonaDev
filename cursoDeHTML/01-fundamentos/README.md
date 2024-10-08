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

![Copia de githubport (5)](https://github.com/user-attachments/assets/b79690b5-7fd1-48c0-8717-6bcfe43c79d7)

<h2 align="center">Comencemos con las primeras etiquetas</h2>

<p align="center"><em>Aunque recien estamos empezando, ya vamos incorporando conceptos. Ya tenemos claro cual es la estructura basica de un documento, que son las etiquetas y los atributos. Sigamos avanzando. Veamos algunas de las etiquetas del lenguaje.</em></p>

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
    <h3>Etiqueta de enlace</h3>
    <p>Define un hipervínculo que conecta el contenido actual con otra página web, sección del documento, archivo o recurso.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <a href="https://www.instagram.com/jona.dev_ok/">Para estar al tanto de todas las novedades, seguime en instagram</a>
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
  <li>
    <h3>Etiqueta de texto resaltado</h3>
    <p>Marca el texto como destacado o resaltado, similar a un marcador de texto en papel.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <p>Recorda estudiar <mark>HTML semántico</mark> para mejorar la accesibilidad.</p>
  </body>
</html>

```
    
  </li>
  <li>
    <h3>Etiqueta de texto tachado y texto insertado</h3>
    <p>Estas etiquetas indican que el texto ha sido eliminado o tachado o bien que el texto ha sido agregado o insertado recientemente</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <p>El curso de HTML <del>inicia mañana</del>, ya esta disponible.</p>
    <p>La segunda sección del curso <ins>estara disponible en unas horas</ins>.</p>
  </body>
</html>

```
    
  </li>
  <li>
    <h3>Etiqueta de abreviatura</h3>
    <p>Define una abreviatura, y al pasar el cursor sobre ella, se puede mostrar el significado completo.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <p>El <abbr title="World Wide Web">WWW</abbr> es un sistema de documentos interconectados.</p>
  </body>
</html>

```
    
  </li>
</ol>

<h2 align="center">Etiquetas de listas</h2>

<ol>
  <li>
    <h3>Listas desordenadas</h3>
    <p>Estas listas no tienen un orden específico y los elementos son presentados con viñetas.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <ul>
      <li>Desarrollo Web</li>
      <li>Programación</li>
      <li>Diseño UX/UI</li>
    </ul>
  </body>
</html>
```

  </li>
  <li>
    <h3>Listas ordenadas</h3>
    <p>Estas listas se utilizan cuando el orden de los elementos es importante. Los elementos de la lista están numerados automáticamente.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <ol>
      <li>Aprender HTML</li>
      <li>Estudiar CSS</li>
      <li>Dominar JavaScript</li>
    </ol>
  </body>
</html>
```

  </li>
  <li>
    <h3>Listas de definición</h3>
    <p>Estas listas son para definir términos y sus descripciones.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <dl>
      <dt>HTML</dt>
      <dd>Lenguaje de marcado utilizado para estructurar el contenido de la web.</dd>
      <dt>CSS</dt>
      <dd>Lenguaje de estilos utilizado para darle formato visual a una página web.</dd>
    </dl>
  </body>
</html>
```

  </li>
</ol>

<h2 align="center">Etiquetas de tablas</h2>

<ol>
  <li>
    <h3>Etiqueta contenedora principal</h3>
    <p>Contiene todas las demás etiquetas relacionadas con la tabla, como filas y celdas.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <table>
      <!-- Contenido de la tabla va aquí -->
    </table>
  </body>
</html>
```

  </li>
  <li>
    <h3>Etiqueta de fila</h3>
    <p>La etiqueta tr define una fila dentro de la tabla. Contiene las celdas, ya sean de encabezado o de datos.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <tr>
      <td>Celda 1</td>
      <td>Celda 2</td>
    </tr>
  </body>
</html>
```

  </li>
  <li>
    <h3>Etiqueta de encabezado</h3>
    <p>La etiqueta th se utiliza para marcar celdas que contienen títulos o descripciones de los datos de una tabla, generalmente al principio de cada columna o fila. Los navegadores suelen mostrar estas celdas en negrita y alineadas al centro.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <tr>
      <th>Producto</th>
      <th>Precio</th>
    </tr>
  </body>
</html>
```

  </li>
  <li>
    <h3>Etiqueta de celda de datos</h3>
    <p>La etiqueta td, se utiliza para contener los datos dentro de cada fila y columna de la tabla. Es el contenido principal de la tabla.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <tr>
      <td>Manzana</td>
      <td>$1</td>
    </tr>
  </body>
</html>
```

  </li>
  <li>
    <h3>Etiqueta de agrupación de cabecera</h3>
    <p>La etiqueta thead, agrupa el conjunto de celdas de encabezado en una tabla. Contiene las etiquetas tr y th para la cabecera de la tabla.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <thead>
      <tr>
        <th>Producto</th>
        <th>Precio</th>
      </tr>
    </thead>
  </body>
</html>
```

  </li>
  <li>
    <h3>Etiqueta de agrupación del cuerpo de la tabla</h3>
    <p>La etiqueta tbody, agrupa el contenido del cuerpo de la tabla, separándolo de la cabecera y el pie. Dentro de esta etiqueta se encuentran las filas tr que contienen los datos td.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <tbody>
      <tr>
        <td>Manzana</td>
        <td>$1</td>
      </tr>
      <tr>
        <td>Banana</td>
        <td>$2</td>
      </tr>
    </tbody>
  </body>
</html>
```

  </li>
   <li>
    <h3>Etiqueta de agrupación del pie de la tabla</h3>
    <p>La etiqueta tfoot, agrupa las celdas que contienen el pie de la tabla, que a menudo incluyen totales o resúmenes. Se coloca normalmente después del cuerpo de la tabla y antes del cierre de la etiqueta table.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <tfoot>
      <tr>
        <td>Total</td>
        <td>$3</td>
      </tr>
    </tfoot>
  </body>
</html>
```

  </li>
  <li>
    <h3>Etiqueta de titulo o descripción de la tabla</h3>
    <p>La etiqueta caption, proporciona un título o una breve descripción de la tabla. Se coloca justo después de la apertura de la etiqueta table y ayuda a los usuarios a entender rápidamente el contenido de la tabla.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <table>
      <caption>Lista de precios de frutas</caption>
      <!-- Resto de la tabla -->
    </table>
  </body>
</html>
```

  </li>
  <li>
    <h3>Etiqueta para definir estilos de la tabla</h3>
    <p>Las etiquetas col y colgroup, permiten definir grupos de columnas dentro de una tabla para aplicar estilos específicos. Aunque no tienen contenido propio, ayudan a estructurar visualmente las tablas.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <colgroup>
      <col span="2" style="background-color: lightgray;">
    </colgroup>
  </body>
</html>
```

  </li>
</ol>

<h3>Aqui un ejemplo de tablas utilizando todas las etiquetas explicadas</h3>

```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <table>
    <!-- Título o descripción de la tabla -->
      <caption>Precios de Productos por Tienda</caption>
    
    <!-- Definir el estilo de las columnas -->
      <colgroup>
        <col span="1">
        <col span="1">
        <col span="1" style="background-color: lightgreen;">
      </colgroup>
    
    <!-- Cabecera de la tabla -->
      <thead>
        <tr>
          <th>Producto</th>
          <th>Tienda A</th>
          <th>Tienda B</th>
        </tr>
      </thead>
    
    <!-- Cuerpo de la tabla -->
    <tbody>
      <tr>
        <td>Manzana</td>
        <td>$1</td>
        <td>$1.20</td>
      </tr>
      <tr>
        <td>Banana</td>
        <td>$0.80</td>
        <td>$0.75</td>
      </tr>
      <tr>
        <td>Naranja</td>
        <td>$0.90</td>
        <td>$0.95</td>
      </tr>
    </tbody>
    <!-- Pie de la tabla -->
    <tfoot>
      <tr>
        <td>Total</td>
        <td>$2.70</td>
        <td>$2.90</td>
      </tr>
    </tfoot>
  </table>
  </body>
</html>
```

<h2 align="center">Etiquetas de formularios</h2>

<ol>
  <li>
    <h3>Etiqueta contenedora del formulario</h3>
    <p>Es el contenedor principal que engloba todos los elementos del formulario.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <form action="/enviar-datos" method="POST">
      <!-- Campos de formulario -->
    </form>
  </body>
</html>
```

  </li>
  <li>
    <h3>Etiqueta de campo de entrada de datos</h3>
    <p>Campo que permite al usuario ingresar información. Es uno de los elementos más versátiles y puede adoptar varios tipos según el valor del atributo type.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <input type="text" name="nombre" placeholder="Escribe tu nombre">
  </body>
</html>
```

  </li>
  <li>
    <h3>Etiqueta descriptiva</h3>
    <p>La etiqueta label, proporciona una descripción semántica para los campos del formulario.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <label for="nombre">Nombre:</label>
    <input type="text" id="nombre" name="nombre">
  </body>
</html>
```

  </li>
  <li>
    <h3>Etiqueta de area de texto</h3>
    <p>La etiqueta textarea, se utiliza cuando se necesita que el usuario ingrese grandes cantidades de texto, como comentarios o mensajes.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <textarea name="comentarios" placeholder="Escribe tus comentarios"></textarea>
  </body>
</html>
```

  </li>
  <li>
    <h3>Etiqueta de botón</h3>
    <p>La etiqueta button es un elemento interactivo que permite al usuario enviar o ejecutar acciones dentro del formulario. Puede ser de tipo submit (enviar datos del formulario), reset (restablecer el formulario) o button (botón sin acción predeterminada).</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <button type="submit">Enviar</button>
  </body>
</html>
```

  </li>
  <li>
    <h3>Etiqueta de menú desplegable</h3>
    <p>La etiqueta select, crea un menú desplegable que permite al usuario seleccionar una opción. Se utiliza junto a la etiqueta option(dentro de select), que define las opciones del menu.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <label for="pais">País:</label>
      <select id="pais" name="pais">
        <option value="ar">Argentina</option>
        <option value="mx">Francia</option>
      </select>
  </body>
</html>
```

  </li>
  <li>
  <h3>Etiqueta de grupo de opciones</h3>
    <p>Agrupa opciones relacionadas dentro de un menú desplegable.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <select name="ciudad">
      <optgroup label="Argentina">
        <option value="buenos_aires">Buenos Aires</option>
        <option value="cordoba">Córdoba</option>
      </optgroup>
      <optgroup label="Francia">
        <option value="paris">Paris</option>
        <option value="marsella">Marsella</option>
      </optgroup>
    </select>
  </body>
</html>
```

  </li>
  <li>
    <h3>Etiqueta de agrupación de campos</h3>
    <p>La etiqueta fieldset agrupa conjuntos de campos que están relacionados dentro de un formulario. Y la etiquta legend le da un titulo a la agrupación de campos.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <fieldset>
      <legend>Información Personal</legend>
      <label for="nombre">Nombre:</label>
      <input type="text" id="nombre" name="nombre">
    </fieldset>
  </body>
</html>
```

  </li>
  <li>
    <h3>Etiqueta de barra de progreso</h3>
    <p>La etiqueta progress representa una barra de progreso que muestra el avance de una tarea.</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <progress value="70" max="100">70%</progress>
  </body>
</html>
```

  </li>
  <li>
    <h3>Etiqueta de medidor</h3>
    <p>La etiqueta meter (similar a progress) representa un medidor dentro de un rango conocido (por ejemplo, capacidad de almacenamiento).</p>
    
```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <label for="nivel">Nivel de batería:</label>
    <meter id="nivel" value="0.6" min="0" max="1">60%</meter>
  </body>
</html>
```

  </li>
</ol>

<h3>Aqui un ejemplo de de formulario.</h3>

```html

<!DOCTYPE html>
<html lang="es">
  <head>
    <title>Bienvenidos a mi web</title>
  </head>
  <body>
    <form>
      <fieldset>
      <legend>Información Personal</legend>
        <label for="nombre">Nombre:</label>
        <input type="text" id="nombre" name="nombre" required>
      </fieldset>
  
      <fieldset>
        <legend>Preferencias</legend>
        <label for="pais">País:</label>
        <select id="pais" name="pais">
          <option value="ar">Argentina</option>
          <option value="fr">Francia</option>
        </select>
  
        <label for="comentarios">Comentarios:</label>
        <textarea id="comentarios" name="comentarios" rows="4"></textarea>
      </fieldset>
  
      <button type="submit">Enviar</button>
    </form>
  </body>
</html>
```

