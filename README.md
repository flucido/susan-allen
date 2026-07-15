# Susan Allen — Project Repository

> **GitHub-backed design + project workspace for the Susan Allen, LMFT engagement.**
> Canonical engagement record stays in the Obsidian vault at `~/workspace/leads/wfc-susan-allen/`; this repo is for the **design artifacts** (mockups, design system, web-deliverable infrastructure) that benefit from version control + backup.

## Status

- **Engagement:** Phase 1 (Squarespace template refresh + SEO/GEO + content)
- **Kick-off:** 2026-07-14 10:01–10:58 AM PT (Frank led, shared WFC Zoom account; Lauren not in attendance)
- **SOW signed:** 2026-07-08 · **$500 deposit received:** 2026-07-10
- **Template decision:** Susan picks by Fri 7/18 (pre-WFC OOO)
- **WFC OOO:** 2026-07-22 to 2026-08-02 (Frank + Lauren; Japan trip)
- **Phase 1 target wrap:** ~2026-08-22 (revised from 8/11–8/14 to absorb WFC OOO)

## Repo Layout

```
susan-allen/
├── README.md                         # this file
├── .gitignore                        # standard ignore for design repos
├── docs/                             # design process + decisions
│   ├── kick-off-summary.md           # 1-pager Frank sends Susan 7/15 AM
│   ├── post-meeting-feedback.md      # succinct feedback from call + transcript
│   └── framework-decision.md         # OKF vs aesthetic-triad (Frank decision)
├── design-system/                    # WFC tokens + Susan-specific variants
│   ├── README.md                     # design system exploration overview
│   ├── tokens-susan-cool.yaml        # leading palette (slate blue + sage + cream)
│   └── pad-coordinates.md            # target PAD per page archetype
├── mockups/                          # HTML mockups of 3 Squarespace templates
│   ├── clove/                        # primary recommendation (mental health)
│   ├── jenani/                       # backup (solo practitioner + FAQ)
│   └── clune/                        # color palette match (sage green)
├── web-deliverable/                  # Cloudflare Pages host for client reviews
│   └── (pending — see ~/workspace/Work/WFC/studio/web-deliverables/README.md)
└── archive/                          # completed / superseded work
```

## Working Conventions

- **HTML mockups:** single-file, self-contained, no build step. WFC tokens embedded as CSS custom properties. `prefers-reduced-motion` respected. WCAG 2.1 AA.
- **Screenshots:** saved alongside the mockup (`screenshot-1-hero.png`, `screenshot-2-approach.png`, etc.) for quick review.
- **Token changes:** edit `design-system/tokens-susan-cool.yaml` first, then propagate to mockups.
- **Commits:** short imperative subject lines, body explains why. Co-authored if Frank + Mavis work on the same change.
- **Backups:** GitHub is the canonical source. Local `~/projects/susan-allen/` is a working clone.

## Related (in Obsidian vault, not this repo)

- [[dossier]] — engagement source of truth
- [[kick-off-notes-2026-07-14]] — 7/14 meeting notes
- [[audit/README]] — pre-kick-off 6-gate audit + template shortlist
- [[../Work/WFC/studio/squarespace-development-reference]] — Squarespace 7.1 dev reference
- [[../Work/WFC/studio/web-deliverables/README]] — web-deliverable mechanism research (Cloudflare Pages recommended)

## First Deployment

The 3 template mockups (Clove, Jenani, Clune) will be the first deployable artifacts. Each will live in its own subfolder and be deployable to Cloudflare Pages for Susan's review.

---

*Repository initialized 2026-07-15 by Mavis for Frank Lucido (WFC).*
*Engagement: Susan Allen, LMFT · Phase 1 hybrid (Squarespace template + SEO/GEO + content).*
