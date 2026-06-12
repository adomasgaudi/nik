# Session log — 2026-06-12

## Changes made

### Collapsible sections
- Added click-to-collapse/expand to all 10 numbered sections
- Chevron icon rotates when closed
- State persisted in `localStorage` (survives page reload)

### CLAUDE.md created
- Documents deployment workflow: commit → push feature branch → merge to `main` → live
- `main` is canonical — every change must end up there

### Version bumps
- v.5 → v.6 → v.7 → v.8 (testing Netlify deploy pipeline)

### Settlement diagram redesign (section 10)
**Old**: debtors left, creditors right, flow lines between them

**New**:
- All 8 people on the left (dark card = paid, light card = owes)
- 4 expense items on the right (Brazylija 600€, Maistas 500€, Dažasvydis 350€, RC 180€)
- **Gray arrows** (thin web) = each person's equal share of each expense (203.75€ / 8 split)
- **Black arrows** (thick, labeled) = what each payer actually fronted
- **Curved settlement arrows** = 7 greedy min-transactions between people, arcing left
- Legend at bottom explaining line types

## Deployment notes
- Netlify was not picking up changes — likely had wrong branch set (not `main`)
- Fix: Netlify dashboard → Site config → Build & deploy → Production branch → set to `main`
