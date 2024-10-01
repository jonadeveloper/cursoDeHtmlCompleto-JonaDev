![4](https://github.com/user-attachments/assets/c3ce67c9-e43a-4e4d-bc31-669258367b8d)

<h1 align="center">Introducción a la semantica HTML</h1>

<p>En este punto, ya vimos cuales son las etiquetas basicas de HTML y un poco más. A partir de ahora vamos a ver las etiquetas semanticas. Lo que va a mejorar la accesibilidad, SEO, y la estructura del documento.</p>

<h3>¿Qué es HTML Semántico?</h3>
<p>Es la manera en la que se deben utilizar las etiquetas para dar un significado claro al contenido para que los navegadores y motores de búsqueda lo comprendan mejor. Vale aclarar que no todas las etiquetas tienen un significado semantico. Esto es clave para decidir que etiquetas utilizar segun su contenido y proposito. <br> <i>* La semantica mejora la experiencia del usuario y facilita el mantenimiento del código.</i></p>

<h3>Etiquetas semanticas principales</h3>
<ol>
  <li>
    <h3>header</h3>
    <p>Significado semantico: Representa el encabezado de una página o una sección del documento. Puede contener elementos como un logotipo, menú de navegación, o título.</p>
    <p>Cuándo usarla: Cuando necesitas definir el encabezado de una página o una sección dentro de un artículo o sección.</p>
    
```html

    <header>
      <h1>Mi Blog</h1>
      <nav>Menú de Navegación</nav>
    </header>

````

  </li>
  <li><h3>nav</h3>
    <p>Significado semantico: Define un bloque de navegación, generalmente usado para agrupar enlaces que permiten al usuario moverse dentro del sitio o a sitios relacionados.</p>
    <p>Cuándo usarla: Para agrupar enlaces de navegación importantes.</p>

```html

    <nav>
      <a href="#inicio">Inicio</a>
      <a href="#contacto">Contacto</a>
    </nav>

````

  </li>
  <li><h3>main</h3> 
    <p>Significado semantico: Define el contenido principal de la página. Solo debe haber un main por documento.</p>
    <p>Cuándo usarla: Para el contenido principal que es único en la página, excluyendo encabezados, pies de página, y navegación.</p>
    
```html

    <main>
      <article>Contenido principal de la página</article>
    </main>

````
  </li>
  <li><h3>section</h3>
    <p>Significado semantico: Representa una sección temática dentro de un documento. Se utiliza para dividir contenido en bloques con significado específico.</p>
    <p>Cuándo usarla: Cuando tienes varias secciones de contenido que están relacionadas entre sí, pero son independientes en cierta medida.</p>

```html

    <section>
      <h2>Sección de Noticias</h2>
      <p>Últimas noticias del día...</p>
    </section>

````

  </li>
  <li><h3>article</h3> 
    <p>Significado semantico: Define un contenido independiente, como una publicación de blog, un artículo de revista o un comentario.</p>
    <p>Cuándo usarla: Para contenido que tiene sentido por sí mismo, como una entrada de blog o un artículo de noticias.</p>
    
```html

    <article>
      <h2>Título del artículo</h2>
      <p>Contenido del artículo.</p>
    </article>

````
  </li>
  <li><h3>aside</h3>
    <p>Significado semantico: Representa contenido relacionado o adicional que está tangencialmente relacionado con el contenido principal, como una barra lateral o un bloque de anuncios.</p>
    <p>Cuándo usarla: Para contenido complementario, como enlaces a artículos relacionados o contenido auxiliar como anuncios.</p>

```html

    <aside>
      <h2>Artículos Relacionados</h2>
      <ul>
        <li>Artículo 1</li>
        <li>Artículo 2</li>
      </ul>
    </aside>


````

  </li>
  <li><h3>footer</h3> 
    <p>Significado semantico: Define el pie de página de un documento o sección, donde generalmente se incluye información de contacto, derechos de autor o enlaces legales.</p>
    <p>Cuándo usarla: Para agrupar información que aparece al final de una página o sección, como créditos o enlaces adicionales.</p>
    
```html

    <footer>
      <p>© 2024 Mi Empresa</p>
      <nav>Política de privacidad | Términos de servicio</nav>
    </footer>

````
  </li>
  <li><h3>figure y figcaption</h3>
    <p>Significado semantico: figure se usa para agrupar contenido gráfico, como imágenes o diagramas, y figcaption proporciona una leyenda o descripción.</p>
    <p>Cuándo usarla: Cuando necesitas incluir una imagen o gráfico con una descripción clara.</p>

```html

    <figure>
      <img src="imagen.jpg" alt="Descripción de la imagen">
      <figcaption>Figura 1: Descripción de la imagen.</figcaption>
    </figure>

````

  </li>
</ol>

<h3>Etiquetas NO semanticas que se suelen usar de manera erronea.</h3>

<ol>
  <li>
    <h3>div</h3>
    <p>Uso incorrecto: Se utiliza para agrupar elementos sin necesidad de establecer relaciones semánticas entre ellos. Se abusa de esta etiqueta para crear casi toda la estructura de una página.</p>
    <p>Alternativa: Usar etiquetas semánticas como section, article, header, footer, y main que describen claramente el propósito del contenido.</p>    
  </li>
  <li>
    <h3>span</h3>
    <p>Uso incorrecto: Se usa de manera excesiva para aplicar estilos o agrupar texto cuando no es necesario. Se abusa de span en lugar de otras etiquetas más adecuadas como strong para texto en negrita o em para texto enfatizado.</p>
    <p>Alternativa: Utilizar etiquetas semánticas como strong, em, o mark cuando sea apropiado.</p>    
  </li>
  <li>
    <h3>b</h3>
    <p>Uso incorrecto: Se usa para hacer texto en negrita sin ninguna semántica, es decir, sin decirle al navegador o a los lectores de pantalla que ese texto tiene importancia o relevancia.</p>
    <p>Alternativa: Usar strong si el texto tiene importancia o relevancia en el contexto.</p>    
  </li>
  <li>
    <h3>i</h3>
    <p>Uso incorrecto: Similar al caso de b, se utiliza para mostrar texto en cursiva, pero sin ninguna semántica adicional.</p>
    <p>Alternativa: Usar em si el texto debe ser enfatizado o leído con un tono diferente.</p>    
  </li>
  <li>
    <h3>font (Obsoleta en HTML5)</h3>
    <p>Uso incorrecto: Se usaba para cambiar el color, tamaño o tipo de fuente. Aún se ve en código legado, aunque está obsoleta.</p>
    <p>Alternativa: Usar CSS para manejar estilos de fuentes con propiedades como font-family, font-size, y color.</p>    
  </li>
  <li>
    <h3>center (Obsoleta en HTML5)</h3>
    <p>Uso incorrecto: Se utilizaba para centrar texto o elementos visuales.</p>
    <p>Alternativa: Usar CSS con la propiedad text-align: center para centrar texto o margin: auto para centrar bloques.</p>    
  </li>
  <li>
    <h3>u</h3>
    <p>Uso incorrecto: Se utiliza para subrayar texto, pero sin darle un significado especial.</p>
    <p>Alternativa: Usar ins (para indicar inserciones de texto en documentos) o aplicar subrayado con CSS si es solo una cuestión de estilo.</p>    
  </li>
  <li>
    <h3>br</h3>
    <p>Uso incorrecto: Se usa para forzar saltos de línea en lugar de organizar el contenido correctamente con márgenes, párrafos o bloques.</p>
    <p>Alternativa: Usar p para crear párrafos, o controlar el espaciado entre elementos mediante CSS (margin, padding).</p>    
  </li>
  <li>
    <h3>table (para diseño)</h3>
    <p>Uso incorrecto: Se usa para maquetar la página o crear grids en lugar de usar CSS. Este era un enfoque común antes de CSS Grid o Flexbox.</p>
    <p>Alternativa: Utilizar CSS Grid o Flexbox para el diseño de la página. Las tablas solo deben ser usadas para datos tabulares.</p>  
  </li>
  <li>
    <h3>iframe (para layout)</h3>
    <p>Uso incorrecto: Se utiliza a veces para insertar secciones de páginas externas o para organizar partes de una página dentro de otra, lo que genera problemas de accesibilidad y SEO.</p>
    <p>Alternativa:Evitar su uso para layouts y preferir incluir contenido con APIs o servicios web cuando sea necesario insertar datos externos.</p>  
  </li>
</ol>
 <i>* ¿Cuándo Usar Etiquetas Semánticas?
Usar Etiquetas Semánticas: Siempre que quieras proporcionar un contexto claro sobre el propósito de una sección o contenido en particular.</i>
<br><br>
<i>* ¿Cuándo Usar Etiquetas No Semánticas?</i>
Usar Etiquetas No Semánticas: Cuando simplemente necesitas agrupar elementos sin agregar contexto, o cuando necesitas aplicar estilos.</i>
<br><br>

![Copia de githubport](https://github.com/user-attachments/assets/ac72290a-818e-40c7-aff5-311f989e5de3)

<h1 align="center">Diferencias entre ID y class</h1>

<p>Aunque en este curso no nos vamos a centrar tanto en los estilos, entender que hay una diferencia muy marcada entre ID y class es muy importante para aplicar buenas practicas en la estructuración de un documento HTML.</p>

<h3>ID:</h3>
<p>Es un identificador único para un solo elemento en el DOM. No puede repetirse en la misma página.</p>
<p><b>Uso:</b> Ideal para elementos que necesitas identificar individualmente, como el encabezado principal o una sección específica.</p>

```html
  <div id="menu">Menú Principal</div>
```

<h3>class:</h3>
<p>Se puede aplicar a múltiples elementos. Es útil para agrupar elementos que comparten estilos o comportamientos.</p>
<p><b>Uso:</b> Utilizado cuando varios elementos necesitan el mismo estilo o comportamiento.</p>

```html
  <div class="boton">Botón 1</div>
  <div class="boton">Botón 2</div>
```

<i>* Diferencias Clave: id es único en toda la página, mientras que class puede reutilizarse.
En CSS, #id selecciona un único elemento, mientras que .class puede seleccionar varios.</i>
<br><br>

![Copia de githubport (1)](https://github.com/user-attachments/assets/7a718cb1-9020-44c1-8b44-853f23b1c482)

<h1 align="center">Formularios avanzados.</h1>

<p>Los formularios son una de las interacciones más comunes en la web. En este punto, vamos a ver cómo crear formularios más completos y accesibles.</p>

<h3>Etiquetas y Atributos Avanzados para formularios.</h3>

<ol>
  <li>
    <h3>input (tipos avanzados)</h3>
    <p>Introducción a tipos avanzados de input</p>
    <ul>
      <li>type="email": Valida automáticamente que el usuario ingrese un formato de email válido.</li>
      <li>type="password": proporcionan una forma para que el usuario ingrese una contraseña de forma segura.</li>
      <li>type="url": Asegura que la entrada sea una URL.</li>
      <li>type="number": Solo permite ingresar números y puede tener atributos como min, max y step para especificar rangos y valores aceptables.</li>
      <li>type="date" y type="datetime-local": Permiten seleccionar fechas y tiempos con un selector gráfico.</li>
      <li>type="range": Crea un control de rango deslizante, ideal para selecciones numéricas rápidas.</li>
    </ul>
    <br><br>
    
```html

    <label for="email">Correo Electrónico:</label>
    <input type="email" id="email" name="email" required>
    
    <label for="date">Fecha de nacimiento:</label>
    <input type="date" id="date" name="date">
    
    <label for="range">Elija un valor:</label>
    <input type="range" id="range" name="range" min="0" max="100">

    <label for="range">Ingrese una contraseña:</label>
    <input type="password">

    <input type="submit" value="Enviar">

```
    
  </li>
  <li>
    <h3>span</h3>
    <p>Uso incorrecto: Se usa de manera excesiva para aplicar estilos o agrupar texto cuando no es necesario. Se abusa de span en lugar de otras etiquetas más adecuadas como strong para texto en negrita o em para texto enfatizado.</p>
    <p>Alternativa: Utilizar etiquetas semánticas como strong, em, o mark cuando sea apropiado.</p>    
  </li>
  <li>
    <h3>b</h3>
    <p>Uso incorrecto: Se usa para hacer texto en negrita sin ninguna semántica, es decir, sin decirle al navegador o a los lectores de pantalla que ese texto tiene importancia o relevancia.</p>
    <p>Alternativa: Usar strong si el texto tiene importancia o relevancia en el contexto.</p>    
  </li>
  <li>
    <h3>i</h3>
    <p>Uso incorrecto: Similar al caso de b, se utiliza para mostrar texto en cursiva, pero sin ninguna semántica adicional.</p>
    <p>Alternativa: Usar em si el texto debe ser enfatizado o leído con un tono diferente.</p>    
  </li>
  <li>
    <h3>font (Obsoleta en HTML5)</h3>
    <p>Uso incorrecto: Se usaba para cambiar el color, tamaño o tipo de fuente. Aún se ve en código legado, aunque está obsoleta.</p>
    <p>Alternativa: Usar CSS para manejar estilos de fuentes con propiedades como font-family, font-size, y color.</p>    
  </li>
  <li>
    <h3>center (Obsoleta en HTML5)</h3>
    <p>Uso incorrecto: Se utilizaba para centrar texto o elementos visuales.</p>
    <p>Alternativa: Usar CSS con la propiedad text-align: center para centrar texto o margin: auto para centrar bloques.</p>    
  </li>
  <li>
    <h3>u</h3>
    <p>Uso incorrecto: Se utiliza para subrayar texto, pero sin darle un significado especial.</p>
    <p>Alternativa: Usar ins (para indicar inserciones de texto en documentos) o aplicar subrayado con CSS si es solo una cuestión de estilo.</p>    
  </li>
  <li>
    <h3>br</h3>
    <p>Uso incorrecto: Se usa para forzar saltos de línea en lugar de organizar el contenido correctamente con márgenes, párrafos o bloques.</p>
    <p>Alternativa: Usar p para crear párrafos, o controlar el espaciado entre elementos mediante CSS (margin, padding).</p>    
  </li>
  <li>
    <h3>table (para diseño)</h3>
    <p>Uso incorrecto: Se usa para maquetar la página o crear grids en lugar de usar CSS. Este era un enfoque común antes de CSS Grid o Flexbox.</p>
    <p>Alternativa: Utilizar CSS Grid o Flexbox para el diseño de la página. Las tablas solo deben ser usadas para datos tabulares.</p>  
  </li>
  <li>
    <h3>iframe (para layout)</h3>
    <p>Uso incorrecto: Se utiliza a veces para insertar secciones de páginas externas o para organizar partes de una página dentro de otra, lo que genera problemas de accesibilidad y SEO.</p>
    <p>Alternativa:Evitar su uso para layouts y preferir incluir contenido con APIs o servicios web cuando sea necesario insertar datos externos.</p>  
  </li>
</ol>
