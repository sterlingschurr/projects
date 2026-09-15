# Project Showcase — Setup

## 1. Get this into a GitHub repo

- Create a new repo on GitHub (public, or private with GitHub Pro/Team/Enterprise
  if you want it private).
- Push everything in this folder to the repo root.

## 2. Turn on GitHub Pages

- In the repo: Settings → Pages → under "Build and deployment", set
  Source to "Deploy from a branch", branch to `main`, folder to `/ (root)`.
- Save. GitHub will build the site automatically. It appears at
  `https://<your-username>.github.io/<repo-name>/` within a minute or two.
- Any time you push a change, GitHub rebuilds it automatically. No manual
  build step, ever.

## 3. Adding a new project

Create a new file in `_projects/`, e.g. `_projects/my-new-thing.md`:

```markdown
---
title: My New Thing
skills: [javascript, react]
date: 2025-01-10
---

Description of the project goes here, normal markdown.
```

That's it. It will automatically:
- Appear on the homepage
- Appear under "javascript" and "react" on the /skills/ page
- Get its own page at /projects/my-new-thing/

## 4. Keeping skill names consistent

Nothing stops you from typing `Python` in one file and `python` in another —
Jekyll will treat those as two different skills. Pick a naming convention
(lowercase, hyphenated, e.g. `rest-api` not `REST API`) and stick to it.
If this list grows past ~15-20 skills, consider keeping a master list in
`_data/skills.yml` to copy from when tagging new projects.

## 5. Previewing changes locally (optional, but recommended)

Without this, you're pushing to GitHub blind and waiting for the build to
see results. To preview on your own machine first:

```bash
# One-time setup (needs Ruby installed)
gem install bundler jekyll
bundle init
bundle add jekyll

# Every time you want to preview
bundle exec jekyll serve
# then open http://localhost:4000
```
