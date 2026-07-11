# Deploy — Maa Sarada Mandir Trust site

This folder is a self-contained static site. No build step.

## Push to GitHub
From this folder's parent (or after copying `site/` into your repo):

    git init            # if not already a repo
    git add .
    git commit -m "Add Maa Sarada Mandir Trust site"
    git branch -M main
    git remote add origin https://github.com/bodhayanm/maasaradamandirtrust.git
    git push -u origin main

## Deploy on Vercel
1. https://vercel.com/new → Import `bodhayanm/maasaradamandirtrust`
2. **Root Directory:** set to `site` (if you pushed the whole repo) — or leave as `.` if these files are at the repo root
3. Framework preset: **Other** (static). No build command, no output dir needed.
4. Deploy. You'll get a *.vercel.app URL.

## Local preview
    python3 -m http.server 8000   # then open http://localhost:8000
