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
    <br>
    <p>Cuándo usarla: Cuando necesitas definir el encabezado de una página o una sección dentro de un artículo o sección.</p>
    
```html

    <header>
      <h1>Mi Blog</h1>
      <nav>Menú de Navegación</nav>
    </header>

```

  </li>
  <li><b>nav</b>: Contiene la barra de navegación.</li>
  <li><b>article</b>: Contiene contenido independiente, como una publicación de blog o artículo.</li>
  <li><b>section</b>: Agrupa contenido temáticamente relacionado.</li>
  <li><b>aside</b>: Define contenido complementario o relacionado al contenido principal, como una barra lateral.</li>
  <li><b>main</b>: Define el contenido principal de la página, excluyendo encabezados, pies de página, etc.</li>
  <li><b>figure y figurecaption</b>: Para agregar imágenes con subtítulos.</li>
  <li>
    <h3>footer:</h3> <p>Contiene el pie de página, como información de contacto o enlaces legales.</p>

```html

    <footer>
      <p>© 2024 Mi Empresa</p>
      <nav>Política de privacidad | Términos de servicio</nav>
    </footer>

```

  </li>
</ol>
