# BSc Data Science for Responsible Business — Student Project Portfolio

A simple 2-page site:
- `index.html` — the program description and the two partner logos
- `projects.html` — 2–3 student projects (currently empty placeholder slots)

No build step, no framework — plain HTML/CSS. Open `index.html` in a browser to preview it
locally, no internet needed except to load the two Google Fonts.

## How to add a project (do this in `projects.html`)

Open `projects.html` in any text editor. Each project is one block that looks like this:

```html
<article class="proj-card">
  <span class="ph-tag">[Optional tag — sector, team, etc. Delete if unused]</span>
  <h3>[Project title]</h3>
  <p class="ph-desc placeholder">[Add a 2–3 sentence description: the problem it solves, what the students
    built, and the tools or technologies used.]</p>
  <a class="proj-link" href="#" target="_blank" rel="noopener">View project →</a>
</article>
```

For each project, edit exactly three things:

1. **Title** — replace `[Project title]` inside the `<h3>` tag.
2. **Description** — replace the bracketed text inside the `<p class="ph-desc placeholder">` tag with
   your real 2–3 sentence description. Once you've done that, delete the word `placeholder` from
   `class="ph-desc placeholder"` (leave just `class="ph-desc"`) — that word is only there to show the
   text in italics as a placeholder.
3. **Link** — replace `href="#"` with the real project link (a GitHub repo, a live demo, a PDF report,
   a Google Drive folder — anything with a URL works).

The small tag above the title (`<span class="ph-tag">`) is optional. Use it for a sector, a team size,
or anything short — or delete that whole line if you don't need it.

**To add a 4th project:** copy one entire `<article class="proj-card"> ... </article>` block and paste
it just before the closing `</div>` of the projects grid (search for `<!-- HOW TO ADD A PROJECT` in the
file — the instructions are also repeated there as a comment).

**To remove a project:** delete its whole `<article>...</article>` block.

## Swapping in the real logos

Both logos are currently placeholders (simple text-based stand-ins), in `assets/`:
- `assets/logo-emlyon-placeholder.svg`
- `assets/logo-centrale-placeholder.svg`

Replace these two files with your official logo files (keep the same filenames, or update the `src=`
paths in the `<img>` tags in both `index.html` and `projects.html` if you rename them). The emlyon logo
is listed first in the code so it appears to the left of the Centrale Lyon logo, as requested — keep
that order if you swap the files.

## Editing the program description

The description lives in `index.html`, inside the `<div class="program-desc">` block. Edit the text
directly there — it's plain HTML paragraphs (`<p>...</p>`).

## Deploying to GitHub Pages

1. Create a repository and upload all the files, **keeping the folder structure** (the `assets/` folder
   must stay next to `index.html` and `projects.html`, and `style.css` must stay at the same level too).
2. Go to the repo's **Settings → Pages**, set **Source** to the `main` branch, folder `/ (root)`, then
   save.
3. Your site will be live within a minute or two at:
   `https://<your-username>.github.io/<your-repo>/`

You can also just double-click `index.html` to preview the site locally before publishing anything.
