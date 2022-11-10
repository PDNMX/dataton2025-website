# Sitio web del Dataton Anticorrupción

Este repositorio tiene el código con el que se genera el sitio web del Datatón Anticorrupción 2021.

Para generar el sitio se utiliza el generador [Hugo](https://gohugo.io).

El sitio actualmente se encuentra hospedado en Netlify y se actualiza automáticamente cada que hay un cambio en la rama principal ("main") de este repositorio.

### Instrucciones para modificar el sitio

Para hacer cambios al sitio, recomendamos modificar los archivos y usar Hugo para "compilar" los archivos estáticos.

1. Instalar Hugo (https://gohugo.io).
2. Clonar este repositorio.
3. Modificar los archivos correspondientes:
    - `/config.toml` para cambiar información general y habilitar secciones.
    - La información de mentores y jueces se genera a partir de los archivos markdown bajo `/content/`
    - El css está en `/themes/dataton-agency/static/css/styles.css`
    - Las imágenes se ponen en `/static/img`
4. Probar el sitio localmente con el comando `hugo server` desde el directorio raíz. Esto muestra el sitio en http://localhost:1313
5. Enviar los cambios al repositorio en GitHub (`git add .` -> `git commit -m "..."` -> `git push origin main`).
6. Al enviar cambios (push), automáticamente se ejecutará una tarea que genere una nueva versión y actualice el sitio desplegado en Netlify.
