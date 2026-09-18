# Jinlong Ji — ML Engineer portfolio

Static personal site for **Jinlong Ji** ([GitHub @eggji](https://github.com/eggji)), Machine Learning Engineer at xAI (San Mateo, CA).

Intended for upload to the user site repo **`eggji/eggji.github.io`** so it serves at **https://eggji.github.io**.

## Files

| File | Purpose |
|------|---------|
| `index.html` | Single-page portfolio (hero, experience, projects, skills, publications, contact) |
| `styles.css` | Layout and theme (mobile-friendly) |
| `script.js` | Mobile nav + year + section highlight |
| `README.md` | This file |

All asset paths are **relative** (`styles.css`, `script.js`) so the site works from the GitHub Pages **user site root**.

## Edit content

1. Open `index.html`.
2. Replace bracketed placeholders such as `[Start date]`, `[Prior company]`, outcome bullets, email, and LinkedIn.
3. **Projects** are labeled **SAMPLE** on purpose — swap in real shipped work and remove the `SAMPLE` badge (`<span class="badge badge-sample">SAMPLE</span>`) when ready.
4. Trim or expand the **Skills** tag lists to match what you actually own.
5. **Publications** is optional; delete the whole `#publications` section (and its nav link) if you want an eng-only page.
6. Tweak colors/spacing in `styles.css` if desired (`:root` CSS variables).

Do not commit secrets, tokens, or private emails you do not want public.

## Preview locally

From this folder:

```bash
# Python
python3 -m http.server 8000

# or Node
npx --yes serve .
```

Then open `http://localhost:8000`.

Or simply open `index.html` in a browser (fine for a static page).

## Enable GitHub Pages (user site → https://eggji.github.io)

1. Create (or use) the repository **`eggji/eggji.github.io`** on GitHub.  
   The repo name must match `{username}.github.io` for a user site.
2. Push these files to the **`main`** branch at the **repository root** (not a `/docs` subfolder):
   - `index.html`
   - `styles.css`
   - `script.js`
   - `README.md` (optional on the live site)
3. In the repo: **Settings → Pages**.
4. Under **Build and deployment**:
   - **Source**: Deploy from a branch
   - **Branch**: `main` / `/ (root)`
5. Save. After a minute or two, the site is live at **https://eggji.github.io**.

Custom domain (optional): add a `CNAME` file at the repo root with your domain, then configure DNS per [GitHub Pages docs](https://docs.github.com/en/pages).

## Positioning notes

- Tone is **ML engineer who ships systems** (training, inference/serving, LLM infra, data, eval) — not an academic CV.
- Keep experience bullets **outcome-oriented** (latency, cost, reliability, scale).
- Keep SAMPLE labels until projects are real.

## License

Content © Jinlong Ji. Feel free to adapt the HTML/CSS structure for your own portfolio.
