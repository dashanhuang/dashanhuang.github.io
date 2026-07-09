# dashanhuang.github.io

Personal academic homepage (static HTML, no build step). Clean academicpages-style
layout: left profile sidebar + main column, fully responsive. All assets bundled.

## Files
- `index.html` — Home (bio, contact, research interests, publications, working papers)
- `teaching.html` — Teaching
- `assets/css/style.css` — styling
- `assets/img/dashan.jpg` — profile photo
- `assets/cv/CV_Dashan_Huang.pdf` — CV
- `assets/files/…` — appendices / data / code linked from publications

Everything the pages link to locally is included — nothing else to add.
(spcaest.m and the JQFA/SSRN paper links point to their external hosts by design.)

## Deploy to dashanhuang.github.io
A user site repo MUST be named exactly `dashanhuang.github.io`.

1. Create a new public repo on GitHub named `dashanhuang.github.io`.
2. Put the contents of this folder (index.html at the repo root) into it. Via the web UI: "Add file → Upload files", drag everything in, Commit. Or via git:
   ```
   git init && git add . && git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/dashanhuang/dashanhuang.github.io.git
   git push -u origin main
   ```
3. GitHub → repo → Settings → Pages → Source: "Deploy from a branch", Branch: `main` / root. Save.
4. Wait ~1 minute, then visit https://dashanhuang.github.io

## Notes
- Contact email: dashanhuang@smu.edu.sg
- To add a new paper, copy an existing `<li>` in `index.html` and edit.
