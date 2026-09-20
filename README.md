# webpersonal

Web personal de Alberto Torrejón Valenzuela: <https://albtorval.github.io/webpersonal/>

Sitio hecho con **blogdown + Hugo** (tema `hugo-classic`, modificado en `themes/`).

## Estructura

- `content/_index.Rmd` — portada (única fuente; no crear `content/index.Rmd`).
- `content/post/`, `content/text/` — artículos y textos (`.Rmd`; el `.html` de al lado lo genera blogdown y hay que subirlo).
- `static/` — CSS (`static/css/theme-override.css`), imágenes y PDFs.
- `docs/` — salida generada (`publishDir`) que sirve GitHub Pages. No editar a mano.

## Flujo de trabajo

1. Editar en RStudio.
2. `blogdown::build_site()` para regenerar `content/*.html` y `docs/`.
3. Commit y push.
