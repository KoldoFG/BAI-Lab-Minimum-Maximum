# Visor BAI · Espacios mínimos y máximos

Herramienta web del LAB del Programa BAI (Pamplona) para proponer, comparar y combinar espacios mínimos y máximos.
Dirección: Deplazes, Mangado · Profesorado: Fdez. Gaztelu, Oiza, Olite, Tabuenca, Vélaz.

Es una sola página (`index.html`), sin servidor ni base de datos. Funciona en castellano y en inglés (selector ES | EN).

## Archivos

| Archivo | Para qué sirve |
|---|---|
| `index.html` | La aplicación completa. |
| `icon.svg`, `icon-192.png`, `icon-512.png` | Icono de la app **BAI Lab** (logo BAI con «LAB» debajo, blanco sobre negro). |
| `apple-touch-icon.png` | Icono al añadirla a la pantalla de inicio en iPhone o iPad. |
| `favicon.svg`, `favicon-32.png` | Icono de la pestaña del navegador (solo «BAI», para que se lea a tamaño pequeño). |
| `site.webmanifest` | Nombre e iconos de la app para instalarla en el móvil o el ordenador. |
| `README.md` | Estas instrucciones. |
| `.nojekyll` | Archivo vacío: indica a GitHub que sirva la página tal cual. |

## Publicarla con GitHub Pages

1. En GitHub, crea un repositorio nuevo, por ejemplo `bai-visor`. Puede ser público o privado; con una cuenta gratuita, Pages solo funciona en repositorios públicos.
2. Sube todos los archivos de esta carpeta, en la raíz del repositorio (sin subcarpetas). Desde la web: **Add file → Upload files**, arrástralos y pulsa **Commit changes**. El archivo `.nojekyll` empieza por punto y algunos sistemas lo ocultan; si no lo ves, no pasa nada, la página funciona igual.
3. Ve a **Settings → Pages**. En **Build and deployment**, elige **Source: Deploy from a branch**, rama **main** y carpeta **/ (root)**. Pulsa **Save**.
4. En uno o dos minutos la página estará en `https://TU-USUARIO.github.io/bai-visor/`. Ese es el enlace que se pasa a los alumnos.

Para actualizar el visor más adelante, basta con subir de nuevo `index.html` (sustituye al anterior). Los datos de los alumnos no se pierden, porque viven en su navegador, no en el repositorio.

## Instalarla como app

Con el icono y el manifiesto, BAI Lab se puede instalar como una app:

- **Ordenador (Chrome o Edge):** abre el enlace y pulsa el icono de instalar en la barra de direcciones.
- **iPhone o iPad (Safari):** Compartir → **Añadir a pantalla de inicio**.
- **Android (Chrome):** menú ⋮ → **Instalar app** o **Añadir a pantalla de inicio**.

La app instalada usa los mismos datos que la página en ese navegador.

## Cómo se trabaja

**Alumnos**

- Escriben su nombre en «Alumno» y eligen grupo.
- Trabajan cada estancia en 01 Mínimos y 02 Máximos, la comparan en 03 Comparar y la combinan en 05 Ud. Hab.
- Para entregar, abren la estancia y pulsan **Exportar estancia**: se descarga un archivo `BAI_Nombre-Apellido_01_Cocina.json` que envían al profesor.
- Todo se guarda solo en su navegador. Si cambian de ordenador o de navegador, escriben allí su nombre e importan sus archivos con **Importar estancia**.

**Profesorado**

- **Importar estancia** admite varios archivos a la vez (o se pueden soltar sobre el visor). Cada alumno queda en su carpeta, abajo en la columna izquierda.
- Con ‹ › junto al nombre se pasa de un alumno a otro sin cambiar de estancia ni de pestaña.
- 04 Matriz muestra estancias × alumnos (mínimos, máximos y comparativa), cada fila a la misma escala.
- En 05 Ud. Hab. se pueden combinar estancias de alumnos distintos y barajar autores.
- En 04 Matriz, **Exportar todo** guarda en un solo archivo tu trabajo y todas las carpetas de alumnos, con sus unidades habitacionales. Sirve como copia de seguridad y para pasar el conjunto a otro profesor, que lo carga con **Importar estancia**: las carpetas se añaden a las suyas.

## Notas

- Las descargas usan la descarga normal del navegador.
- Las tipografías (Schibsted Grotesk e IBM Plex Mono) se cargan de Google Fonts; sin conexión, el visor usa las del sistema.
