# votanessuno.github.io

Sito web di **Vota Nessuno** — il partito della maggioranza silenziosa.

## Setup locale

```bash
gem install bundler
bundle install
bundle exec jekyll serve
```

Il sito sarà disponibile su `http://localhost:4000`.

## Struttura

```
├── _config.yml         # Configurazione Jekyll
├── _layouts/           # Template HTML
│   ├── default.html    # Guscio base
│   ├── home.html       # Homepage con sidebar
│   └── page.html       # Subpage
├── _includes/          # Componenti riutilizzabili
│   ├── header.html     # Topbar, header, marquee, nav
│   └── footer.html     # Footer
├── _posts/             # Blog posts (YYYY-MM-DD-titolo.md)
├── assets/
│   ├── css/style.css   # Stili
│   └── images/         # Logo e immagini
├── index.html          # Homepage
├── manifesto.md        # Pagina manifesto
└── 404.md              # Pagina 404
```

## Scrivere un blog post

Crea un file in `_posts/` con il formato `YYYY-MM-DD-titolo-del-post.md`:

```yaml
---
layout: page
title: "Titolo del post"
date: 2026-02-28
---

Testo del post qui in Markdown...
```

## Deploy

Push su `main` → GitHub Pages builda e deploya automaticamente.
