# salembo.github.io

Sitio personal de Ana Maria Ruiz: portafolio + blog, publicado con GitHub Pages y Jekyll (tema minima).

## Estructura

| Carpeta / archivo | Qué contiene |
|---|---|
| `index.md` | Página de inicio |
| `about.md` | Página "About me" |
| `projects.md` | Lista de proyectos (se genera sola a partir de `_projects/`) |
| `blog.md` | Lista de entradas (se genera sola a partir de `_posts/`) |
| `_projects/` | Un archivo `.md` por proyecto |
| `_posts/` | Un archivo `.md` por entrada del blog |
| `_templates/` | Plantillas para copiar (Jekyll no las publica) |
| `assets/images/` | Imágenes |
| `assets/main.scss` | Estilos propios encima del tema minima |

## Publicar una entrada nueva

1. Copia `_templates/post.md` a `_posts/AAAA-MM-DD-titulo-corto.md` (la fecha del nombre es la fecha de publicación).
2. Cambia el título, la descripción y las etiquetas, y escribe el texto en Markdown.
3. Haz commit y push a `main`. En uno o dos minutos aparece en `/blog/` y en el feed RSS (`/feed.xml`).

## Agregar un proyecto

1. Copia `_templates/project.md` a `_projects/nombre-corto.md`.
2. Completa `title`, `description`, `tech`, `repo` (y opcionalmente `demo` e `image`). `order` decide la posición: los números menores van primero, y los 3 primeros aparecen en la portada.
3. Commit y push. Queda publicado en `/projects/nombre-corto/`.

## Ver el sitio en tu computadora (opcional)

```bash
gem install bundler jekyll
bundle init && bundle add github-pages --group jekyll_plugins
bundle exec jekyll serve
```

Luego abre http://localhost:4000.
