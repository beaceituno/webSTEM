<!-- badges: start -->

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE) [![Netlify Status](https://api.netlify.com/api/v1/badges/fc0143c8-b8b5-4807-83c5-b327e267594e/deploy-status)](https://app.netlify.com/sites/clubstemmairena/deploys)

<!-- badges: end -->

# webSTEM · Club STEM Mairena

Web del Club STEM del IES Juan de Mairena (San Sebastián de los Reyes, Madrid), con las actividades de ciencia, tecnología, ingeniería y matemáticas que realizamos en los recreos.

🌐 **Web:** <https://clubstemmairena.netlify.app>

## Estructura

| Ruta | Contenido |
|------|-----------|
| `index.qmd` | Página de inicio |
| `about.qmd` | Información sobre el club |
| `blog_curso_actual/` | Actividades del curso actual (una carpeta por actividad: `DDMMAAAA_nombre/index.qmd` + `images/`) |
| `blog_histórico/` | Actividades de cursos anteriores |
| `docs/` | Documentos PDF (plan de centro, concurso de logotipo...) |
| `images/` | Imágenes comunes (logo, favicon...) |
| `styles.css` | Estilos propios sobre el tema `sketchy` |

## Añadir una actividad

1. Copia una carpeta existente de `blog_curso_actual/` y renómbrala como `DDMMAAAA_nombre`.
2. Edita `index.qmd`: título, descripción, fecha, imagen de portada y categorías (curso, tipo, área).
3. Guarda las imágenes en la carpeta `images/` de la actividad y añade siempre texto alternativo (`fig-alt`).

## Generar la web en local

Requiere [Quarto](https://quarto.org/docs/get-started/).

```bash
quarto preview   # vista previa con recarga automática
quarto render    # genera la web en _site/
```

## Publicación

La web se publica automáticamente en Netlify al subir cambios a `main`, mediante el plugin [`@quarto/netlify-plugin-quarto`](https://github.com/quarto-dev/netlify-plugin-quarto).
También puede publicarse manualmente con `quarto publish netlify`.

## Licencia

[MIT](LICENSE) © Beatriz Aceituno Moreno
