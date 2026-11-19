# Yixuan Wang — Academic Portfolio

This repository contains the complete public, static version of the portfolio. It can be deployed directly with GitHub Pages and does not require Node.js, a database, or a separate build command.

## First deployment

1. Upload every file and folder in this repository to the `main` branch of the GitHub repository. Keep the folder structure unchanged.
2. On GitHub, open **Settings → Pages**.
3. Under **Build and deployment**, choose **GitHub Actions** as the source.
4. Open the **Actions** tab. The workflow named **Deploy portfolio to GitHub Pages** will run automatically.
5. When the workflow finishes, the site URL will appear in **Settings → Pages** and in the workflow summary.

If the repository is named `<username>.github.io`, the site URL will be `https://<username>.github.io/`. Otherwise it will normally be `https://<username>.github.io/<repository-name>/`.

## Updating the website later

You do not need to create a new deployment configuration. Edit the relevant files, commit the changes, and push them to `main`. GitHub Actions will automatically publish the new version.

The main page, text, interactions, and project definitions are in `index.html`. Website assets are organized as follows:

- `certificates/` — certificate images used by the website
- `projects/odis/` — ODIS project figures and interactive map
- `projects/hate-crimes/` — hate-crime project visualizations
- `projects/stress-models/` — stress-model project figures

When replacing an image, keeping the existing filename is the simplest option. If the filename changes, update the matching path in `index.html`.

## Local preview

From this repository folder, run:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000` in a browser. Stop the preview with `Ctrl+C`.

## Privacy

Only files required by the public website are included here. Raw transcripts, CV drafts, proposals, notebooks, source datasets, and other working documents are intentionally excluded. Do not commit private or confidential materials to a public repository.
