# Wildlife Genomics Lab @ Smith College — website

Source for <https://tanyalama.github.io>, built by GitHub Pages (Jekyll, no remote theme).

## Updating content (no HTML needed)

| To change…            | Edit                        |
|-----------------------|-----------------------------|
| News items            | `_data/news.yml`            |
| Publications          | `_data/publications.yml` (+ `in_prep.yml`, `other_pubs.yml`) |
| Lab members / alumni  | `_data/people.yml` (photos in `assets/img/people/`, ~500 px square JPG) |
| Page text             | `research.md`, `teaching.md`, `outreach.md`, `join.md`, `cv.md` |
| Nav, links, email     | `_config.yml`               |
| Colors / fonts        | `assets/css/main.css` (`:root` variables) |

Drop a public CV at `assets/cv/Lama_CV.pdf` and a download button appears on `/cv/` automatically.

## Preview locally

```
bundle install
bundle exec jekyll serve
```

Old `/pages/*.html` URLs redirect to the new pages.
