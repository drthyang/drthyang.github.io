# TODO

## Active
- [ ] Upload `assets/resume.pdf` — CV download button on homepage and nav are both broken until this exists

## Backlog

### Content fixes
- [ ] Verify Nat. Commun. DOI `10.1038/s41467-026-71683-7` once paper is officially published

### Style fixes
- [ ] Replace SVG concept visuals with final paper figures or project screenshots when available

### Enhancements
- [ ] Add arxiv links to publications that have preprints (`_data/publications.yml` — all `arxiv` fields are currently empty)
- [ ] Recent Highlights section on `index.md` is hardcoded — consider pulling from `_data/` or front matter so it stays in sync with publications

## Done
- [x] Added local concept visuals for research, software, and learning-notes cards
- [x] Rewrote the homepage for stronger industry-facing positioning
- [x] Added industry direction and categorized technical stack to `about.md`
- [x] Reworked software cards into compact technical case studies
- [x] Rewrote "Physics-informed Neural Network" card in `learning-notes.md`
- [x] Fixed `learning-notes.md` CSS to align with the dark theme
- [x] Unified `.highlight` color in `about.md` to match the site accent
- [x] Publication list sorted by year with accent-colored year column
- [x] Author name auto-bolded via Liquid `replace` filter in `publications.md`
- [x] Responsive card layouts for research, software, and learning-notes pages
- [x] Dark theme applied consistently across research, software, publications pages
- [x] Blog posts set up (`_posts/2026-01-20-CoSn.md`, `_posts/2026-02-16-mn3sn.md`)
