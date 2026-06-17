# Hao Zou Personal Website

This is a redesigned GitHub Pages personal website based on Jon Barron's academic website style.

## Deployment

Recommended path: keep the existing `haozou-official.github.io` repository, back it up, and replace the contents with this folder. You do not need to initialize a new repository unless you want to change the GitHub Pages URL.

```bash
# 1. Clone your existing GitHub Pages repo
git clone git@github.com:haozou-official/haozou-official.github.io.git
cd haozou-official.github.io

# 2. Optional backup branch
git checkout -b backup-old-site
git push origin backup-old-site

# 3. Return to main and replace files
git checkout main
rm -rf * .[^.]* 2>/dev/null || true
# copy all files from this folder into the repo root

# 4. Commit and deploy
git add .
git commit -m "Redesign personal website"
git push origin main
```

GitHub Pages should update at `https://haozou-official.github.io/` within a few minutes.

## Files to update soon

- `files/Hao_Zou_CV.pdf`: replace with your finalized CV.
- `images/papers/*.svg`: replace placeholder figures with final paper figures when available.
- OSWorld 2.0 links: add arXiv/project page after public release.
- Double-blind caution: if any under-review venue prohibits public author-identifying disclosure, temporarily change the status to "Manuscript, 2026" or hide the row.

## Template credit

Adapted from Jon Barron's website template: https://github.com/jonbarron/jonbarron.github.io
