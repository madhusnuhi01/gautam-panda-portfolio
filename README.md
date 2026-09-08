# Gautam Panda — Portfolio Website

A static, single-repo portfolio site for Prof. Dr. Gautam Panda (Chief Scientist & Professor, AcSIR, CSIR-Central Drug Research Institute). No build step — plain HTML/CSS/JS, ready for GitHub Pages.

## Files

- `index.html` — main portfolio page (about, research, career, awards, impact, selected publications, patents, group, contact)
- `publications.html` — full chronological list of 141 journal papers
- `style.css` — shared styles
- `script.js` — small script for the mobile nav toggle

## Publish it on GitHub Pages

1. Create a new repository on GitHub (e.g. `gautam-panda-portfolio`).
2. Upload these four files (or the whole folder) to the repository — either via the GitHub web UI ("Add file → Upload files") or with git:
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```
3. In the repository, go to **Settings → Pages**.
4. Under **Build and deployment → Source**, choose **Deploy from a branch**.
5. Under **Branch**, choose `main` and folder `/ (root)`, then **Save**.
6. GitHub will publish the site within a minute or two at:
   `https://<your-username>.github.io/<repo-name>/`

## Updating content later

- Edit the text directly inside `index.html` / `publications.html` — everything is plain, readable markup, no build tooling required.
- Contact details, links (CDRI profile, Google Scholar, ORCID, lab site) and the stat numbers in the hero section are the easiest things to keep current — search for them near the top of `index.html`.
- To add a new publication, copy an existing `<li class="pub">…</li>` block in `publications.html` under the correct `<div class="year-head">` (add a new year heading if needed).

## Notes on what was left out

For privacy, the site omits the date of birth and home/residential address that appeared in the source CV, keeping only the institutional (CDRI) contact details. Remove or add anything you'd like — it's your content.
