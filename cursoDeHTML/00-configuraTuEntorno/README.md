![Copia de githubport](https://github.com/user-attachments/assets/c0bed80f-ea7e-4af3-bad7-99664e7efee9)

<h1 align="center">Como configurar tu entorno de trabajo</h1>

<p align="center"><em>En esta sección te voy a dejar el paso a paso para poder configurar tu entorno de desarrollo. Cuales son las herramientas que debes instalar y como configurarlas para poder trabajar de una manera optima tanto a lo largo de este curso como en cualquiera de los proyectos que quieras llevar a cabo en el futuro.</em></p>

<h3>Instala un navegador web:</h3>
<p>Cualquier navegador web te va a ser util para trabajar. Pero, mi recomendación es utilizar chrome. <br> Ingresa al sitio oficial de <a href="https://www.google.com/intl/es-419/chrome/dr/download/?brand=JJTC&gad_source=1&gclid=CjwKCAjwodC2BhAHEiwAE67hJO4VoiLaELcAmk7-YmwOcfvJzNhBvpVX4AhphuZGXcLa3EAwKUCA7xoCRW0QAvD_BwE&gclsrc=aw.ds">google chrome</a> y dale click en el boton de descarga.</p>

![WhatsApp Image 2024-09-01 at 22 03 50](https://github.com/user-attachments/assets/546e6950-b8c0-4ac5-a3b0-b03c02422533)
<p>Luego de que se complete la descarga del archivo ejecutable, segui los pasos de la siguiente pagina. Una vez que completes los pasos estas listo para empezar a utilizar el navegador. </p>

![Diseño sin título](https://github.com/user-attachments/assets/ef862f45-34ff-4306-a3cc-23aa4a1801b3)

<br>
<p align="center"><strong>TE RECOMIENDO ESTABLECER EL NAVEGADOR INSTALADO COMO PREDETERMINADO.</strong></p>
<hr>
<h3>Instala el editor Visual Studio Code:</h3>
<p>Ingresa al sitio oficial de <a href="https://code.visualstudio.com/download">Visual Studio Code</a>, selecciona tu sistema operativo y dale click en el boton de descarga.</p>

![WhatsApp Image 2024-09-01 at 22 46 06](https://github.com/user-attachments/assets/1b17d2de-5538-47c8-9c86-aa4f2be8ae9c)
<br>
<p>Luego de que se complete la descarga del archivo ejecutable, segui los pasos para completar su instalación.</p>
<hr>
<h3>Instala GIT - El sistema de control de versiones:</h3>
<p>Ingresa al sitio oficial de <a href="https://git-scm.com/">GIT</a>. Vas a ver una recomendación de descarga a tu derecha. Esto sucede porque git detecta desde que sistema operativo estas ingresando y te recomienda la descarga mas conveniente para dicho sistema. Dale click al boton de descarga y segui los pasos para completar la descarga.</p>

![Diseño sin título (2)](https://github.com/user-attachments/assets/4c6b73f0-7f27-4fc9-a650-7143a45352c6)
<br>
<p>Una vez que este instalado van a ver dos opciones d ejecutar git en su equipo. Deben ejecutar la opcion de git bash y se va a abrir una terminal con la que van a poder trabajar.</p>
<h3>Configuración de GIT:</h3>
<p>Paso 1: Una vez que la instalación de GIT haya terminado, abri la terminal de Git Bash, copia y ejecuta el siguiente comando:</p>

```bash
git --version
```

<p>Esto deberia mostrarte la versión de Git instalada</p>
<br>
<p>Paso 2: Configura GIT con tu información de usuario. Ejecuta el siguiente comando en la terminal de bash para configurar tu nombre de usuario y correo electrónico, que serán usados en tus commits:</p>

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tuemail@ejemplo.com"
```

<p>Verifica la configuración ejecutando:</p>

```bash
git config --global --list
```

<p>Esto debería mostrar el nombre y correo electrónico que configuraste.</p>

<p>Paso 3: Conectar GitHub usando SSH. En la terminal o Git Bash, ejecuta el siguiente comando para generar una nueva clave SSH:</p>

```bash
ssh-keygen -t ed25519 -C "tuemail@ejemplo.com"
```

<p>Si tu sistema no soporta ed25519, podes usar rsa:</p>

```bash
ssh-keygen -t rsa -b 4096 -C "tuemail@ejemplo.com"
```

<p>El sistema te va a pedir que elijas una ubicación para guardar la clave (puedes presionar Enter para aceptar la ubicación predeterminada) y que ingreses una frase de seguridad (esto ultimo es opcional).</p>
<br>
<p>Asegúrate de que el agente SSH esté en funcionamiento, luego agrega tu clave SSH generada:</p>

```bash
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519
```

<p>Si usaste rsa, el comando sería:</p>

```bash
ssh-add ~/.ssh/id_rsa
```
<br>
<p>Agregar la clave SSH a tu cuenta de GitHub. Copia la clave pública generada:</p>

```bash
cat ~/.ssh/id_ed25519.pub
```

<p>Si usaste rsa:</p>

```bash
cat ~/.ssh/id_rsa.pub
```

<p>Copia el contenido que se muestra en la terminal y inicia sesión en tu cuenta de GitHub. En la ezquina superior derecha dale click a tu foto de perfil y selecciona settings</p>

![Diseño sin título (4)](https://github.com/user-attachments/assets/b6af2d6e-3297-4251-b694-0b59f87bec34)

<p>En el menú de la izquierda, selecciona SSH and GPG keys y luego New SSH key. Pega tu clave pública en el campo Key y dale un título. Por ultimo dale click a Add SSH key</p>

![Diseño sin título (5)](https://github.com/user-attachments/assets/1e10dc22-9709-473c-b242-7e356357152b)

<p>Para verifica que todo este funcionando correctamente ejecuta:</p>

```bash
ssh -T git@github.com
```

<p>Si todo está bien, deberías ver un mensaje de bienvenida desde GitHub.</p>

<h5>Listo!! Ahora has conectado exitosamente GitHub con la terminal de Git en tu equipo, y vas a poder trabajar con tus repositorios remotos directamente desde la línea de comandos.</h5>

<h3>Por ultimo, pero igualmente importante. Instala Node.js:</h3>
<p>Ingresa al sitio oficial de <a href="https://nodejs.org/en">Node.js</a>, dale click en el boton de descarga y segui los pasos para completar la descarga.</p>

![Diseño sin título (6)](https://github.com/user-attachments/assets/1d1d099a-2f1d-4a83-abb6-28dfcd4b8267)
