# jgalandb.github.io

Portfolio - Jorge Galán del Blanco

Mi currículum en formato web. Lo hice para tener algo más completo que un PDF y para practicar HTML, CSS y JavaScript mientras estudio. Demo: https://jgalandb.github.io/

Vengo del marketing y la analítica digital y estoy cambiando hacia la ingeniería de datos. Por eso la web simula la consola de un data lake: cada sección es una carpeta (s3://jgb-datalake/...), la experiencia aparece como ejecuciones de un job y las habilidades como un pipeline de datos.

Qué hace
Secciones: inicio, sobre mí, pipeline de skills, formación, experiencia y contacto.
Se puede cambiar entre español e inglés.
Tiene modo claro y oscuro. Por defecto usa el del sistema.
Se adapta a ordenador, tablet y móvil.
Botones para descargar el CV en los dos idiomas, escribirme un correo y abrir mi LinkedIn.
Fondo animado dibujado con canvas.
Cómo está hecho

Solo HTML, CSS y JavaScript, sin frameworks ni librerías. Lo único externo son las fuentes de Google Fonts.

Idioma: los textos llevan un atributo data-k. En js/script.js hay un diccionario con las traducciones y, al cambiar de idioma, se recorren esos elementos y se cambia el texto.
Tema: los colores son variables CSS. El tema claro se activa con prefers-color-scheme o con el botón de la barra superior.
Navegación: cada sección tiene un id y solo se muestra la activa según el hash de la URL (#about, #skills...). Así cada apartado tiene su propio enlace y no hay recargas.
Responsive: por encima de 1025 px la web se muestra dentro de un monitor. A partir de 900 px el menú lateral pasa a ser desplegable y a partir de 640 px todo va en una sola columna.
Estructura
index.html
css/styles.css
js/script.js
img/photo.jpg
og-image.png
CV_JorgeGalanDelBlanco_ES.pdf
CV_JorgeGalanDelBlanco_EN.pdf
Probarlo en local

No hay nada que instalar. Se puede abrir index.html directamente en el navegador, o levantar un servidor sencillo:

git clone https://github.com/jgalandb/jgalandb.github.io.git
cd jgalandb.github.io
python -m http.server 8000

y entrar en http://localhost:8000.

Publicación

Está desplegado con GitHub Pages desde la rama main. Cada push se actualiza solo en uno o dos minutos.

Cosas que quiero mejorar
Añadir una sección de proyectos cuando tenga más subidos a GitHub, incluido mi proyecto final de grado (KOIN, una web de gestión financiera personal y de empresa).
Mejorar la accesibilidad, sobre todo la navegación con teclado.
Separar el diccionario de traducciones en su propio archivo.
Contacto

jgalandb@gmail.com LinkedIn: https://linkedin.com/in/jorgegalandelblanco/
