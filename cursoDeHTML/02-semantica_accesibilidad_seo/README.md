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
  
</ol>

| Etiqueta     | Semántica/No Semántica | Descripción                                                                 | Jerarquía                                        | Uso                                             |
| ------------ | ---------------------- | --------------------------------------------------------------------------- | ------------------------------------------------ | ----------------------------------------------- |
| `h1` - `h6`  | Semántica              | Encabezados de diferentes niveles, de `h1` (más importante) a `h6` (menos). | Tienen jerarquía, siendo `h1` el más importante. | Para títulos y subtítulos en una página.        |
| `p`          | Semántica              | Define un párrafo.                                                          | No tiene jerarquía.                              | Para agrupar y estructurar bloques de texto.    |
| `a`          | Semántica              | Define un hipervínculo para navegar entre páginas.                          | No tiene jerarquía.                              | Para crear enlaces a otras páginas o recursos.  |
| `strong`     | Semántica              | Texto importante, aparece en negrita y tiene semántica de énfasis.          | No tiene jerarquía, pero marca importancia.      | Para destacar texto importante.                 |
| `em`         | Semántica              | Texto enfatizado, aparece en cursiva con énfasis semántico.                 | No tiene jerarquía.                              | Para enfatizar o destacar texto.                |
| `blockquote` | Semántica              | Define una cita en bloque de otro autor.                                    | No tiene jerarquía formal.                       | Para insertar citas o referencias textuales.    |
| `code`       | Semántica              | Muestra fragmentos de código en texto monoespaciado.                        | No tiene jerarquía.                              | Para mostrar código o comandos.                 |
| `pre`        | Semántica              | Texto preformateado, respeta espacios y saltos de línea.                    | No tiene jerarquía.                              | Para texto o código con formato exacto.         |
| `mark`       | Semántica              | Resalta el texto, útil para llamar la atención.                             | No tiene jerarquía.                              | Para resaltar texto.                            |
| `b`          | No semántica           | Texto en negrita sin implicaciones semánticas.                              | Solo visual.                                     | Para texto visualmente importante.              |
| `i`          | No semántica           | Texto en cursiva sin implicaciones semánticas.                              | Solo visual.                                     | Para estilizar texto, como nombres o títulos.   |
| `ul`         | Semántica              | Lista desordenada.                                                          | No tiene jerarquía.                              | Para listas de elementos sin orden.             |
| `ol`         | Semántica              | Lista ordenada.                                                             | No tiene jerarquía.                              | Para listas de elementos con un orden numérico. |
| `table`      | Semántica              | Contenedor de datos tabulares.                                              | Tiene jerarquía interna (thead, tbody, etc.).    | Para mostrar datos en una tabla estructurada.   |
