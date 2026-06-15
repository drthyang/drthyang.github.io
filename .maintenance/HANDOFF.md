# Site Maintenance Handoff

## Current State
- Repository: `drthyang/drthyang.github.io`
- Local branch: `main`
- Remote branch: `origin/main`
- Public site: `https://drthyang.github.io`
- Framework: Jekyll with `remote_theme: mmistakes/minimal-mistakes`
- Ruby version: pinned in `.ruby-version`

## Guardrails
- Do not edit public website content unless the requested change names the target page or section.
- Public content lives in root pages such as `index.md`, `about.md`, `research.md`, `software.md`, `publications.md`, `learning-notes.md`, `blog/index.md`, `_posts/`, and `_data/`.
- Treat `_site/` as generated output. Do not use it as the source of truth for content edits.
- Root Markdown maintenance files can be rendered by Jekyll. Keep internal handoffs and maintenance notes in `.maintenance/`.
- Before making content changes, run `git status --short --branch` and confirm whether the working tree is clean.

## Preview Workflow
Use Jekyll from the repo root so the preview is rendered from current source files:

```sh
PATH=/Users/tt9/.rbenv/shims:/usr/bin:/bin:/usr/sbin:/sbin bundle exec jekyll serve --host 127.0.0.1 --port 4002
```

Open `http://127.0.0.1:4002/`.

Do not preview by serving `_site/` directly with `python -m http.server`; checked-in `_site/` can be stale and may not match the current source/public build.

## After Preview
- Stop the local Jekyll server.
- Check for generated-file churn with `git status --short`.
- If only `_site/` files changed because of preview/build, restore them before continuing:

```sh
git restore -- _site
```

## Last Maintenance Notes
- The working tree was cleaned back to `main...origin/main` before this handoff update.
- Local preview on `4002` was used for review and then stopped.
- No source website content was intentionally changed as part of this maintenance cleanup.
