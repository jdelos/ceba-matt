# CEBA DApp design-system generation prompt

Paste completed `INPUTS-REQUIRED.md` plus this prompt into frontend generator.

```text
Design complete, mobile-first design system for CEBA DApp.

## Context

- CEBA is issuer-facing fundraising and participant onboarding surface for Calçotada.
- VSC Protocol is separate infrastructure/developer surface. Do not present VSC as one shared investment token, issuer, or pooled treasury.
- Current product scope is invite-only, eligibility-gated, and may be non-live. Design must support clear `not open`, `invite only`, `pending review`, `unavailable`, and `demo/test` states.
- Never invent financial, legal, regulatory, liquidity, return, buyback, ownership, voting, redemption, exchange-listing, or launch claims.
- Use only facts supplied in approved content and claims ledger.
- When fact is missing, use `[Approved claim needed]`, not invented copy.

## Goal

Create trust-building experience moving visitor through:

Calçotada culture and ambition
→ company and issuer identity
→ current participation status
→ how participation works
→ eligibility and risk disclosure
→ secure invite-only join flow
→ contribution/confirmation evidence and help.

## Brand direction

- Feel: warm Catalan hospitality, grounded craft, credible modern finance, transparent technology.
- Avoid: crypto-casino visuals, neon speculation, artificial urgency, generic banking sterility, fake dashboards, excessive 3D.
- Visual contrast:
  - CEBA: human, food, place, founder, community, issuer story.
  - VSC: restrained technical infrastructure, protocol diagrams, documentation links.
- Use existing approved cultural photography as emotional anchor. Product UI must remain calm, precise, readable.
- Build visual system scaling across English, Catalan, Spanish, Dutch, French, German. Support longer translated strings.

## Primary audiences

1. Invited prospective participant: needs trust, eligibility clarity, risk clarity, next step.
2. Existing participant: needs status, evidence, documents, support, recovery actions.
3. Curious public visitor: needs clear cultural/company story without unapproved offer claims.
4. Developer or technical visitor: needs clear exit path to VSC Protocol documentation, not sales copy.

## Information architecture

### 1. Home

- Cultural hero with one clear current-status banner.
- Explain Calçotada/CEBA in plain language.
- CTA changes by availability:
  - `Request invite`
  - `Continue application`
  - `View current status`
  - `Join unavailable`
- No CTA implying live investment when status unknown.

### 2. Why Calçotada

- Founder/company story.
- Cultural proof and operating context.
- Only approved factual proof points.

### 3. How participation works

- Plain-language sequence:
  `Invite → account → eligibility → identity review → contribution → confirmation → records`
- Show eligibility, payment, settlement, asset/entitlement state as separate steps.
- Explain user expectation at each step and support location.

### 4. Current round/status

- Reusable status module.
- Clearly distinguish:
  - available
  - invite-only
  - waitlist
  - paused
  - not yet open
  - closed
  - test/demo
- Include approved terms, risks, documents, last updated date.
- Never render estimates as guarantees.

### 5. Join flow

- Auth/wallet connection where applicable.
- Eligibility and KYC state.
- Contribution/payment state.
- Confirmation/receipt state.
- Recoverable error states.
- Help path on every blocking state.

### 6. Participant area

- Application or contribution status.
- Documents and receipts.
- Activity history.
- Support and recovery actions.
- Never frame unconfirmed activity as completed.

### 7. Help and documents

- Glossary.
- Risks and limitations.
- Contact/support.
- Controlled document center.
- VSC technical documentation link, visually and verbally separate.

## Design-system deliverables

### Foundations

- Color tokens: warm neutral base, food/culture accent, accessible semantic success/warning/error/info colors.
- Typography: editorial display face plus highly readable UI/body face.
- Spacing, layout grid, radii, borders, shadows, elevation.
- Icon rules and image treatments.
- Motion: short, purposeful, reduced-motion safe.
- Add dark/light mode only if it improves clarity.

### Components

- Header with clear CEBA/VSC boundary.
- Status banner and status badge.
- Primary, secondary, tertiary, destructive, disabled, loading buttons.
- Content cards, evidence cards, document cards, disclosure panels.
- Stepper/progress indicator.
- Form fields, validation, identity states, consent/checklist patterns.
- Transaction/contribution state card:
  `not started`, `action required`, `pending`, `processing`, `confirmed`, `failed`, `expired`, `needs support`.
- Receipt and activity timeline.
- Empty, loading, offline, permission-denied, error states.
- Footer, language selector, help drawer, toast/notification patterns.
- Accessible modal and confirmation dialog.

## Accessibility rules

- Meet WCAG 2.2 AA.
- Do not convey status by color alone.
- Visible keyboard focus.
- Minimum touch targets 44 × 44 px.
- Plain-language headings and actions.
- Error messages explain problem, impact, recovery action.
- Respect `prefers-reduced-motion`.
- Images need meaningful alt text or explicit decorative treatment.
- Never hide risk or eligibility information behind hover-only interaction.

## Content rules

- Tone: warm, direct, calm, specific, non-promotional.
- Write short sentences and concrete actions.
- State uncertainty plainly.
- Separate:
  - confirmed fact
  - process step
  - current status
  - limitation/risk
  - future intention
- Never use `investment`, `return`, `guaranteed`, `liquidity`, `ownership`, `buyback`, `voting`, or `trade` unless exact approved wording exists.
- Do not call VSC a single token. Describe issuer-specific assets only when approved source defines them.
- All numbers, deadlines, terms, legal claims come from approved content model.

## Output format

1. Product principles: 5–7 short rules.
2. Brand architecture diagram: CEBA/Calçotada issuer surface versus VSC Protocol technical surface.
3. Sitemap and primary user journeys.
4. Design tokens in JSON-like table.
5. Component inventory with variants and states.
6. Desktop and mobile wireframes for Home, How it works, Current status, Join, Pending, Failed, Confirmed, Participant area, Help/documents.
7. State matrix for onboarding, KYC, payment/contribution, confirmation.
8. Example non-approved placeholder copy marked `[Approved claim needed]`.
9. Accessibility checklist.
10. Open decisions and content required before production.

Use realistic interface detail. Do not use fabricated metrics, testimonials, legal badges, security certifications, partner logos, token prices, countdowns, charts, or investment claims.
```
