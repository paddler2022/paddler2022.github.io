# paddler2022.github.io

Personal academic homepage for **Yuheng Lu (卢昱恒)**, live at
<https://paddler2022.github.io>.

Built with the [al-folio](https://github.com/alshedivat/al-folio) Jekyll theme.
GitHub Actions builds and deploys the site automatically on every push — you never
run a server yourself.

## Where to edit things

| What | File |
| --- | --- |
| Name, site title, URL, favicon, Scholar name | `_config.yml` |
| Bio, subtitle, profile photo caption | `_pages/about.md` |
| Publications (titles, arXiv, code, abstracts) | `_bibliography/papers.bib` |
| News items (homepage) | `_news/*.md` |
| CV page content | `_data/cv.yml` |
| Contact / social links | `_data/socials.yml` |
| Profile photo | `assets/img/prof_pic.jpg` |
| CV PDF | `assets/pdf/CV_Yuheng_Lu.pdf` |

Search the files for `EDIT` to find the placeholders that still need your input:

- **Google Scholar ID** in `_data/socials.yml` (`scholar_userid`).
- **Co-author names** and **code/repo links** in `_bibliography/papers.bib`
  (currently placeholder names like `Coauthor, A.`; the arXiv links are already set).

## Deploy (one-time setup)

1. Push this repo to `main`.
2. In **Settings → Actions → General → Workflow permissions**, select
   **Read and write permissions** (so the deploy action can publish).
3. Wait for the **Deploy site** workflow (Actions tab) to finish — it builds the site
   and pushes the result to a `gh-pages` branch.
4. In **Settings → Pages**, set **Source → Deploy from a branch → `gh-pages` / (root)**.

After that, every push to `main` re-deploys automatically.

## Local preview (optional, needs Docker)

You don't need this to publish, but if you want to preview locally:

```bash
docker compose up
# then open http://localhost:8080
```

Stop with `Ctrl+C`. (Requires Docker Desktop.)
