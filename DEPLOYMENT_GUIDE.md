# GitHub Pages deployment checklist

## Upload the package

- Extract `yixuan-portfolio-github-pages-v1.zip`.
- Open the extracted folder.
- Upload its **contents**, not the containing folder, to the root of the repository.
- Confirm that `index.html`, `.nojekyll`, `.github/`, `certificates/`, and `projects/` are all at the repository root.

## Enable Pages

1. Go to **Settings → Pages**.
2. Set **Source** to **GitHub Actions**.
3. Go to **Actions** and wait for **Deploy portfolio to GitHub Pages** to complete.

## Make changes next week

1. Edit `index.html` for text, courses, project descriptions, captions, or code excerpts.
2. Replace or add files under `projects/` or `certificates/` for new images and project outputs.
3. Commit and push to `main`.
4. Wait for the automatic Pages workflow to finish.

You do not need to reconfigure GitHub Pages after ordinary content changes. Each push creates and publishes a new site version automatically.

## Common checks

- Keep paths and filename capitalization exact; GitHub Pages is case-sensitive.
- Do not move `index.html` out of the repository root.
- If an old image remains visible, use a new filename and update its path in `index.html` to bypass browser caching.
- Review the repository before making it public because every committed file is downloadable.
