# Md Sarfraj — portfolio website

Source for **https://imdsarfraz.github.io**: a one-page portfolio built with plain
HTML and CSS (no frameworks, no build step), hosted free by GitHub Pages.

## What's in this folder

| File / folder | What it is |
| --- | --- |
| `index.html` | The whole website — all the text lives here |
| `assets/css/style.css` | Colours, fonts and layout (colours are set once at the top) |
| `assets/Md_Sarfraj_CV.pdf` | The CV behind every "Download CV" button |
| `assets/img/` | Favicon, phone icon and the preview image shown when the link is shared |
| `404.html` | The "page not found" page |
| `robots.txt`, `sitemap.xml` | Help Google find the site |
| `.nojekyll` | Tells GitHub Pages to publish the files exactly as they are |

## Preview your changes

Double-click `index.html` to open it in your browser. Refresh the browser after each save.

## Common edits - If you want to reuse

- **Change any text:** open `index.html` in VS Code, press `Ctrl+F`, search for a few words of the
  text you want to change, edit it, save. Each section starts with a comment such as
  `<!-- ===================== EXPERIENCE ===================== -->`.
- **Replace the CV:** save the new PDF as `assets/Md_Sarfraj_CV.pdf`, overwriting the old file.
  Keep the same name and every button keeps working.
- **Add a project:** copy one whole `<article class="project">` … `</article>` block, paste it
  below the last one, and change the text and the GitHub link.
- **Update the date in the footer:** search for `Last updated`.
- **Icons:** the LinkedIn, GitHub, YouTube and email logos are drawn once at the top of `index.html`
  (the `<svg class="icon-sprite">` block) and reused anywhere with
  `<svg class="icon" aria-hidden="true" focusable="false"><use href="#icon-github"></use></svg>`.

## Charts

The two project charts are drawn from real outputs in the linked repositories:
the retention matrix in `Cohort-Retention-Analysis` and the expected-loss-by-grade table printed in
`Credit-Risk-Modeling/Credit_Risk_Modelling.ipynb` (Part 13.1). Each chart has a "Show the data table"
button with the exact numbers. If the underlying analysis changes, update the chart and
its table together so they never disagree.

## Publish an update

After the first upload, publishing changes takes three commands in a terminal opened in this folder:

```powershell
git add -A
git commit -m "Describe what you changed"
git push
```

