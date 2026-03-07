# PROJECT.md — RM Advisory Site & GTM Project

## What This Is

This is the RM Advisory website and go-to-market project for Rodrigo Medgenberg — a fractional commercial leadership and board advisory practice targeting fintech, capital markets, and PE-backed B2B SaaS companies.

**Live site:** https://rm-advisory.vercel.app
**Repo:** GitHub `RM-Advisory`, `main` branch
**Deployment:** Vercel auto-deploys on push to `main`

---

## Project Structure

```
RM-Advisory/
├── index.html          # The entire site — single-file HTML
├── vercel.json         # Vercel routing config
├── README.md           # Project overview, ICP, deliverables, version history
└── CLAUDE.md           # This file — working instructions
```

The site is a **single self-contained HTML file**. All CSS is inline in `<style>` tags. All JS is inline in `<script>` tags. No external dependencies except Google Fonts (Fraunces, Inter, DM Mono).

---

## Design System — Do Not Change

These design decisions were made deliberately over multiple iterations. Do not alter without explicit instruction from Rodrigo.

### Palette
```
Dark sections (hero, nav, credential bar, CTA band, footer):
  --dark-bg: #0b0b0b
  --dark-text: #f2efe9
  --dark-text-secondary: #b0ada8
  --dark-text-muted: #7d7a75

Light sections (body):
  --light-bg: #faf8f5
  --light-text: #2c2a26
  --light-text-secondary: #575248
  --light-text-muted: #847e75

Accent: --accent: #c9a06c (copper/bronze)
```

### Typography
```
Display: 'Fraunces', Georgia, serif  (headlines, credential numbers)
Body: 'Inter', -apple-system, sans-serif  (paragraphs, descriptions)
Mono: 'DM Mono', monospace  (labels, tags, nav, metadata)
```

### Components
```
border-radius: 14px (cards, grids)
box-shadow: 0 18px 55px rgba(0,0,0,0.12)
buttons: border-radius: 999px (pill shape)
form fields: border-radius: 12px
```

### Tone
- **Premium, editorial, operator** — not startup, not SaaS marketing
- Think private wealth office meets fintech, not Y Combinator landing page
- The copper accent was chosen deliberately to signal "established" not "trendy"

---

## Content Rules

### Brand Voice
- First person ("I build...") — this is a personal operator brand, not a company
- Direct, confident, no hedging
- Operator language: "in the deals, in the CRM, in the room"
- Never lead with AI — AI is a supporting detail, not the headline
- Signal company-level thinking (P&L, cost discipline, margin) not just revenue function

### Anonymisation Rules
- **EXANTE** → "a global multi-asset brokerage" or "global multi-asset brokerage serving institutional traders and asset managers"
- **Escher Group** → "a PE-backed global software leader"
- **Deutsche Börse** → "Tier-1 Exchange" or "one of Europe's largest financial market infrastructure providers"
- **Digital Asset** → "a distributed ledger technology company" or "blockchain infrastructure"
- **Opensee** → "a Big Data platform serving financial services"
- **Reuters** is OK to name (it's a well-known brand, no NDA concerns)
- **Salesforce** is OK to name
- **CBOE** and **EUREX** are OK to name

### Key Metrics (verified by Rodrigo)
- 20+ years in commercial leadership
- $Bn+ AUM under commercial oversight (Exante — keep vague, no exact figure)
- 200+ revenue professionals led (70 AEs at Salesforce + 190 RMs co-led at Exante)
- 5 regions sold across (Middle East, US, UK & Ireland, DACH, EU, Asia, LATAM)
- Full P&L ownership across two companies
- 67% YoY revenue growth (Opensee)
- 25% YoY growth at Salesforce UK & Ireland
- +30% revenue at Escher

---

## External Integrations

### Calendly
- URL: https://calendly.com/rm-advisory/30min
- Linked from: nav CTA, hero button, CTA band button, contact section "Book directly"
- All open in `target="_blank"`

### Formspree
- Contact form submits to Formspree → rodrigo.medgenberg@gmail.com
- Do not change the form action URL without checking with Rodrigo

### LinkedIn
- Profile: https://www.linkedin.com/in/rmedgenberg/
- Linked from: contact section, footer

### Email
- Current: rodrigo.medgenberg@gmail.com (temporary)
- Future: rodrigo@[custom-domain].com via Google Workspace
- When domain is purchased, update email in: contact section, footer, Formspree config

---

## Site Sections — Quick Reference

| Section | Background | ID | Notes |
|---------|------------|-----|-------|
| Nav | Dark | — | Fixed, Calendly CTA |
| Hero | Dark | — | Fraunces headline, DO NOT change "I build revenue engines" |
| Credential Bar | Dark | — | 5 metrics, $Bn+ AUM |
| Routing | Light | — | Two-panel: cold vs warm visitors |
| Approach | Light | #approach | AI vs Human split |
| Philosophy | Light | — | 3 cards |
| Track Record | Light | #track-record | 4 cards + outcomes grid |
| Services | Light | #services | 3 columns: Audit, Programme, Commercial Leadership |
| CTA Band | Dark | — | Calendly link |
| For Investors | Light | #investors | PE/VC operating partner section |
| About | Light | #about | Career arc + sidebar |
| Contact | Light | #contact | "What happens next" + form |
| Footer | Dark | — | LinkedIn + email |

---

## Common Edit Patterns

### Updating text content
The HTML is minified-ish but readable. Use search to find the section, then edit the text directly. Key landmarks:
- `class="hero"` — hero section
- `class="cred-bar"` — credential metrics
- `id="approach"` — AI vs Human section
- `id="services"` — engagement models
- `id="investors"` — PE/VC section
- `id="about"` — about + sidebar
- `id="contact"` — contact form and details

### Adding a new section
Follow the existing pattern:
```html
<section class="section" id="new-section">
  <div class="container">
    <div class="mono" style="color:var(--light-text-muted);margin-bottom:0.8rem;">Section Label</div>
    <h2>Section Heading</h2>
    <!-- content -->
  </div>
</section>
```

### Responsive breakpoints
- `@media(max-width:1024px)` — tablet (grids collapse to 1 column, services to 2)
- `@media(max-width:768px)` — mobile (everything single column, hamburger nav)

---

## What NOT to Do

1. **Don't change the headline** "I build revenue engines — and the leaders who run them" without explicit approval
2. **Don't lead with AI** — it was deliberately moved to a supporting role after client feedback
3. **Don't change the colour palette** — multiple alternatives were evaluated and rejected
4. **Don't switch fonts** — Fraunces was chosen over Cormorant Garamond after testing
5. **Don't add a framework/build tool** — the single HTML file is intentional for simplicity
6. **Don't use real company names** for Exante, Escher, Digital Asset, or Opensee
7. **Don't remove the "For Investors" section** — it's core to the CEO/board positioning strategy
8. **Don't change Calendly links** without updating ALL four instances

---

## ICP Context (For Content Decisions)

When writing or editing content, keep in mind:

- **Primary buyer:** PE operating partners and board members (top-down, not bottom-up)
- **Primary ICP:** Fintech/brokerage Series B+ scaling sales teams
- **Secondary ICP:** PE-backed B2B SaaS post-investment needing GTM fix
- **Rodrigo's positioning:** Company-level commercial operator, not functional CRO
- **CEO narrative:** The advisory practice is designed to build toward CEO / operating partner roles — every piece of content should signal company-level thinking

---

## Related Documents

These are maintained outside the repo but inform the project:

- **RM-Advisory-Strategy-ICP-Differentiation-Programme.docx** — ICP tiers, competitive analysis vs RevenueOS-style competitors, 90-day programme model design
- **RM-Advisory-LinkedIn-Content-Calendar.docx** — 12-week posting plan, full drafts, audience rotation
- **RM-Advisory-LinkedIn-Profile-Update.docx** — Headline, About, role descriptions, skills overhaul

---

*Last updated: March 2026*
