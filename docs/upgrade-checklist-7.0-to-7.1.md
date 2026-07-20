---
title: Susan Allen — Squarespace 7.0 → 7.1 Upgrade Checklist
created: 2026-07-20
type: checklist
status: DRAFT
client: Susan Allen, LMFT
scheduled_upgrade: 2026-08-03 (Monday, WFC back from OOO)
framework_source: "[[https://support.squarespace.com/hc/en-us/articles/360038270572-Moving-from-Squarespace-version-7-0-to-version-7-1]]"
related:
  - "[[Work/WFC/studio/squarespace-development-reference]]"
  - "[[docs/sow]]"
  - "[[docs/kickoff-notes]]"
  - "[[docs/audit-template-shortlist]]"
  - "[[docs/email-2026-08-03-upgrade-notice]]"
tags: [wfc, susan-allen, squarespace, 7.0-to-7.1, migration, checklist, upgrade]
---

# Susan Allen — Squarespace 7.0 → 7.1 Upgrade Checklist

> **Why this is happening:** Clove (and all 7.1 templates) require Squarespace 7.1. Susan's current site is on 7.0 (set up 8-9 years ago by a family member; the Arial font fallback behavior is a 7.0 tell). The 7.0 → 7.1 upgrade is the platform-level foundation for the Clove template work. **Clove itself is a 7.1 template** — confirmed via the Squarespace Health & Beauty gallery.
>
> **When:** Mon 8/3/2026, ~9am PT. First thing when WFC returns from OOO. Pre-OOO is 7/22-8/2.
>
> **Source article:** [Moving from Squarespace version 7.0 to version 7.1](https://support.squarespace.com/hc/en-us/articles/360038270572-Moving-from-Squarespace-version-7-0-to-version-7-1)

---

## Phase 0 — Pre-Upgrade Verification (8/1 weekend or 7/30-7/31 evening)

> Do these BEFORE 8/3. Some are quick, some require a check on Susan's account.

- [ ] **Verify current platform version.** Log into Susan's Squarespace account → Settings → check version. Must be on 7.0 for the in-place upgrade to work. If already 7.1, skip Phases 1-2.
- [ ] **Verify current template is not discontinued.** Settings → check template name. The 7.0 → 7.1 upgrade tool will block if the template is discontinued. Susan's template was set up 8-9 years ago — could be an old Wells/Bedford/etc. If discontinued, swap to a current 7.0 template first (e.g., Bedford, Brine, or similar 7.0 template that's still supported).
- [ ] **Verify Developer Mode is OFF.** Settings → Advanced → Developer Tools → Developer Mode should be OFF. The article is explicit: "If you can't update to 7.1, this means you're using an unsupported template or developer mode is still active." Susan is not a developer — should be off by default.
- [ ] **Verify page count is under 150.** The article says: "The update tool has a limit of 150 pages. If your site has more than 150 pages, check this list to learn which pages count toward the limit." Susan has ~6 pages (HOME, ABOUT, FOCUS, THERAPY, CONTACT, RESOURCES) — well under.
- [ ] **Verify Squarespace plan tier.** Per the dev reference: Code Injection + Code Block JS require **Core+ ($23/mo)**. If Susan is on Personal, recommend plan upgrade before 8/3. (This is a Susan-side decision, not blocking the platform upgrade, but blocking the WFC build work post-7.1.)
- [ ] **Verify Susan's 2FA status is set.** Susan said on the kickoff "I need to, like, lock it down." Confirm before the upgrade so 2FA prompts don't block Frank mid-upgrade.
- [ ] **Inventory Susan's custom code.** Per the article: "Keep in mind that any changes you've made in your site's built-in style editor will disappear, even if you made the changes before enabling developer mode" — N/A for Susan (no dev mode). But verify what's in Custom CSS + Code Injection so we can confirm it carries over.
- [ ] **Take screenshots of current 7.0 site.** For "before" reference. Audit folder already has these (`docs/audit-screenshots/current/`).

---

## Phase 1 — The 7.0 → 7.1 Upgrade (8/3 morning, ~9-11am PT)

> Frank leads. Susan does not need to be online.

- [ ] **Log into Susan's Squarespace account** (`susanallenlmft@gmail.com` / site username "Suzanne"; password in Frank's 1Password). If 2FA prompts, coordinate with Susan in real-time.
- [ ] **Open the Design panel.** Look for the "Update to Version 7.1" button. If absent: site is already 7.1 OR template is unsupported OR developer mode is on.
- [ ] **Click "Update to Version 7.1"** → review the preview flow → click "Get Started."
- [ ] **Read the info screens.** The article notes: "All other site functions are disabled until you publish or end the preview."
- [ ] **Click "Preview site in 7.1."** This creates a 7.1 preview environment alongside the live 7.0 site. Live site is unaffected.
- [ ] **In preview: click "Edit" in the top-left.** Walk through each page and confirm content carried over:
  - [ ] Home page
  - [ ] About page
  - [ ] Focus (specialties) page
  - [ ] Therapy page
  - [ ] Contact page
  - [ ] Resources (= /blog, 3 posts)
  - [ ] Header / Footer (note: footer "POWERED BY SQUARESPACE" credit)
  - [ ] Custom CSS (under Design → Custom CSS) — verify the code is preserved
  - [ ] Code Injection (Settings → Advanced → Code Injection) — verify header/footer code preserved
  - [ ] Navigation structure
  - [ ] Logo / branding
- [ ] **Document any content that didn't migrate cleanly.** Per the article, certain 7.0 elements have "alternative options" in 7.1. Specific known issues:
  - Sidebar content (in block fields) — may need rebuilding
  - Cover pages — N/A for Susan
  - Custom blocks — Susan's site is standard, low risk
  - Index page item layouts — N/A
- [ ] **Test the /services URL behavior.** The audit noted this silently redirects to home. In 7.1 the behavior may change. Document.
- [ ] **If 7.1 preview looks good: click "Publish update."** ⚠️ **This can't be undone.** Per the article: "When you're ready to update your site to version 7.1, click Publish update. This can't be undone."
- [ ] **Site is now on 7.1.** Live domain serves 7.1 with migrated content. Same URLs, same content, new backend.

---

## Phase 2 — Post-Upgrade Verification (8/3 afternoon, ~1-3pm PT)

> Frank confirms the upgrade took cleanly before starting template work.

- [ ] **Walk the live site** at susanallentherapy.com on desktop + mobile. Verify:
  - [ ] All pages render
  - [ ] Navigation works
  - [ ] Custom CSS still applied (font, color, spacing)
  - [ ] Footer + header render correctly
  - [ ] No broken links
  - [ ] No 404s (especially the /services silent-redirect issue)
- [ ] **Test Custom CSS** in Design → Custom CSS editor. Verify the WFC/Lauren/Susan custom code is intact. Per the article: "Custom code in your Custom CSS and Advanced code injection panels" is preserved.
- [ ] **Check Squarespace version in Settings** — confirm "Version 7.1" is shown.
- [ ] **Email Susan** with "upgrade complete, site is on 7.1, no visible change yet, template work starts this week" — see [[email-2026-08-03-upgrade-notice]] for the template.

---

## Phase 3 — Clove Template Application (8/4 onward)

> This is the actual visual change. Susan will see the new template applied to her content.

- [ ] **Open the Clove template in the template gallery** (`squarespace.com/templates` → search "Clove") to confirm the live demo URL matches the audit's reference (`clove-fluid-demo.squarespace.com`).
- [ ] **In Susan's 7.1 site: Design → Template → select Clove.** Per the article: "All version 7.1 templates have the same features and design options."
- [ ] **Apply WFC design tokens** via Custom CSS (audit + token layer in `design-system/README.md`):
  - [ ] Color tokens (Cool variant — slate blue + sage + warm cream)
  - [ ] Typography (Cormorant Garamond display + Atkinson Hyperlegible body)
  - [ ] Spacing scale (8pt)
  - [ ] Motion defaults (calm hover effects, `prefers-reduced-motion` respected)
- [ ] **Map Susan's content onto Clove's structure** (per `mockups/clove/index.html`):
  - [ ] Hero: "Reproductive & perinatal mental health. Solo private practice, SF + Marin"
  - [ ] "My approach" 3-card grid (Relational / Integrative / Specialty-driven)
  - [ ] Specialties 2x2 grid (Infertility & family building, Pregnancy & postpartum, Reproductive mental health, Women's mental health)
  - [ ] Credentials single-card with ASRM/PSI/Donor Conceived prominence
  - [ ] Testimonial (placeholder until Susan provides)
  - [ ] Blog grid (3 existing posts)
  - [ ] "Get in touch" CTA → "Email Susan" (per SOW email-only intake)
  - [ ] Footer with HIPAA-aware communications notice
- [ ] **Fix the /services silent-redirect** — build the Specialties page as a real page (this is the SOW's primary content goal).

---

## Phase 4 — Content + Config (8/4-8/18, Milestones 3-5 from SOW)

> Per the SOW + kickoff notes. Most of this work falls under Milestone 3-5.

- [ ] **Milestone 3: Template config + Specialties page** (Week of 8/4)
- [ ] **Milestone 4: Content + FAQ + OKF/knowledge scaffold** (Week of 8/11)
- [ ] **Milestone 5: On-page SEO + WCAG 2.1 AA + preview link** (Week of 8/18)
- [ ] **HIPAA-aware communications notice** (Lauren drafted 7/18, needs review + apply)
- [ ] **Informed consent language** (Lauren drafted 7/18, needs review + apply)

---

## Phase 5 — Phase 1 Wrap (~8/22)

- [ ] **Critique Report** for each page (per [[Work/WFC/studio/deliverables]] — standard WFC deliverable)
- [ ] **Susan review + final approval**
- [ ] **Invoicing** (Phase 1 = $1,000 floor, 8 hrs × $125; balance due at launch)
- [ ] **Phase 2 conversation** (SEO/AI findability, $1,600-$3,000 range)

---

## Risks + Mitigation

| Risk | Severity | Mitigation |
|------|----------|-----------|
| Susan's 7.0 template is discontinued (blocks upgrade) | HIGH | Inventory template in Phase 0; swap to current 7.0 template if needed |
| Custom CSS / Code Injection doesn't carry over | MEDIUM | Documented pre-upgrade; can re-add manually if needed |
| Blog content doesn't migrate cleanly | MEDIUM | 3 posts on classic editor — should be fine; verify in preview |
| Footer "POWERED BY SQUARESPACE" badge doesn't carry | LOW | Acceptable per SOW; can be styled via Custom CSS |
| /services URL behavior changes | LOW | Already 404s silently; will rebuild as real Specialties page |
| Susan's plan tier blocks Code Injection | MEDIUM | Verify in Phase 0; recommend Core+ upgrade before 8/3 |
| 2FA blocks Frank mid-upgrade | LOW | Confirm Susan's 2FA status pre-OOO; coordinate in real-time if needed |
| Squarespace service outage 8/3 | LOW | Pick a backup date (8/4 or 8/5) if 8/3 has issues |

## What Susan Will Notice

- **8/3 (upgrade day):** Nothing visible. Site looks the same. Same URLs, same content. The backend is now 7.1.
- **8/4-8/5 (template application):** Site starts looking different. New template (Clove), new colors (WFC Cool palette), new layout. Susan will see the new template appear.
- **8/18-8/22 (Phase 1 wrap):** Full audit + final touches. Susan reviews and approves.

## Rollback Plan

Per the article: "This can't be undone." Once 7.1 is published, there's no in-place rollback to 7.0. If something goes catastrophically wrong:
- Restore content from Squarespace's automatic backups (Squarespace keeps 30 days of backups; check Settings → Site Availability)
- Worst case: rebuild from a 7.1 trial with copied content
- **Note:** This is a real risk. Plan accordingly. The preview environment is the testing ground — never publish 7.1 without thorough preview.

---

*Compiled by Mavis 2026-07-20 18:50 PT. Owner: Frank. Source: Squarespace support article + dev reference + audit + kickoff notes. Send the companion email ([[email-2026-08-03-upgrade-notice]]) to Susan 7/21 (last day before OOO) so she has a heads-up.*
