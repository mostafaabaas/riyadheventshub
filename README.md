# Riyadh Events Hub — riyadheventshub.com (static landing site)

The Saudi events & entertainment marketing service of **influUGC**. Built Nov 6, 2026.
**Files only — not deployed.**

## Activation context

Owner activation order, Nov 6, 2026 — second of three domains pulled from the
sale portfolio into the network (after `egy.one`, before `aistore.design`).
Role: **Saudi events & entertainment marketing landing** — event coverage &
content production, influencer invitations & event PR, UGC campaigns for events
and festivals, entertainment brand social campaigns, and brand activations.

- This **cancels the Riyadh-trio bundle-sale plan for this name**.
  `riyadhshowtime.com` and `riyadhfunzone.com` **remain sale stock** — only
  riyadheventshub.com was activated.
- The domain currently sits in the **new Namecheap account** (`influugc`) with a
  $200-era sale designation; pulling it from sale there is queued into the
  new-account registrar session batch (see remaining steps).

## Design direction (owner network rule)

**ALL network satellite sites use the main influUGC identity** — no distinct
per-site design:

- Black background `#000`, neon lime accent `#C8FF00`, dark panels, bold heavy
  typography — the www.influugc.com feel (same `styles.css` design system as
  prinfluencer).
- Brand lockup: `Riyadh Events Hub.` wordmark with the subline "The Saudi events
  & entertainment marketing service of influUGC" (Arabic: «خدمة تسويق الفعاليات
  والترفيه في السعودية من influUGC»).
- Only real company data: est. 2020, Arab League St Agouza (Giza 12651),
  Egypt + Saudi/Gulf. Proof featured first is real: **Riyadh Season and the Saudi
  Tourism Authority are real influUGC clients**, alongside flynas, Saudia,
  realme, Domino's, TikTok Live, Zanussi. No prices, no invented figures, no
  testimonials, no stock imagery (CSS/text only).

## Pages built (3 HTML pages, 2 languages)

| File | What |
|---|---|
| `index.html` | Arabic-first landing (RTL, Saudi-friendly Arabic): hero, client proof strip (Riyadh Season + Saudi Tourism Authority first), **guides section (3 content-first guides — see retrofit note below)**, 5 event services (coverage & content production, influencer invitations & event PR, UGC campaigns, entertainment social campaigns, brand activations), why influUGC (with the in-body editorial link to influugc.com), 4-step process (before / during / after the event + report), 6-question answer-first FAQ, contact/CTA band, network footer. |
| `en.html` | Full English mirror (LTR), same structure, guides and FAQ. |
| `404.html` | Branded not-found page (Arabic). |

Plus: `styles.css`, `favicon.svg` (black + lime RE mark), `sitemap.xml`
(hreflang-annotated), `robots.txt`, `llms.txt`.

## SEO / GEO

- Canonical base `https://riyadheventshub.com/` (the real domain — if the site
  is first deployed to an `onrender.com` URL before the domain attaches, switch
  all canonical/OG/sitemap/robots/llms bases in one pass, same as the ugccompany
  rule in `../DEPLOY.md` §2).
- Title/meta target "Event & Entertainment Marketing" / «تسويق الفعاليات
  والترفيه» + Riyadh / Saudi Arabia in both languages; OpenGraph + Twitter
  cards; hreflang ar/en both ways.
- JSON-LD: `Organization` (with `parentOrganization: influUGC`, postal address,
  areaServed, the four real social profiles), `WebSite`, and `FAQPage` matching
  each page's visible FAQ word for word.

## CTAs (both carry the satellite UTM set)

- Booking → `https://www.influugc.com/book?utm_source=riyadheventshub&utm_medium=satellite&utm_campaign=network`
- WhatsApp (client line) → `https://wa.me/201029979797?utm_source=riyadheventshub&utm_medium=satellite&utm_campaign=network`
- Footer legal line: "Part of the influUGC network" linking to the hub.

## Content-first retrofit (Nov 6, 2026)

Retrofitted to the owner's Nov 6 content-first model (sites lead with useful
tips/guides/information for search engines + AI answers, with influUGC services
and real work woven in), following the aistore guides implementation:

- **Guides section is now section 01** on both homepages (after the proof
  strip, before services); the later sections renumbered 02–05. Header nav and
  the footer gained a Guides column, mirroring aistore.
- **3 guides per homepage (AR + EN), answer-first, zero invented figures:**
  1. `#guide-plan` — how to plan content coverage for a Riyadh event/festival
     (moments map, per-phase deliverables, named roles, pre-agreed approvals).
  2. `#guide-invite` — inviting creators to Saudi events: permits (via the
     organiser; general guidance only, no legal claims), written invitations,
     venue/audience etiquette, hosting logistics.
  3. `#guide-measure` — measuring an event's content results: what to track
     (inventory, platform analytics, engagement quality, audience voice,
     follow-on actions) — no invented benchmark figures.
- Each guide closes with a soft woven-in influUGC line + the standard central
  CTAs (book + WhatsApp, `utm_source=riyadheventshub`). Guide styles added to
  `styles.css` (same block as aistore). `llms.txt` gained a Guides section.
- `sitemap.xml` unchanged — guides are anchor sections on the existing URLs,
  no new pages.

## What remains (not done here)

1. **Pull from sale in the new-account session** — remove riyadheventshub.com's
   $200 sale designation/listings in the new Namecheap account (`influugc`),
   queued with the other registrar-session batch items. (riyadhshowtime.com and
   riyadhfunzone.com stay listed for sale — untouched.)
2. **Deploy** — static folder; any static host or a Render Static Site (free
   tier per the network rule). No server/admin in this build: the brief scoped a
   static landing.
3. **Domain attach** — point `riyadheventshub.com` DNS at the host (same
   checklist pattern as `../DEPLOY.md` §4: apex A + www CNAME from the host's
   screen; no MX changes — mail stays on influugc.com).
4. After go-live: dedicated Google Search Console property + submit
   `sitemap.xml`; verify both pages return 200 and the FAQ renders.

## Deploy status (Nov 6, 2026)

- **Repo**: https://github.com/mostafaabaas/riyadheventshub (private, branch `main`) — source pushed Nov 6, 2026.
- **Hosting**: PENDING-DASHBOARD — the Render Static Site service has **not** been created yet.
  Creating it requires the Render dashboard (no Render API key is available to the
  automation): Render Dashboard → New → Static Site → connect this repo — the repo's
  `render.yaml` blueprint pre-fills the service name (`riyadheventshub`) and publish path (`.`).
  Expected live URL once created: https://riyadheventshub.onrender.com
- **Domain attach**: separate later batch (see "What remains" item 3 above).
