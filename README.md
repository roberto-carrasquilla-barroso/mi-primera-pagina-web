# Trabajo individual: Mi primera página web

## Descripción del trabajo

Este proyecto consiste en el desarrollo de un sitio web personal estático utilizando únicamente HTML y CSS. El objetivo principal es aplicar los conocimientos aprendidos en la asignatura **Fundamentos de la Ingeniería Informática** para diseñar una página web que muestre información sobre mi grado, mis intereses y mi progreso académico.

La estructura del sitio sigue el mapa de navegación indicado en el enunciado:

- `index.html`: página principal con una presentación general del sitio.
- `about.html`: sección "Acerca de mí" con información personal y académica.
- `contact.html`: página de contacto con un formulario sencillo (sin lógica de envío).
- `net.html`: sección de red con enlaces a las páginas web de compañeros.
- `topic.html`: sección temática dedicada a un tema de interés personal.
- `degree.html`: sección sobre el grado en Ingeniería Informática y sus asignaturas.

Todos los estilos del sitio se encuentran en una hoja de estilos externa común almacenada en la carpeta `css` y enlazada desde cada página HTML.

La organización del repositorio utiliza la carpeta `docs` como raíz del sitio público, siguiendo el esquema propuesto en las indicaciones:

- `docs/css/styles.css`: hoja de estilos global.
- `docs/public/*.html`: todas las páginas HTML del sitio.
- `docs/images/`: carpeta única para todas las imágenes utilizadas.
- `README.md`: este documento, con la descripción y la reflexión sobre el proyecto.

El sitio web se publica mediante GitHub Pages configurando la carpeta `docs` como origen de la página.

## Problemas durante el desarrollo

Durante la realización del trabajo han aparecido varios problemas técnicos:

1. **Configuración de GitHub Pages**  
   Al principio, la página se publicaba correctamente, pero los cambios en los archivos no se actualizaban en la versión online. Esto se debía a que la configuración de GitHub Pages no utilizaba la carpeta correcta como origen del sitio. Tras revisar la configuración y seleccionar la rama `main` y la carpeta `/docs`, el despliegue comenzó a funcionar correctamente.

2. **Ruta de la hoja de estilos CSS**  
   El mayor problema fue que los estilos no se aplicaban en GitHub Pages. Localmente la web se veía bien, pero en la versión publicada se mostraba sin formato. El motivo era que la ruta al archivo CSS no coincidía con la estructura de carpetas utilizada. Se corrigió ajustando el enlace a:
