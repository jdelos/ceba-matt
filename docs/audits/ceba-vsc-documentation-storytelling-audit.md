# CEBA + VSC documentation, storytelling, and website audit

**Date:** 2026-02-13  
**Scope:** canonical local checkouts only: `vsc-protocol` at `d510141`; `ceba-dapp-clean` at `7b2d9f5`. No source code changed.  
**Method:** source, content, route, configuration, and asset inventory. “Gap” and “Mobbin research” are researcher recommendations, not current-product claims. Every factual statement below links primary local evidence.

## Executive summary

VSC already has strong, deliberately technical developer documentation: generated contract reference plus narrow integration and safety guides. Its public product story is intentionally absent, and canonical Phase 1 rules sharply limit any near-term marketing claims. [VSC README](../../workspace/repos/vsc-protocol/README.md) · [docs-site index](../../workspace/repos/vsc-protocol/apps/docs-site/src/content/docs/index.md) · [Phase 1 baseline](../../workspace/repos/vsc-protocol/docs/domain/phase-1-focused-integration-baseline.md)

CEBA DApp has richer cultural, founder, token, video, photo, and multilingual editorial material, plus join/KYC/contribution UI. Present landing route is a full-screen rotating image treatment with one localized title; primary navigation exposes Home, About, and Join, not a coherent explanation of current VSC Phase 1. [CEBA landing](../../workspace/repos/ceba-dapp-clean/src/components/pages/LandingGWG.astro) · [CEBA header](../../workspace/repos/ceba-dapp-clean/src/components/Header.astro) · [CEBA join route](../../workspace/repos/ceba-dapp-clean/src/pages/[lang]/founders/[slug].astro)

**Core recommendation:** retain two separate surfaces. Make VSC docs protocol/developer-first. Make CEBA issuer/onboarding-first, but rebuild claims around approved Phase 1 facts and explicit state/risk disclosure before using historic token-promotion content. [VSC boundary ADR](../../workspace/repos/vsc-protocol/docs/adr/0004-separate-vsc-protocol-stewardship-from-issuers.md) · [VSC limitations](../../workspace/repos/vsc-protocol/apps/docs-site/src/content/docs/guides/known-limitations.md)

## Research angles

1. **Documentation architecture:** authority, audience, generation, navigation, and publishing state.
2. **Website structure:** active routes, IA, conversion path, localization, and operational flow.
3. **Story and asset inventory:** reusable copy, imagery, video, documents, and present narrative.
4. **Claim integrity and reference research:** content conflicts against canonical Phase 1; focused Mobbin browse areas.

## Findings

### 1. VSC documentation structure

1. **Claim:** VSC root documentation separates contract/product code, Astro/Starlight docs, content, durable domain/PRD/ADR docs, and operations records. README calls `docs/domain/phase-1-focused-integration-baseline.md` canonical current scope. **Support:** direct evidence. **Confidence:** high. [VSC README](../../workspace/repos/vsc-protocol/README.md)

2. **Claim:** docs site is Astro Starlight. Sidebar separates **Public developer docs** from **Internal contributor docs**; public navigation includes overview, boundaries, limitations, and four contract-reference pages. **Support:** direct evidence. **Confidence:** high. [Starlight config](../../workspace/repos/vsc-protocol/apps/docs-site/astro.config.mjs)

3. **Claim:** site states target as developer/contributor documentation; it identifies Calçotada as first issuer and CEBA as token ticker/brand, says generated pages derive from source where possible, and disclaims legal/tax/investment/regulatory advice. **Support:** direct evidence. **Confidence:** high. [docs-site index](../../workspace/repos/vsc-protocol/apps/docs-site/src/content/docs/index.md)

4. **Claim:** docs PRD specifies NatSpec plus `@solarity/hardhat-markup` for Solidity reference, TSDoc/TypeDoc for TypeScript reference, and handwritten integration/boundary/safety guides. It explicitly excludes investor-facing education, DApp workflow copy, public hosting, production addresses, and release versioning. **Support:** direct evidence. **Confidence:** high. [Developer documentation PRD](../../workspace/repos/vsc-protocol/docs/prd/developer-documentation.md)

5. **Gap / recommendation:** VSC needs no marketing redesign inside developer docs. Add only a concise issuer-neutral “what VSC is / is not” entry point and clean route from a future product site to developer docs. Keep legal/economic explanations owned by approved issuer materials, not generated ABI docs. **Support:** researcher inference from scope boundaries. **Confidence:** high. [VSC docs overview](../../workspace/repos/vsc-protocol/apps/docs-site/src/content/docs/guides/overview.md) · [Developer documentation PRD](../../workspace/repos/vsc-protocol/docs/prd/developer-documentation.md)

### 2. VSC product-story constraints

1. **Claim:** canonical Phase 1 is invite-only Calçotada Pre-seed: EUR-denominated €120,000 all-or-nothing target, one ERC20 Payment Asset, bounded sigmoid primary pricing, opaque eligibility references, escrow/refunds, multisig-compatible roles, and default-disabled deposit gate. No provider integration or real deployment authorization is included. **Support:** direct evidence. **Confidence:** high. [Phase 1 baseline](../../workspace/repos/vsc-protocol/docs/domain/phase-1-focused-integration-baseline.md)

2. **Claim:** protocol guidance says no real-money approval; exact EUR asset and Polygon deployment remain unresolved; ERC20 possession does not itself provide recognized entitlement, redemption, payout formula, or guaranteed liquidity. **Support:** direct evidence. **Confidence:** high. [Known limitations](../../workspace/repos/vsc-protocol/apps/docs-site/src/content/docs/guides/known-limitations.md)

3. **Claim:** VSC canonical language requires issuer/protocol separation: Calçotada is first independent issuer, while VSC standard does not pool issuers’ assets or rights. **Support:** direct evidence. **Confidence:** high. [Context glossary](../../workspace/repos/vsc-protocol/CONTEXT.md) · [Separation ADR](../../workspace/repos/vsc-protocol/docs/adr/0004-separate-vsc-protocol-stewardship-from-issuers.md)

4. **Gap / recommendation:** before creating VSC public storytelling, decide approved public posture, owner, legal review route, hosting, addresses/version policy, and launch evidence. These were intentionally deferred in VSC docs; none should be implied by polished visual work. **Support:** researcher inference. **Confidence:** high. [Developer documentation PRD](../../workspace/repos/vsc-protocol/docs/prd/developer-documentation.md) · [Phase 1 baseline](../../workspace/repos/vsc-protocol/docs/domain/phase-1-focused-integration-baseline.md)

### 3. CEBA DApp structure and content model

1. **Claim:** README positions CEBA checkout as Astro/React app for generic network-configured VSC Protocol v2 and identifies localized join route `/en/founders/join`; it also documents local protocol deployment, Dynamic wallet auth, KYC, contribution, and confirmation infrastructure. **Support:** direct evidence. **Confidence:** high. [CEBA README](../../workspace/repos/ceba-dapp-clean/README.md)

2. **Claim:** localized home routes render `LandingGWG`; this component displays full-screen image carousel, localized `landing.gwg.title`, and click-to-advance overlay. It contains no active primary CTA in rendered markup. **Support:** direct evidence. **Confidence:** high. [localized index route](../../workspace/repos/ceba-dapp-clean/src/pages/[lang]/index.astro) · [LandingGWG](../../workspace/repos/ceba-dapp-clean/src/components/pages/LandingGWG.astro)

3. **Claim:** header navigation renders localized Home and About links, omits Blog because marked disabled, and provides Join only in mobile controls. Desktop logo link points to `/` rather than computed localized home path. **Support:** direct evidence. **Confidence:** high. [CEBA header](../../workspace/repos/ceba-dapp-clean/src/components/Header.astro)

4. **Claim:** founder join route accepts only `join`, uses DApp wrapper, localized title/description, and presents checkout UI. **Support:** direct evidence. **Confidence:** high. [Founder route](../../workspace/repos/ceba-dapp-clean/src/pages/[lang]/founders/[slug].astro)

5. **Claim:** Astro content collections load localized `sections`, `blog`, and `wgwPages` Markdown/MDX, with schema-managed fields. Blog content exists in `ca`, `de`, `en`, `es`, `fr`, and `nl`; section content exists in `ca`, `en`, `es`, and `nl`. **Support:** direct evidence. **Confidence:** high. [Content collections](../../workspace/repos/ceba-dapp-clean/src/content.config.ts) · [blog tree](../../workspace/repos/ceba-dapp-clean/src/content/blog) · [sections tree](../../workspace/repos/ceba-dapp-clean/src/content/sections)

6. **Gap / recommendation:** current IA has a conversion endpoint but no visible desktop journey connecting culture, company, offer status, eligibility, mechanics, risks, and help. Treat this as information-architecture work before component work. **Support:** researcher inference. **Confidence:** high. [LandingGWG](../../workspace/repos/ceba-dapp-clean/src/components/pages/LandingGWG.astro) · [CEBA header](../../workspace/repos/ceba-dapp-clean/src/components/Header.astro) · [Founder route](../../workspace/repos/ceba-dapp-clean/src/pages/[lang]/founders/[slug].astro)

### 4. Existing CEBA storytelling and visual assets

1. **Claim:** available cultural visual system includes full-screen calçotada carousel photos, founder/person imagery, food/world imagery, badges, uploaded section illustrations, 3D earth textures, 935 CEBA batch WebP files, and multiple hero/background/token videos. **Support:** direct evidence. **Confidence:** high. [image assets](../../workspace/repos/ceba-dapp-clean/src/assets/images) · [public assets](../../workspace/repos/ceba-dapp-clean/public) · [LandingGWG asset use](../../workspace/repos/ceba-dapp-clean/src/components/pages/LandingGWG.astro)

2. **Claim:** CEBA includes long-form founder/company story material and localized blog entries. English “About Us” describes investment/company structure; English founder letter frames founder history and cultural-business ambition. **Support:** direct evidence. **Confidence:** high. [About Us](../../workspace/repos/ceba-dapp-clean/src/content/blog/en/about-us.mdx) · [Founder Letter](../../workspace/repos/ceba-dapp-clean/src/content/blog/en/founder-letter.md)

3. **Claim:** section content includes token narrative, RMSC narrative, FounderCoin membership narrative, and linked Green Paper PDF. **Support:** direct evidence. **Confidence:** high. [tokens section](../../workspace/repos/ceba-dapp-clean/src/content/sections/en/tokens.md) · [RMSC section](../../workspace/repos/ceba-dapp-clean/src/content/sections/en/rmsc-token.md) · [FounderCoin section](../../workspace/repos/ceba-dapp-clean/src/content/sections/en/founder-coin.md) · [public docs](../../workspace/repos/ceba-dapp-clean/public/docs)

4. **Gap / recommendation:** asset volume is not asset system. Establish approved asset taxonomy: cultural/editorial photography; issuer/company proof; product/interface captures; protocol diagrams; and legal/risk disclosure graphics. Add ownership, rights, locale, alt text, focal point, and approved-use status. **Support:** researcher inference. **Confidence:** medium. [image assets](../../workspace/repos/ceba-dapp-clean/src/assets/images) · [public assets](../../workspace/repos/ceba-dapp-clean/public)

### 5. Claim conflicts and publishing risk

1. **Claim:** some current CEBA sections promise fixed returns, buyback commitments, easy token trading, voting rights, “only 250” urgency, and company ownership assertions. **Support:** direct evidence. **Confidence:** high. [CEBA project section](../../workspace/repos/ceba-dapp-clean/src/content/sections/en/ceba-project.md) · [token benefits](../../workspace/repos/ceba-dapp-clean/src/content/sections/en/token-benefits.md) · [FounderCoin section](../../workspace/repos/ceba-dapp-clean/src/content/sections/en/founder-coin.md)

2. **Claim:** canonical VSC Phase 1 excludes product redemption, exit/distribution/repurchase formulas, secondary exchange/liquidity promises, broad access, and production launch authorization. Its documents flag transferability/legal treatment as unresolved. **Support:** direct evidence. **Confidence:** high. [Phase 1 baseline](../../workspace/repos/vsc-protocol/docs/domain/phase-1-focused-integration-baseline.md) · [Known limitations](../../workspace/repos/vsc-protocol/apps/docs-site/src/content/docs/guides/known-limitations.md)

3. **Contradiction:** CEBA historical promotional claims conflict with canonical Phase 1 boundaries. Do not migrate them into current landing, join, email, ads, or Mobbin-inspired screens without owner/legal approval and a current source of truth. **Support:** direct evidence plus researcher comparison. **Confidence:** high. [CEBA project section](../../workspace/repos/ceba-dapp-clean/src/content/sections/en/ceba-project.md) · [token benefits](../../workspace/repos/ceba-dapp-clean/src/content/sections/en/token-benefits.md) · [Phase 1 baseline](../../workspace/repos/vsc-protocol/docs/domain/phase-1-focused-integration-baseline.md)

4. **Claim:** VSC’s structured Phase 1 content pack labels consumption as closed-group demo/settled only and says publication or deposit enablement needs later explicit approval. **Support:** direct evidence. **Confidence:** high. [Phase 1 content README](../../workspace/repos/vsc-protocol/content/phase1/README.md)

### 6. Proposed Mobbin browsing research

Mobbin browsing should collect **interaction patterns, IA, disclosure placement, state transitions, responsive behavior, and accessibility cues**. It must not copy branding, copy, screens, claims, or imply source endorsement. This is researcher recommendation; no external/Mobbin source was used in this audit.

| Surface | Browse areas | Capture question | CEBA/VSC use |
|---|---|---|---|
| **CEBA public issuer site** | Cultural hospitality brands; founder-story landing pages; membership/community programs; premium food/event discovery | How does photo-led hero establish meaning, then reach a clear next action without burying navigation? | Replace carousel-only opening with culture → company → current status → action narrative. |
| **CEBA offer readiness** | Regulated investing, wealth onboarding, crowdfunding, high-consideration purchase flows | How are eligibility, availability, risks, waitlist/invite, and unavailable states stated before commitment? | Build approved invite-only/non-live state; never borrow financial promises. |
| **CEBA account + join** | Wallet/passkey onboarding; identity verification; checkout progress; payment approval; pending/failed/confirmed receipts | What state language, recovery actions, help, and progress indication reduce abandonment and prevent false completion? | Map Dynamic, KYC, approval, contribution, confirmation, and recovery states to current flow. |
| **CEBA holdings/evidence** | Portfolio/activity history; order/transaction detail; verification status; document centers | How do users inspect status, receipt, and next action without mistaking estimates for guarantees? | Future contribution/entitlement evidence model, bounded by protocol facts. |
| **VSC product entry** | API/platform homepages; developer tools; protocol ecosystem maps; open-source project sites | How are protocol, issuer, operator, and developer paths separated on first visit? | A minimal VSC landing or gateway linking docs, without turning technical docs into marketing. |
| **VSC developer docs** | API reference, SDK quickstarts, contract/address explorers, changelogs | How do docs expose network/version/deployment status, safety warnings, test-only labels, and copyable examples? | Improve discoverability around existing integration docs; retain Starlight source-of-truth model. |
| **VSC issuer/operator future** | B2B setup wizards, admin consoles, compliance checklists, multi-step configuration | How are role boundaries, irreversible steps, audit trail, approvals, and disabled gates represented? | Future issuer/operator tooling only; Phase 1 does not authorize production UI. |

## Recommended information architecture

### CEBA: public issuer + invite flow

1. **Home:** cultural hook, issuer identity, one current-status banner, primary CTA matching actual availability.
2. **Why Calçotada / company:** founder and operating story, only substantiated proof points.
3. **How participation works:** plain-language eligibility, invite, identity check, contribution, escrow, outcome; link technical terms to controlled explainers.
4. **Current round:** terms/status only from approved source; no forecast, return, liquidity, buyback, or ownership claim outside approval.
5. **Join:** authentication, eligibility, contribution, confirmation, recoverable failure states.
6. **Help, documents, and contact:** controlled documents, glossary, current risks/limitations, support path.

This is researcher inference. It follows active route limitations and canonical protocol state boundaries. [CEBA header](../../workspace/repos/ceba-dapp-clean/src/components/Header.astro) · [CEBA join route](../../workspace/repos/ceba-dapp-clean/src/pages/[lang]/founders/[slug].astro) · [Phase 1 baseline](../../workspace/repos/vsc-protocol/docs/domain/phase-1-focused-integration-baseline.md)

### VSC: protocol/developer surface

1. **Protocol gateway:** concise role map and “not an issuer/not an offer” statement.
2. **Build / integrate:** existing contract integration path, contract refs, safety limits.
3. **Issuer/operator (later):** clearly separate non-production conceptual material until governance, legal, hosting, and launch decisions exist.
4. **Contributor:** existing internal workflow/reference section; do not expose by default if future public hosting has different access needs.

This is researcher inference. [Starlight config](../../workspace/repos/vsc-protocol/apps/docs-site/astro.config.mjs) · [Developer documentation PRD](../../workspace/repos/vsc-protocol/docs/prd/developer-documentation.md) · [Separation ADR](../../workspace/repos/vsc-protocol/docs/adr/0004-separate-vsc-protocol-stewardship-from-issuers.md)

## Prioritized next work

1. **P0 — content freeze and claim inventory:** classify every current CEBA content record/document as approved, historical, superseded, demo-only, or prohibited for public publication. Resolve conflict with Phase 1 source before design work. [CEBA project section](../../workspace/repos/ceba-dapp-clean/src/content/sections/en/ceba-project.md) · [Phase 1 content README](../../workspace/repos/vsc-protocol/content/phase1/README.md)
2. **P1 — approved content model:** add one owner-approved CEBA source for current round/status/disclosures, wired separately from historical blog and campaign sections. This audit does not prescribe code changes. [Content collections](../../workspace/repos/ceba-dapp-clean/src/content.config.ts) · [Phase 1 baseline](../../workspace/repos/vsc-protocol/docs/domain/phase-1-focused-integration-baseline.md)
3. **P1 — Mobbin synthesis:** collect 5–8 examples per table area; document pattern, screenshot/link, device, behavior, accessibility notes, and explicit adaptation/not-copy rationale.
4. **P1 — CEBA IA prototype:** prototype first with real approved words and all unavailable/pending/error/confirmed states, then visual assets.
5. **P2 — VSC gateway decision:** decide whether VSC needs separate public product gateway before altering current docs site; preserve developer-doc contract as-is meanwhile. [Developer documentation PRD](../../workspace/repos/vsc-protocol/docs/prd/developer-documentation.md)

## Limits

No live site, external website, legal review, CMS preview, visual rendering, image-rights audit, or Mobbin browsing was performed. Local inventory cannot prove deployed routes, public availability, asset rights, translation completeness, analytics, conversion behavior, or claim approval status. Local checkout commits stated above are audit snapshot identifiers, not release attestations.

## Source register

All kept sources primary local repository material.

- **VSC:** [README](../../workspace/repos/vsc-protocol/README.md) — repository map and docs commands.
- **VSC:** [Phase 1 focused integration baseline](../../workspace/repos/vsc-protocol/docs/domain/phase-1-focused-integration-baseline.md) — controlling scope and launch limits.
- **VSC:** [CONTEXT glossary](../../workspace/repos/vsc-protocol/CONTEXT.md) and [separation ADR](../../workspace/repos/vsc-protocol/docs/adr/0004-separate-vsc-protocol-stewardship-from-issuers.md) — identity/role boundaries.
- **VSC:** [Starlight config](../../workspace/repos/vsc-protocol/apps/docs-site/astro.config.mjs), [docs index](../../workspace/repos/vsc-protocol/apps/docs-site/src/content/docs/index.md), [developer-docs PRD](../../workspace/repos/vsc-protocol/docs/prd/developer-documentation.md) — documentation IA and scope.
- **VSC:** [known limitations](../../workspace/repos/vsc-protocol/apps/docs-site/src/content/docs/guides/known-limitations.md) and [Phase 1 content pack](../../workspace/repos/vsc-protocol/content/phase1/README.md) — safety and publication limits.
- **CEBA:** [README](../../workspace/repos/ceba-dapp-clean/README.md), [routes](../../workspace/repos/ceba-dapp-clean/src/pages), [header](../../workspace/repos/ceba-dapp-clean/src/components/Header.astro), [LandingGWG](../../workspace/repos/ceba-dapp-clean/src/components/pages/LandingGWG.astro) — site/flow structure.
- **CEBA:** [content config](../../workspace/repos/ceba-dapp-clean/src/content.config.ts), [sections](../../workspace/repos/ceba-dapp-clean/src/content/sections), [blog](../../workspace/repos/ceba-dapp-clean/src/content/blog), [assets](../../workspace/repos/ceba-dapp-clean/src/assets/images), [public](../../workspace/repos/ceba-dapp-clean/public) — editorial and visual inventory.
- **CEBA:** [CEBA project](../../workspace/repos/ceba-dapp-clean/src/content/sections/en/ceba-project.md), [token benefits](../../workspace/repos/ceba-dapp-clean/src/content/sections/en/token-benefits.md), [FounderCoin](../../workspace/repos/ceba-dapp-clean/src/content/sections/en/founder-coin.md) — historic promotional claims requiring review.
