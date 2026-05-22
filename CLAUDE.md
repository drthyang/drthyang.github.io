# Personal Website — thyang-phys.github.io

Jekyll + Minimal Mistakes (dark skin). Hosted on GitHub Pages at https://drthyang.github.io.

## Tech stack
- Jekyll with `remote_theme: mmistakes/minimal-mistakes`
- Ruby version pinned in `.ruby-version`
- Navigation defined in `_data/navigation.yml`
- Publication data driven by `_data/publications.yml`
- All CSS is inline per page file (no separate per-page stylesheets)

## Key conventions
- Dark theme accent color: `#4facfe` (blue) — use this for all highlights, links, borders
- Body text color: `#b0b0b0` on dark backgrounds
- Images live in `assets/images/`
- Pages use `layout: single` with `author_profile: true` unless they need a splash header
- Responsive breakpoint for card grids: `max-width: 768px` or `900px`

## Site structure
| File | Purpose |
|---|---|
| `index.md` | Homepage — hero + two core cards + recent highlights |
| `about.md` | Bio, skills, education |
| `research.md` | Research project cards (splash layout with header image) |
| `software.md` | Software package cards (splash layout with header image) |
| `publications.md` | Publication list rendered from `_data/publications.yml` |
| `learning-notes.md` | Notes/projects page (currently has placeholder content) |
| `blog/index.md` | Blog index, posts live in `_posts/` |

## Known missing files
- `assets/resume.pdf` — CV download link is live but file not uploaded yet
- Several placeholder images in `assets/images/` (see TODO.md for full list)

## Author info
- Name: Tsung-Han Yang, Ph.D.
- Role: Postdoctoral Researcher at Oak Ridge National Laboratory (ORNL)
- Focus: Quantum Materials (neutron scattering, RMC modeling) + Data Science / Quant Finance
- GitHub: https://github.com/drthyang
