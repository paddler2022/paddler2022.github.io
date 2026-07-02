# paddler2022.github.io

Personal academic homepage for **Yuheng Lu (卢昱恒)**, served at
<https://paddler2022.github.io>.

Plain HTML / CSS / JS — **no build step**. GitHub Pages serves `index.html` directly
(a `.nojekyll` file disables Jekyll processing).

## Structure

```
index.html            # the whole page (all content lives here)
assets/
  css/style.css       # styling + light/dark theme
  js/main.js          # theme toggle + footer year
  img/profile.jpg     # portrait
  img/favicon.svg     # favicon (initials)
  pdf/CV_Yuheng_Lu.pdf# CV linked from the header
```

## Editing

Everything you'll want to change is in `index.html`, marked with `<!-- EDIT ... -->`
comments where relevant:

- **Contact links** — search for `EDIT:` in the hero section and drop in your real
  Google Scholar / GitHub / email URLs. (GitHub already points to `paddler2022`.)
- **Publications** — each `<li class="pub">` block. Replace the `…co-authors…`
  placeholders with the real author lists, and swap the `href="#"` on the
  **arXiv / Code** buttons for the real links once they're public.
- **News** — the `<ul class="news">` list; newest on top.
- **PhD-seeking callout** — the highlighted box in the hero; edit the target term or
  remove it entirely.
- To replace the photo, drop a new image at `assets/img/profile.jpg`.

## Local preview

```bash
python -m http.server 8000
# then open http://localhost:8000
```

## Deploy

Push to `main`; enable **Settings → Pages → Deploy from branch → main / (root)**.
The site updates automatically on every push.
