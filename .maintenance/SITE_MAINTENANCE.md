# Site Maintenance Notes

## Repository Layout
- `index.md`: homepage.
- `about.md`: biography, skills, education, and profile details.
- `research.md`: research portfolio cards.
- `software.md`: packages and tools cards.
- `publications.md`: publication list rendered from `_data/publications.yml`.
- `_data/navigation.yml`: top navigation.
- `_data/publications.yml`: publication metadata.
- `_posts/`: blog posts.
- `assets/images/`: images and visual assets.
- `_site/`: generated Jekyll output; not the editing source.

## Styling Conventions
- Keep per-page CSS inline in the page file.
- Use the accent color `#4facfe` for highlights, links, and borders.
- Use `#b0b0b0` for body text on dark backgrounds.
- Keep cards at `8px` border radius or less.
- Use responsive breakpoints around `768px` or `900px`.

## Safe Edit Process
1. Start with `git status --short --branch`.
2. Edit only the requested page, data file, or maintenance doc.
3. Preview with `bundle exec jekyll serve`, not a static `_site/` server.
4. Verify the target page in the browser.
5. Restore generated `_site/` churn unless the deployment workflow explicitly needs it.
6. Review `git diff --check` and `git diff --stat` before committing.

## Known Maintenance Items
- `assets/resume.pdf` is still missing, so the CV link is live but unresolved.
- Placeholder/concept visuals remain in several cards and can be replaced with final figures or screenshots later.
- `_data/publications.yml` has empty `arxiv` fields that can be filled when preprints are available.
- Homepage recent highlights are hardcoded and can drift from `_data/publications.yml`.

## Do Not Accidentally Publish
- Internal notes should stay under `.maintenance/`.
- Do not add new root-level Markdown handoff files unless they are meant to become public pages.
- Avoid editing `_config.yml` `include` or `exclude` settings as part of routine content changes.
