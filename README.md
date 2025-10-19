# gh-deployment-workflow

Simple demo repo that deploys `index.html` to GitHub Pages **only when `index.html` is changed**.

## What this repo contains
- `index.html` — the web page that will be published to GitHub Pages.
- `.github/workflows/deploy.yml` — GitHub Actions workflow that deploys to Pages when `index.html` changes.

## How it works
The workflow triggers on `push` to the `main` branch, but **only** if the `index.html` file was among the changed files. The workflow uploads `index.html` as a Pages artifact and deploys it using GitHub's official Pages actions.

## Live site
When deployed, the site will be available at:
https://aminexi.github.io/gh-deployment-workflow/
<img width="1477" height="446" alt="image" src="https://github.com/user-attachments/assets/cae503a9-705e-4142-9993-304620538276" />


## To test locally / push changes
1. Make a change to `index.html`.
2. Commit and push to `main`.
3. The workflow will run only if `index.html` was changed. Check the Actions tab and Pages status for deployment logs.



https://roadmap.sh/projects/github-actions-deployment-workflow
