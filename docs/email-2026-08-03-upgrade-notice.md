---
title: Susan — Squarespace Upgrade Notice (Email draft for 7/21 send)
created: 2026-07-20
type: email-draft
status: DRAFT — Frank to review, customize, send 7/21 (last day before OOO)
client: Susan Allen, LMFT
intended_send: 2026-07-21
scheduled_event: 2026-08-03 upgrade
tags: [wfc, susan-allen, email, upgrade, 7.1, clove, client-facing]
related: "[[docs/upgrade-checklist-7.0-to-7.1]]"
---

# Susan — Squarespace Upgrade Notice (Email draft)

> **To:** Susan Allen, LMFT `<susanallenlmft@gmail.com>`
> **From:** Frank Lucido `<frank.lucido@gmail.com>`
> **Subject:** Squarespace upgrade plan — heads up for Mon 8/3
> **Status:** DRAFT — Frank to review, customize, send 7/21
> **Suggested send time:** Tuesday 7/21 (last business day before WFC OOO 7/22-8/2)

---

## Email body

Hi Susan,

Quick heads-up before Lauren and I head out next week. One thing on the project timeline I want to make sure you're not surprised by: **on Monday 8/3, the morning I'm back from Japan, I'm going to do a Squarespace platform upgrade on your site — version 7.0 → 7.1.** Then I'll start applying the Clove template we picked.

This is a normal, well-trodden upgrade. Squarespace walks you through it in a preview environment before anything changes on your live site. But I want you to know it's coming, in case you happen to be online and see a "we're updating your site" message on Monday morning.

### What this is and why it matters

Your site was built 8-9 years ago on Squarespace version 7.0. Clove (the template we picked) is a 7.1 template, so we need to bring your account up to 7.1 first. This is the platform underneath the template — it's the foundation. Same as upgrading your phone's operating system so you can run a newer app.

### What you'll see, and when

| Date | What happens | What you see |
|---|---|---|
| **Mon 8/3 morning** | Squarespace platform upgrade (7.0 → 7.1) | Nothing visible. Same URLs, same content. Site looks the same. |
| **8/3 afternoon + following days** | Apply Clove template + WFC design system (colors, type, spacing) | **This is when the site starts looking different.** New template, new colors, new layout. |
| **Weeks of 8/4-8/18** | Content swap (specialties page, credentials, FAQ, HIPAA notice) | Site content gets refined. All your existing words stay, just better organized. |
| **~8/22 (target)** | Phase 1 wrap. You review + approve. | Final version. |

### What you need to do

**Nothing for the upgrade itself.** I'll do it all in the Squarespace backend. A few things I've already flagged for you from our last call:

- **2FA on Squarespace** — please confirm it's enabled (you mentioned you'd lock it down). I'll be logging in Monday morning and 2FA will help if Squarespace asks for a code.
- **If you want to be online for the upgrade** — happy to coordinate, but you don't have to be. The preview environment means I can test everything before it goes live.

### Things that won't change

- **Your domain** (`susanallentherapy.com`) — same URL, same DNS, same everything.
- **Your content** — all your existing text, your photos, your blog posts, your contact info. The upgrade preserves all of it.
- **Your contact email** — still `susanallenlmft@gmail.com` for intake (per our SOW).
- **Your professional email / Google Workspace** (if you have one set up) — separate from Squarespace, untouched.

### What changes (intentionally, on 8/3+)

- **The look.** New template, new colors (the cool blue palette we discussed), new typography. This is the visible change.
- **The /services page.** This is the one that currently silently redirects to your home page. I'm rebuilding it as a real "Specialties" page that lists your 4-5 leading specialty areas (infertility / pregnancy + postpartum / etc.) with the ASRM/PSI credentials front and center.
- **The H1 hierarchy.** Currently your H1 is your brand name on every page, which makes the page content hard to find. After the upgrade, the H1 = the page topic, brand stays in the header.

### Why I waited until 8/3

The upgrade is straightforward but it's not instant. There's a preview-and-publish workflow, and after the upgrade I need to apply the Clove template + the WFC design system + your content swaps. That's a few days of focused work, not something I can do in a hotel room. So I deliberately didn't start before the trip. The "real work" of Phase 1 starts 8/3.

### Phase 1 timeline (re-confirmed)

- 8/3: Upgrade + start template work
- 8/3-8/18: Template, content, SEO, WCAG, HIPAA
- ~8/22: Phase 1 wrap, you review + approve
- After: Phase 2 conversation (SEO/AI findability, $1,600-$3,000 range, separate SOW)

---

If you have any questions before 8/3, just reply. Otherwise I'll send a quick "upgrade complete" note Monday afternoon and we'll go from there.

Enjoy the rest of your week, and I hope your daughter decides to go to Japan next year — it's a magical place.

Best,
Frank

---

Frank Lucido
WellFull Collective
frank.lucido@gmail.com

---

## Notes for Frank

- **Send timing:** 7/21 (Tue), before WFC OOO. Susan will have it before the break.
- **Tone:** Warm but practical. Personal note at end (Japan / daughter) is from the kickoff — Susan mentioned her daughter wants to go to Japan, and Frank + Lauren are going. Light callback.
- **The /services silent redirect is a real audit finding** (audit Gate 1 fail). Susan probably knows about it. Worth mentioning so the upgrade email doesn't surprise her when it shows up in the new template.
- **2FA note** is important — Susan said on the kickoff "I need to, like, lock it down." If she hasn't, the upgrade could be interrupted.
- **The H1 hierarchy fix is mentioned** because the audit called it a HIGH fail. Susan may notice when the new template goes live.
- **Phase 1 timeline re-confirmed** — important because the original 8/11-8/14 target was revised to ~8/22. Susan should know we're still on track.
- **Lauren's Discovery session + HIPAA notice** — already delivered (per Frank's 7/15-7/18 plan). Not mentioned in this email because it's separate from the upgrade.
- **"Powered by Squarespace" badge** — current site has it in footer. Will carry over post-upgrade. Can be hidden via Custom CSS if Susan wants. Not mentioned in email (low-priority; can handle in QA).
- **No passwords in this email** — Susan's admin password stays in Frank's 1Password.

## Sources

- [[upgrade-checklist-7.0-to-7.1]] — the technical checklist for 8/3
- [[https://support.squarespace.com/hc/en-us/articles/360038270572-Moving-from-Squarespace-version-7-0-to-version-7-1]] — Squarespace support article (the one you shared)
- [[Work/WFC/studio/squarespace-development-reference]] — 7.1 + Fluid Engine + developer-mode rules
- [[docs/audit-current-site]] — 6-gate audit (the /services + H1 + WCAG findings)
- [[docs/audit-template-shortlist]] — Clove as the chosen 7.1 template
- [[docs/kickoff-notes]] — kickoff context (Japan trip, daughter, 2FA, loss context)

---

*Drafted by Mavis 2026-07-20 18:50 PT. Frank: review, customize, send 7/21 (Tue).*
