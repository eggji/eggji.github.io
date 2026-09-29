# Jinlong Ji — personal homepage

Quiet personal page for **Jinlong Ji** ([@eggji](https://github.com/eggji)).
GitHub Pages: **`eggji/eggji.github.io`** → [eggji.github.io](https://eggji.github.io).

## Files

- `index.html` — about, interests, publications, blog teaser, links
- `styles.css` — light layout
- `blog/` — posts (`index.html` list, `_template.html`, individual HTML posts)
- `papers/` — One Paper a Day notes (`index.html` list with tag filter, `_template.html`, one HTML file per paper)

## Write a blog post

1. Copy `blog/_template.html` → `blog/your-slug.html`
2. Edit title, date, and body
3. Add a link in `blog/index.html` and in the Blog section of `index.html`
4. Commit and push to `main` (Pages serves from root)

## Add a paper note (One Paper a Day)

1. Copy `papers/_template.html` → `papers/<arxiv-id>.html` (e.g. `papers/2504.13837.html`)
2. Fill in title, authors, arXiv link, date read, tags, TL;DR, Conclusion summary, and My take
3. Add an entry at the **top** of the list in `papers/index.html`: copy an existing `<li>`, update the date,
   title/link, the tag chips, and `data-tags` (tags separated by `|`, same spelling as the chips; the filter matches on it)
4. Reuse existing tag names where possible (e.g. `RL`, `LLM reasoning`, `Post-training`, `Evaluation`,
   plus a type tag like `Empirical study`, `Method`, `Benchmark`)
5. Commit and push to `main`

## Preview

```bash
python3 -m http.server 8000
```

Open `http://localhost:8000`.
