# RM Advisory — Project README

## Overview

RM Advisory is a fractional commercial leadership and board advisory practice founded by **Rodrigo Medgenberg**. The project encompasses a full go-to-market build: website, deployment, content strategy, ICP definition, competitive positioning, and LinkedIn presence — designed to attract PE operating partners, board members, and fintech/capital markets founders.

**Live site:** [rm-advisory.vercel.app](https://rm-advisory.vercel.app)
**Booking:** [calendly.com/rm-advisory/30min](https://calendly.com/rm-advisory/30min)
**GitHub repo:** github.com/rodrigomedgenberg-cloud/RM-Advisory

---

## Founder Profile

- **Background:** CBOE (Chicago) → EUREX (Frankfurt) → Reuters/LSEG → Salesforce (70+ AEs, UK & Ireland) → blockchain infrastructure → Big Data fintech → global multi-asset brokerage (current)
- **Scale:** 200+ revenue professionals led, $Bn+ AUM under commercial oversight, 5 regions
- **P&L:** Full ownership across two companies (PE-backed global software, multi-asset brokerage)
- **Languages:** German (native), Spanish (native), English (fluent)
- **Base:** Dublin, Ireland — working globally (Middle East, US, UK, DACH, EU, Asia, LATAM)

---

## Tech Stack

| Component | Tool | Notes |
|-----------|------|-------|
| Website | Single HTML file | Fraunces + Inter + DM Mono, dark hero → light body |
| Hosting | Vercel (free tier) | Auto-deploys from GitHub main branch |
| Repository | GitHub | `RM-Advisory` repo, `main` branch |
| Forms | Formspree | Contact form submissions → Gmail |
| Booking | Calendly | Free tier, 30-min working session |
| CLI | Claude Code | Direct GitHub push, no manual copy-paste |
| Email | Gmail (temporary) | rodrigo.medgenberg@gmail.com — to be replaced with Google Workspace + custom domain |

---

## Design System

```
Palette:
  --dark-bg: #0b0b0b (hero, nav, footer, CTA band)
  --light-bg: #faf8f5 (body sections)
  --accent: #c9a06c (copper/bronze — buttons, highlights)
  --dark-text: #f2efe9
  --light-text: #2c2a26

Typography:
  Display: Fraunces (serif, decisive/operator tone)
  Body: Inter (clean readability)
  Labels/Mono: DM Mono (systems/operator aesthetic)

Components:
  border-radius: 14px
  box-shadow: 0 18px 55px rgba(0,0,0,0.12)
  buttons: pill-shaped (border-radius: 999px)
  form fields: border-radius: 12px
```

---

## Site Structure

1. **Nav** — fixed, dark, with Calendly CTA
2. **Hero** — dark, Fraunces headline, credential kicker
3. **Credential Bar** — dark, 5 metrics (20+ years, $Bn+ AUM, 200+ professionals, 5 regions, Full P&L)
4. **Routing Section** — light, two-panel ("We haven't met" / "We've already spoken")
5. **Approach** — light, AI vs Human split layout
6. **Philosophy** — light, 3 cards (stages, AI-augmented, skill capacity)
7. **Track Record** — light, 4 cards (Salesforce, Big Data Fintech, Blockchain/Exchange, PE-Backed Software) + outcomes grid
8. **Engagement Models** — light, 3 columns (Audit, Programme, Commercial Leadership)
9. **CTA Band** — dark, Calendly link
10. **For Investors** — light, PE/VC operating partner section (problem + solution layout)
11. **About** — light, narrative arc + sidebar (industries, capabilities, languages, markets)
12. **Contact** — light, "What happens next" 3-step process + form + contact details
13. **Footer** — dark, LinkedIn + email

---

## Engagement Models

| Model | Description | Investment |
|-------|-------------|------------|
| **Revenue System Audit** | AI-powered data analysis + 90-min operator diagnostic | From €750 |
| **Revenue Engine Programme** | 90-day structured build: diagnose → build → coach & transfer | €15K – €40K |
| **Commercial Leadership** | Embedded operator (€6K–€20K/month) or Board advisory (equity + retainer) | Varies |

---

## ICP (Ideal Client Profile)

### Tier 1 — Primary: Fintech & Brokerage (Series B+)
- Multi-asset brokerages, trading platforms, wealth management fintechs
- 15-100 employees, 5-30 sellers, scaling into new regions
- **Buyer:** Board member or PE operating partner (top-down entry)

### Tier 2 — Secondary: PE-Backed B2B SaaS
- 6-18 months post-investment, revenue plan underperforming
- €5M–€30M ARR, PE firm has identified GTM as constraint
- **Buyer:** PE operating partner

### Tier 3 — Tertiary: Capital Markets Infrastructure + Middle East Tech
- Exchanges, data vendors, market infrastructure (high-value, long cycles)
- Middle East companies building GTM for the first time

---

## Competitive Positioning

**vs. programme-based competitors (e.g. RevenueOS-style):**

| Dimension | Competitor | RM Advisory |
|-----------|-----------|-------------|
| Industry | B2B SaaS / enterprise only | Fintech, capital markets, brokerage + SaaS |
| Delivery | Team-based programme | Operator-led (Rodrigo in the room) |
| Entry point | Sells to CROs | Sells to board / PE operating partners |
| Geography | Europe | Middle East, Europe, US, global |
| AI | Advises on AI | Practitioner — runs AI workflows weekly |

**4 Moats:** Fintech depth, operator (not programme), board-level entry, Middle East + multilingual

---

## Deliverables Produced

### Website
- `index.html` — current live version (pushed via Claude Code)
- `vercel.json` — Vercel deployment config

### Strategy Documents
- `RM-Advisory-Strategy-ICP-Differentiation-Programme.docx` — ICP, competitive differentiation, programme model, site change recommendations
- `RM-Advisory-LinkedIn-Content-Calendar.docx` — 12-week content plan, 1x/week, full post drafts
- `RM-Advisory-LinkedIn-Profile-Update.docx` — Headline, About, RM Advisory role, EXANTE update, skills overhaul, featured section

### Historical HTML versions (archived)
- v1: Initial dark version (Cormorant Garamond, neon green accent)
- v2: Light version alternative
- v3: Dark hero + light body (copper accent, Cormorant Garamond)
- v4: Fintech positioning integrated
- v5: Design polish (Fraunces font, rounded corners, pill buttons, accessibility)
- v6: Board Advisor card + Middle East added
- v7: Perplexity improvements (routing section, outcomes bar, "What happens next")
- Current: CEO positioning, P&L signals, For Investors section, 3-column services, programme model

---

## Pending / Next Steps

- [ ] **Domain registration** — buy custom domain (rm-advisory.com or alternative), connect to Vercel
- [ ] **Google Workspace** — set up rodrigo@yourdomain.com, replace Gmail on site
- [ ] **LinkedIn profile update** — implement changes from LinkedIn Profile Update doc
- [ ] **LinkedIn Week 1 post** — "Sales methodologies are dead. The fields aren't." (Tuesday/Wednesday)
- [ ] **Conectd.co registration** — start building board advisory pipeline
- [ ] **Specialist bench** — identify 2-3 freelancers per discipline (RevOps/CRM, AI/automation, enablement, analytics)
- [ ] **Name the methodology** — e.g. "Revenue Operating System" or "Revenue Engine Method" for IP anchoring
- [ ] **For Investors page** — potential standalone page (Phase 2)

---

## Version History

| Date | Change | Trigger |
|------|--------|---------|
| Mar 3 | Initial site build, dark theme | Project start |
| Mar 3 | Dark vs light comparison | Client preference exploration |
| Mar 3 | Dark hero + light body, copper accent | Final design direction |
| Mar 3 | AI-augmented positioning | Client feedback on differentiation |
| Mar 3 | AI toned down, operator-first | Client: "Don't lead with AI" |
| Mar 3 | Fintech positioning integrated | Client: balance fintech + SaaS |
| Mar 5 | Fraunces font, design polish, accessibility | Design refinement |
| Mar 5 | Board Advisor card, Middle East | Service expansion |
| Mar 5 | Routing section, outcomes bar, "What happens next" | Perplexity best practices |
| Mar 5 | Deployed to Vercel | Live at rm-advisory.vercel.app |
| Mar 5 | Calendly integrated | All booking buttons wired |
| Mar 5 | LinkedIn content calendar created | 12-week plan |
| Mar 7 | CEO positioning pivot | ChatGPT CEO readiness assessment |
| Mar 7 | P&L ownership, For Investors section | Board/PE buyer signals |
| Mar 7 | 3-column services, 90-day programme model | ICP + competitive analysis |
| Mar 7 | Credential bar updated ($Bn+ AUM, 200+ professionals) | Exante scale reflected |
| Mar 7 | CBOE + Reuters career arc | About section enriched |
| Mar 7 | LinkedIn profile overhaul guide | Full repositioning |

---

*Built with Claude (Anthropic) + Claude Code. Hosted on Vercel. Managed via GitHub.*
