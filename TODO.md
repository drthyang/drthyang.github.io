# TODO

## Active
- [ ] Upload `assets/resume.pdf` — CV download button on homepage and nav are both broken until this exists
- [ ] Add real images to replace all placeholders (see Placeholder Images section below)

## Backlog

### Content fixes
- [ ] Rewrite "Physics-informed Neural Network" card in `learning-notes.md` — currently copy-pasted from MarketLab (same description, tags, and GitHub link)
- [ ] Verify Nat. Commun. DOI `10.1038/s41467-026-71683-7` once paper is officially published
- [ ] Add Google Scholar link to `_config.yml` author sidebar (currently commented out)

### Style fixes
- [ ] Fix `learning-notes.md` CSS — uses light-mode colors (`#fff`, `#2c3e50`, `#e1e4e8`) that break the dark theme; align with site palette (`#111`/`#1a1a1a` background, `#b0b0b0` text, `#4facfe` accent)
- [ ] Unify `.highlight` color in `about.md` — currently `#0366d6` (GitHub blue); change to `#4facfe` to match rest of site

### Enhancements
- [ ] Add arxiv links to publications that have preprints (`_data/publications.yml` — all `arxiv` fields are currently empty)
- [ ] Recent Highlights section on `index.md` is hardcoded — consider pulling from `_data/` or front matter so it stays in sync with publications

## Placeholder images needed
These files are referenced in pages but do not exist in `assets/images/`:

| File | Used in |
|---|---|
| `PRL_Mn3Sn.png` | `research.md` — Topological Transport project |
| `placeholder_phonon.png` | `research.md` + `learning-notes.md` — Phonon project |
| `phonon_dos_placeholder.png` | `software.md` — RMC Phonon Dynamics card |
| `rmc_plot_placeholder.png` | `software.md` — RMCprofile Atomic Density card |
| `mpdf_placeholder.png` | `software.md` — Magnetic PDF card |
| `stock_plot_placeholder.png` | `software.md` — marketlab card |
| `placeholder_market.png` | `learning-notes.md` — MarketLab + PINN cards |

## Done
- [x] Publication list sorted by year with accent-colored year column
- [x] Author name auto-bolded via Liquid `replace` filter in `publications.md`
- [x] Responsive card layouts for research, software, and learning-notes pages
- [x] Dark theme applied consistently across research, software, publications pages
- [x] Blog posts set up (`_posts/2026-01-20-CoSn.md`, `_posts/2026-02-16-mn3sn.md`)
