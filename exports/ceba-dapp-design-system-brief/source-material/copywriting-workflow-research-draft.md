# Research: CEBA + VSC copywriting workflow

**Research date:** 21 October 2026. Environment clock at start: `2026-10-21T19:28:25+02:00`.  
**Scope:** editorial production workflow, not visual redesign, public copy approval, financial advice, or launch authorization.  
**Repository snapshot:** canonical `vsc-protocol` HEAD `d510141c41b836013590f8d0a9c276be97445c6f`; canonical `ceba-dapp-clean` HEAD `7b2d9f5f627c0b49e11d729f0334c4c5ecffe292`. Both working trees already contained changes. Findings describe inspected files, not deployed websites or clean releases.  
**Output:** this report only. No repository edits, commits, issue creation, publishing, or extra agents.

## Summary

Use **founder-led discovery, audience-led structure, and evidence-gated production**. First agree what founder means; then test what readers need; then draft one connected CEBA/VSC journey against controlled facts, terminology, and transaction states. Smallest robust setup: one shared editorial control document, existing Phase 1 content source after integrity repair, and compact page/state briefs beside existing content—not another CMS or bulk AI rewrite.

Keep **CEBA/Calçotada issuer story** distinct from **VSC Protocol infrastructure story**. VSC is not one shared investment token: canonical ADR defines protocol standard and token category, with separate issuer-specific assets. Highest-priority work is reconciling legacy financial promises, resolving terminology and publication authority, and fixing failed content-pack integrity checks before reuse. [L1][L2][L3][L6][L7]

**Recommendations below are proposals, not founder instructions, audience findings, legal conclusions, or approved copy.**

## Research method and evidence boundaries

Four research angles:

1. **Intent and positioning:** founder/cultural archive, issuer/protocol roles, audience needs, value proposition.
2. **Editorial system:** message hierarchy, voice, terminology, page briefs, multilingual consistency, ownership.
3. **High-consequence journeys:** financial claims, approval gates, wallet/KYC/payment states, accessibility.
4. **Production and validation:** human-controlled AI drafting, comprehension testing, release/version discipline.

Read root `AGENTS.md`, research skill, prior storytelling audit, shared domain/glossary, and relevant nested instructions before analysis. Existing root documentation has audit/architecture/ADR areas, not established root research area; authoritative run output path overrides suggested repository destination. Prior audit used only as discovery map; important findings rechecked against canonical sources. [L0][L19]

Dedicated `web_search`, `source_check`, provider loader, and context-fetch tools were unavailable. With supervisor permission, used shell HTTP search and fetched original publisher pages/PDFs; manually inspected publisher, final URL, supporting passage, and retrieval date. Google and DuckDuckGo returned bot challenges; Bing returned irrelevant or broad results for several targeted queries. GOV.UK search API also returned mostly broad matches. Search attempts covered user-needs/interviews, accessibility/financial errors, AI verification, content testing, and editorial voice. **Discovery coverage limited; search snippets supplied no factual evidence.** Official pages and their own navigation supplied usable sources. No private repository content or credentials sent to search services.

Evidence labels:

- **Direct evidence:** inspected source says or implements claim. Local content proves what repository contains—not truth of historical commercial assertions.
- **Interpretation:** comparison or application of inspected sources.
- **Recommendation / researcher inference:** proposed workflow or design choice, requiring owner decision and testing.
- **Unknown:** evidence absent, inaccessible, or unresolved.

Official guidance describes its publisher’s practices. Strategyzer and NN/G describe their own methods; neither proves CEBA conversion gains. No performance uplift, audience preference, market size, legal classification, or launch status inferred from those sources.

## Findings

### 1. Establish brand roles before polishing sentences

**Claim:** VSC Protocol is reusable fundraising infrastructure; Calçotada is first independent issuer. ADR explicitly says VSC identifies protocol standard and token category, not one fungible asset shared across companies. Docs entry identifies CEBA as first issuer’s token ticker and brand. **Sources:** [separation ADR][L2], [domain glossary][L3], [docs entry][L4]. **Support:** direct evidence. **Confidence:** high for documented model; no independent corporate verification.

**Recommendation:** use distinct public narratives linked by factual relationship, not umbrella investment language:

| Name/context | Working editorial rule | Must not imply |
|---|---|---|
| **VSC Protocol** | Infrastructure/standard. Explain responsibilities and integration boundaries. | Company investment, universal VSC coin, shared issuer treasury, pooled economic rights. |
| **Calçotada / company** | Issuer and business story. Use exact legal entity only after owner/counsel verifies spelling and role. | Protocol ownership or other issuers’ obligations. |
| **CEBA** | Issuer-specific ticker/brand per current docs; confirm public naming policy. | Separate legal entity, protocol token, already available asset. |
| **VSC Token** | Domain category for issuer-specific tokens. Explain issuer and rights source whenever relevant. | All VSC Tokens interchangeable; automatic legal entitlement from wallet balance. |
| **EconomicShareToken** | Preserve exact code symbol in developer docs. Map to approved public term rather than rename code through copy. | Different product merely because public wording differs. |
| **VSC DApp / CEBA DApp** | Separate generic platform concept from repository/application label. State whose journey user is entering. | Operator, issuer, and protocol steward are same organization. |
| **Open Venture Foundation / VSC Services BV** | Intended steward/operator structure in ADR. Qualification required until incorporation, governance, and authority verified. | Confirmed incorporation, license, regulated service, or operational readiness. |
| **Founder / participant / holder** | Reserve “founder” for actual founders unless approved community label is clearly explained. Use participant before settlement. | Joining makes someone director, voting shareholder, founding-team member, or token holder immediately. |

Shared root glossary uses “Economic Share Token”; protocol domain says avoid that term in public domain language. Treat as code/domain mapping problem, not permission to silently overwrite either source. Historic “Calçotada Protocol,” CalçotCoin, Romesco/RMSC, and FounderCoin names need explicit legacy mapping. [L3][L9][L10][L19]

### 2. Phase 1 is source-controlled scope, not publication permission

**Claim:** controlling baseline specifies invite-only EUR-denominated €120,000 all-or-nothing Phase 1, one ERC20 Payment Asset, bounded sigmoid pricing, action-point eligibility, escrow, explicit finalization, refunds, deferred token minting, and default-disabled deposits. It expressly gives no real-money launch/deployment/solicitation approval. Exact production asset/provider/network path and several legal/operational questions remain unresolved. **Sources:** [Phase 1 baseline][L1], [known limitations][L5], [contract][L18]. **Support:** direct evidence. **Confidence:** high for baseline, unknown for any external deployment.

**Recommendation:** maintain three separate fields for every relevant statement: **technical scope**, **publication approval**, and **operational availability**. Implemented capability is not approved offer; approved wording is not evidence feature is live. Do not turn numerical demo terms into homepage offer merely because numbers exist in JSON.

### 3. Founder archive contains useful tensions—not settled intent

**Claim:** founder letter emphasizes engineering, markets, IP, scaling, and traditions crossing borders; cultural sections emphasize belonging, shared meals, differences, and community. Personal story presents loneliness and an early gathering; later letter says “This is not nostalgia” and ends “If not, step aside.” **Sources:** [founder letter][L8], [personal story][L11], [food mission][L12], [ambition][L13]. **Support:** direct evidence of authored material. **Confidence:** high for wording, low for present-day founder priority without interview.

**Researcher inference:** strongest discovery question is not “Which slogan sounds best?” It is **how cultural connection, repeatable business systems, and participation fit together—and which leads for each audience**. Archive supports several directions. It does not authorize choosing “community movement,” “food-tech investment,” or “financial democratization” as definitive founder intent.

Preserve concrete vocabulary, lived scenes, names/diacritics, and candid engineering perspective. Reverify biography, patents, customer counts, commercial results, sustainability claims, and quotations separately. Tone editing must not convert “we want to” into “we do,” or remove founder’s ambition to make story generically warm.

### 4. Claims conflicts reach metadata and active route inputs

**Claim:** legacy CEBA sections promise buybacks, guaranteed returns, anytime trading, voting rights, ownership, and scarcity. English translation file also contains “Limited to 5,555 tokens,” €100 participation language, and “First 250 Founders”; localized join route reads `dapp.header.join`. These are not merely dormant long-form articles. **Sources:** [project section][L9], [benefits][L10], [translations][L14], [join route][L15]. **Support:** direct evidence of source strings and route binding; no live rendering checked. **Confidence:** high.

**Recommendation:** claim review must cover page body, titles/descriptions, social previews, navigation, button labels, emails, PDFs, translation files, and failure/success screens. “Not financial advice” footer cannot substitute for correcting unsupported claims. Quarantine legacy claims for review; do not delete historical provenance or imply this report performed a publishing freeze.

### 5. Existing structured source is useful—but currently fails integrity checks

**Claim:** Phase 1 content pack declares controlling locale `en-GB`, supported locales `en-GB`, `nl-NL`, `es-ES`, provenance, record hashes, and demo-only consumption rules. `settled` records still do not authorize production publication. **Sources:** [pack README][L6], [JSON][L7]. **Support:** direct evidence. **Confidence:** high.

**New validation finding:** existing validator failed:

```text
AssertionError [ERR_ASSERTION]: p1.campaign.collaborator-story ack hash mismatch
stored:   sha256:c0b53654bafa3ace0034a88acd5c758c2fd12d415689070ad9d82cc902babb77
computed: sha256:0d88365dbe74a3e2a10cd80a8407e4b9ec4f868b7a901143721265f3f255effd
```

`node --test content/phase1/validate.test.mjs` also failed both tests. Runtime was Node `v24.21.0`; independent Python sorted-key SHA-256 calculation reproduced mismatch. JSON and validator had no working-tree diff from HEAD when checked. Cause not established; no hashes changed. [L7][L22]

**Recommendation:** reuse existing structure only after owner reconciles intended provenance/content and validator passes. Do not “repair” integrity by blindly recalculating hashes. Hash equality would prove internal consistency, not founder acknowledgment, legal sign-off, or commercial truth.

### 6. Needs, tasks, and acceptance criteria make better production spine than topic lists

**Claim:** GOV.UK requires evidence-based user needs, separates need from preselected solution, gives “As a… I need… So that…” structure, and records acceptance criteria and content ownership. Its interview guidance favors open neutral questions, real examples, informed consent, and follow-up clarification. **Sources:** [Identify user needs][E1], [Using in-depth interviews][E2]. **Support:** direct evidence of official method. **Confidence:** high; CEBA adaptation remains recommendation.

**Recommendation:** connect each page to specific decision/task, not “we need an About page.” Founder supplies intent and business constraints; users supply evidence about comprehension, priorities, vocabulary, and objections. Neither replaces other.

### 7. Voice system should preserve identity while changing tone with risk

**Claim:** Mailchimp distinguishes stable voice from situation-dependent tone, prioritizes clarity over entertainment, and warns translators against synonym variation, idioms, and culturally inappropriate informality. **Sources:** [Voice and Tone][E3], [Writing for Translation][E4]. **Support:** direct evidence of first-party editorial policy. **Confidence:** high for policy; not proof its personality fits CEBA.

**Recommendation:** share precision, honesty, and respect across both surfaces; let CEBA carry cultural warmth and founder character, while VSC emphasizes inspectable mechanics and boundaries. Transaction failures should be calm and literal, not onion jokes or promotional enthusiasm.

### 8. Accessibility and source verification are gates, not final polish

**Claim:** WCAG 2.2 includes financial/legal error prevention, accessible authentication, programmatic status messages, and language identification. WAI writing guidance covers descriptive titles, meaningful headings/links, text alternatives, captions/transcripts, clear instructions, and concise language. NIST’s generative-AI profile identifies confabulation and specifically recommends reviewing/verifying generated sources and citations. **Sources:** [WCAG 2.2][E5], [WAI writing guidance][E6], [NIST AI 600-1 §2.2 and MS-2.5-003][E7]. **Support:** direct evidence. **Confidence:** high.

**Recommendation:** no copy release without source-to-sentence review and in-context accessibility checks. AI fluency and readability scores cannot establish truth, accessibility conformance, or understanding.

## Compare approaches: use small pieces, not whole frameworks

| Approach | Useful contribution | Tradeoff / failure mode | CEBA/VSC decision |
|---|---|---|---|
| **Founder narrative first** | Distinctive conviction, lived examples, cultural roots. | Founder recall does not verify facts or establish audience priorities; hero story can overwhelm task. | Use interview and annotated archive to define intent, not final page order. [L8][E2] |
| **GOV.UK content design** | Evidence-backed needs, tasks, acceptance criteria, plain language, maintenance. | Government-service tone alone can flatten cultural/business identity. | Use as production spine; preserve founder voice inside that structure. [E1][E8][E9][E10] |
| **Strategyzer Value Proposition Canvas** | Separates customer jobs/pains/gains from proposed value; asks for evidence of fit. | Large workshop can formalize assumptions without validating them; benefits can become promises. | One compact profile per priority audience; mark assumptions. No need to adopt full commercial system. [E11] |
| **Problem–approach–proof–limits–action narrative** | Connects meaning, mechanism, evidence, and next step. | Not validated universal persuasion formula; conventional urgency conflicts with financial caution. | Researcher-recommended message order; test alternatives, never manufacture stakes or scarcity. |
| **Mailchimp-style voice/terminology rules** | Stable voice with contextual tone; translator-friendly consistency. | Borrowed brand personality becomes imitation; lengthy style guide rarely used. | One-page voice card plus controlled term table. [E3][E4] |
| **Content-focused task testing** | Reveals misunderstandings, jargon, relevance, and action confusion. | Small qualitative samples do not establish conversion uplift or population rates. | Start with moderated tasks and teach-back; postpone A/B tests until traffic and valid endpoint exist. [E12][E13] |
| **AI-first bulk rewrite / SEO-first calendar** | Fast volume and variations. | Scales old claims, invented founder intent, terminology drift, and duplicate pages. | Reject as starting point. Use bounded AI after evidence and brief gates. Google advises people-first content; no ranking guarantee. [E7][E14] |

**Smallest robust combination:** founder interview + needs evidence + one message/terms/claims control document + page/state briefs + one test-and-revise loop. Use existing Markdown/MDX, translation JSON, Git review, and Phase 1 validator. Add tooling only when manual dependency checks become unreliable.

## Recommended workflow: inputs, outputs, owners, gates

Roles below are proposed responsibilities, not existing appointments. One editor can run research and drafting. Founder approves intended meaning; protocol maintainer checks mechanics; issuer-authorized reviewer and qualified counsel decide legal/financial wording and publication route. No editor or AI substitutes for those approvals.

| Stage | Inputs | Small output | Accountable owner; reviewers | Acceptance gate |
|---|---|---|---|---|
| **0. Contain and baseline** | This report; canonical docs/code; current pages, strings, PDFs; source status. | Content inventory marked keep/rework/legacy/block; disputed claims list; exact source revision. | Editorial lead; protocol + issuer owners. | Every high-risk claim mapped to source or blocked. Publication scope explicit. Hash failure assigned for reconciliation; no automatic carry-forward. |
| **1. Extract founder intent** | Cultural/founder archive; recorded interview in founder’s chosen language, with consent. | One-page intent brief; verbatim quote bank; fact/ambition/unknown annotations. | Editorial lead; founder signs meaning and quotation permissions. | Founder can recognize priorities, disagreements, limits, and non-goals. No editorial paraphrase passed off as quote. |
| **2. Understand audience decisions** | Existing research/support/questions/analytics if available; interviews with likely readers. | Prioritized need/task cards; audience vocabulary; evidence strength and unanswered questions. | Research/editorial lead; product owner selects priority. | Each proposed need has observation/source or explicit hypothesis label. Do not use founder’s friends as only proxy for all audiences. |
| **3. Decide positioning and architecture** | Intent brief, needs, issuer/protocol boundaries, proof inventory. | Separate positioning statements; shared role map; message hierarchy; term/voice card. | Founder + product/issuer owner; protocol reviewer. | Explain what each brand is, for whom, why relevant, difference, evidence, limits, next step. No shared-token or voting-right confusion. |
| **4. Brief one connected journey** | Approved message map; actual source routes/states. | Page briefs and state matrix; proposed navigation and cross-links; copy skeleton. | Editorial lead; UX + frontend + support reviewers. | Each page has one primary reader decision and source owner. No orphan CTA, duplicate offer truth, or missing unavailable/error state. |
| **5. Draft and challenge claims** | Approved brief, quote bank, allowed claim IDs, terminology. | Source-language draft with claim references; two useful lead variants at most; unanswered items. | Human editor; founder for intent, domain owner for facts, counsel for high-risk claims. | Every factual/material promise traced; estimates and aspirations labeled; risk context adjacent to relevant action. No blank approval interpreted as consent. |
| **6. Test and localize** | Cleared prototype copy; realistic tasks; frozen source revision; glossary. | Findings and revisions; reviewed locale variants; accessibility/state QA. | Research lead + locale reviewer; domain/counsel re-review changed meaning. | Critical misunderstandings corrected and retested. Each locale preserves rights, conditions, numbers, availability, and recovery meaning. |
| **7. Approve, release, maintain** | Exact reviewed revision; state evidence; locale checks; remaining risk register. | Release record with approvers, scope, versions, owner, review triggers, withdrawal route. | Authorized publisher; named content owner. | Release only inside approved audience/channel/jurisdiction/status. Content approval does not enable deposits. Material source change invalidates affected approvals. |

**First slice:** CEBA home orientation + founder/company explanation + participation-status/help content, paired with concise VSC “what it is / boundaries / developer docs” entry and representative join states. These can begin as text sections, not new routes. Defer exhaustive blog calendar, broad issuer acquisition copy, platform redesign, and speculative future flows.

## Founder discovery: extract intent without inventing it

### Interview method

1. **Prepare annotated archive.** Bring 6–10 short excerpts spanning cultural purpose, engineering/business thesis, personal history, and participation. Mark source/date; do not assemble them into presumed brand position.
2. **Run one focused session, roughly 60–90 minutes.** Planning estimate, not research requirement. Start with concrete origin and recent conversations; then examine priorities, tradeoffs, audiences, evidence, and limits. Record only with consent; retain original language alongside translation. [E2]
3. **Separate five kinds of statements:** remembered event, personal belief, current fact needing proof, future ambition, and explicit promise. Ask for examples and documentary owners, not increasingly flattering adjectives.
4. **Build traceable synthesis.** Each intended message includes exact excerpt/timecode, editor’s interpretation, proposed public meaning, and unresolved point. Preserve conflicting statements until founder resolves them.
5. **Use member-check review.** Founder marks “accurate / not what I mean / no longer current / private.” Then chooses primary idea and unacceptable interpretations. Approval authenticates intent, not market fit or financial truth.

**Recommendation:** ask founder to explain project to one person outside crypto and one protocol developer. Differences expose audience-dependent explanation; they do not prove which audience should lead.

### Founder questionnaire for later interview—not questions requiring answers now

**Purpose and conviction**

1. Which real moment made this work worth pursuing? What happened, who was there, and what changed afterward?
2. What should someone understand after one minute that current website fails to communicate?
3. If readers remember one idea tomorrow, which idea matters most? Which two ideas can wait?
4. Which part is cultural purpose, which part is business thesis, and which part is financing mechanism? How should they relate?

**Authenticity and tension**

5. Does “We feed the bonds that shape our world” still express your intent? What concrete work makes it true—or an ambition?
6. Founder letter emphasizes markets, IP, and scalable systems; personal story emphasizes belonging. Which leads for which reader, and why?
7. What does “not nostalgia” reject? What cultural meaning must remain intact?
8. Which phrases sound unmistakably yours? Which archived phrases now feel wrong, exaggerated, exclusionary, or outdated?
9. Which personal details, names, photographs, and quotations may be public? Which require someone else’s consent?

**Audience and positioning**

10. Whom must each website serve first: customers/hosts, collaborators, invited participants, developers, or future issuers? What decision should each make?
11. Describe last real conversation where someone misunderstood project. What did they think, and how did you explain it?
12. What alternatives do those people use today—including doing nothing? Which distinction can we demonstrate rather than claim?
13. What would make someone correctly decide this is not for them?

**Identity, proof, and boundaries**

14. In your words, what are CEBA, Calçotada, VSC Protocol, and hosted DApp? Which entity makes which commitments?
15. Which results, customer stories, partnerships, qualifications, or IP claims can we document now? Who owns evidence and permissions?
16. Which statements are future hopes? Which promises must website never make?
17. What may visitors do now, in which setting, and who verifies that status before publication?
18. What must people understand about risk, eligibility, escrow, refunds, settlement, and rights before acting?

**Voice, languages, governance**

19. Where should language be warm, bold, technical, or restrained? Where would humor feel disrespectful?
20. Which language best captures your meaning? Which locales need native review rather than literal translation?
21. Who resolves founder/editor/domain/legal disagreements, and who can stop publication?
22. What evidence would show website communicates better: accurate retelling, better questions, correct next actions, fewer support errors, or something else?

## Audience research and positioning

### Start with decision groups—not invented personas

These are **research hypotheses**, not established segments:

| Candidate reader | Decision to investigate | Evidence to seek | Why separate |
|---|---|---|---|
| Culture/customer/collaborator visitor | Understand experience/business and find relevant non-financial next step. | Recent inquiries, customer conversations, partner objections, vocabulary. | May want food/hosting information, not investment explanation. |
| Invited prospective participant | Understand issuer, availability, conditions, downside, and whether to continue. | Questions from actual invitees; read-aloud explanation and document-finding tasks. | Trust and comprehension matter more than promotional excitement. |
| VSC integrator/contributor | Determine scope, interfaces, state semantics, and limitations. | Developer interviews, docs walkthrough, integration questions. | Needs precise mechanics; cultural narrative cannot replace reference. |
| Future issuer/operator | Determine fit and responsibilities. | Explicit discovery interviews only after priority confirmed. | Current Phase 1 does not establish production service for arbitrary issuers. |

Recruit across relevant domain knowledge, language, access needs, and familiarity with founder. Include skeptical/non-converting readers; never present prototype research as investment invitation. A practical starting batch is 4–6 interviews in highest-priority group, then another targeted round if important differences remain. This is resourcing advice, **not** claim that five users establish completeness. Use separate smaller developer walkthroughs rather than mix incompatible tasks in one sample. [E2][E12][E13]

Collect past behavior and recent decisions before showing proposed copy. Avoid “Would you invest?” as proof of demand. Record observation, interpretation, frequency in sample, contradictory cases, and confidence. Existing analytics/support records were not available in this research.

### Positioning worksheet

For each surface:

> For **[specific reader in situation]**, **[brand/entity]** is **[understandable category]** that helps with **[task/outcome]** through **[actual mechanism]**. Unlike **[real alternative]**, its relevant difference is **[substantiated distinction]**. Evidence: **[IDs]**. Not intended for / does not provide: **[limits]**.

Use Strategyzer’s jobs/pains/gains distinction to expose hypotheses, not invent benefits. “Fit is a claim until customers confirm it” is owner’s own caution. [E11]

Separate CEBA’s business value from financing mechanism. Separate VSC’s technical mechanism from issuer investment outcome. “Transparent,” “fair,” “secure,” “sustainable,” and “community-owned” need defined scope and evidence; do not use them as unqualified substitutes for explanation.

## Message hierarchy, IA, and page briefs

### Proposed hierarchy

**Shared spine:** identity and relevance; concrete approach; evidence; current scope and limits; next appropriate action. Pages may change order by task, but must not bury information needed for informed action. GOV.UK recommends frontloading important information; this is guidance, not proof every cultural page needs same layout. [E9]

**CEBA orientation:** cultural/business purpose first, what company is building second, supported proof third, participation relationship and current availability next. Place funding status before funding CTA—not after immersive founder story.

**VSC orientation:** protocol category and intended builder first, role/issuer separation second, supported mechanics third, scope/limitations and docs path next. Do not copy CEBA’s issuer offer into protocol homepage.

**Founder page:** specific scene, resulting conviction, what founder chose to build, what evidence exists, next step. Long-form voice can be personal; financial rights still come from approved issuer documents.

### Minimal page/section map

| Surface | Reader question / page job | Owns | Links onward |
|---|---|---|---|
| CEBA home | What is this, why relevant, what can I do? | Short identity, message summary, status-qualified navigation. | Company/founder; participation information if approved; contact. |
| Company/founder | Why this work, why this team, what evidence? | Founder intent and verified business proof. | Evidence sources; cultural/operational details; current status. |
| Participation/status | Who is issuer, what is available, what conditions apply? | Approved current status, eligibility overview, mechanics, risks, documents. | Exact reviewed terms, help, allowed next action. No automatic join funnel. |
| Join / activity / recovery | What happens now, what has happened, what must I do? | State-specific action and receipt explanation. | Status/help/documents; original transaction evidence. |
| Help/documents | Where can I check meaning or get help? | Controlled glossary, document versions, support route. | Relevant step; issuer/protocol boundary explanation. |
| VSC entry + existing docs | What does protocol do and where do I integrate? | Issuer-neutral overview and limitations; generated reference retains code authority. | Build guides, contracts, known limitations, version/source context. |

Treat as information responsibilities, not mandate for six new pages. Existing CEBA landing is image-led with localized headline; active join route already exists. Existing VSC docs PRD deliberately excludes investor-facing copy and public-hosting decisions. Keep developer docs intact; decide whether separate gateway is needed only after audience research. [L16][L15][L17]

One fact should have one authoritative owner. Home may summarize participation terms; it should link controlled source, not maintain independent financial table. Cross-links must identify surface switch: company story, issuer terms, or protocol docs. Include source and destination in brief, including browser title, description/social preview, headings, link labels, disclosure placement, empty states, and emails triggered by page.

### Compact page brief template

```text
Page/section ID | surface | locale | owner | source revision | status
Reader + situation:
Evidence-backed need (or labeled hypothesis):
Decision/task this page supports:
Single main message:
Supporting messages (max 3) + proof/claim IDs:
Must-understand limits / risks / unavailable features:
Primary action + preconditions + destination:
Secondary help / exit route:
Content order + cross-links + metadata:
Required UI states / accessibility notes:
Success task + critical misunderstanding to prevent:
Founder / domain / legal / locale reviewers:
Review trigger or expiry:
```

## Voice and multilingual consistency

### Proposed one-page voice card

| Principle | CEBA use | VSC use | Boundary |
|---|---|---|---|
| Human, specific | Real meals, places, people, choices. | Explain builder’s next task and consequences. | No invented anecdotes or synthetic testimonials. |
| Ambitious, not inflated | State mission as intention; show grounded progress. | Explain reusable design without claiming universal adoption. | No guaranteed growth, returns, liquidity, or effortless compliance. |
| Precise, not cold | Explain terms without removing conditions. | Preserve exact contract symbols and distinctions. | Never trade legal meaning for brevity. |
| Welcoming, not coercive | Invitation to understand; legitimate choice not to join. | Clear entry points for differing expertise. | No false scarcity or shaming hesitation. |

**Tone by situation:** story = warm and concrete; explanation = calm and direct; review/consent = explicit; pending = factual and patient; failure = non-blaming with recovery; confirmed = specific about what succeeded. “Success!” alone is inadequate when only wallet authorization or app-record update succeeded. [E3][L20]

### Locale plan

**Direct evidence:** DApp locale config lists `en`, `es`, `ca`, `nl`, with English fallback; blog folders also include `de` and `fr`. Phase 1 pack supports `en-GB`, `nl-NL`, `es-ES`; Catalan not declared there. Join component includes hard-coded English alongside localized surrounding route. Directory presence does not prove full translations or approved offer languages. [L6][L14][L15][L20][L21]

**Recommendation:**

1. Keep founder interview in chosen original language. Preserve exact source quotation; label translated quotations and obtain approval for meaning.
2. Respect existing `en-GB` controlling locale for Phase 1 pack unless owner formally changes it. Founder-story source language may differ; identify source per content item, not one assumed language for everything.
3. Translate approved source revision, not independently evolving locale pages. Use stable content and claim IDs; record source hash, translator, reviewer, review date, and stale status.
4. Maintain term table with definition, allowed translation per locale, prohibited variants, code symbol, and context. “Token,” “certificate,” “entitlement,” “escrow,” “refund,” “finalization,” and “founder” need special care.
5. Transcreate cultural warmth/headlines within approved intent; keep financial conditions, numbers, restrictions, and action semantics equivalent. Human locale reviewer plus domain/counsel review where material meaning changes.
6. When material source changes, mark affected translations stale. Do not silently show old financial terms or rely on English fallback as consent. Decide explicit unavailable-language behavior with owner/counsel.
7. Review in context: language attributes, screen-reader labels, line wrapping, amounts/decimals, dates/time zones, links, downloadable documents, and error states. Preserve `Calçotada`, `calçots`, and personal names; explain unfamiliar cultural terms without erasing them.

Mailchimp’s translation guide supports clear syntax and consistent terminology, not literal translation of its brand. W3C language-of-parts criterion includes exceptions for proper names and technical terms; do not incorrectly mark every Catalan name as a new language passage. [E4][E5]

## Claims ledger and approval gates

### Trust hierarchy

Authority depends on claim type:

- **Founder intention:** approved interview/intent brief; not AI interpretation.
- **Contract mechanics:** controlling Phase 1 baseline and relevant contract source; deployed version/state must be checked before operational copy.
- **App behavior:** current implementation plus tested integration, not UI string or README alone.
- **Company/legal/economic rights:** current authorized issuer documents and qualified review; code cannot establish them.
- **Business results:** accountable owner’s records with dates, definitions, permissions, and limitations.
- **Audience needs:** research observations, not founder preference, screenshots, or general internet trends.
- **Availability:** dated operational evidence plus publication authority; neither Git HEAD nor enabled technical flag proves authorization.

### Compact ledger template

```text
Claim ID | exact proposed wording | entity/surface | locale
Type: fact / intention / forecast / comparison / legal-right / state / quote
Source owner + exact passage/record + date + revision
Evidence supports: [scope]; does NOT support: [limits]
Risk/required context | allowed audience/channel/jurisdiction
Status: unverified / substantiated / approved-for-scope / blocked / superseded
Founder meaning approval | domain check | legal/financial review | locale check
Approval evidence + approved revision | expiry/change trigger | all usages
```

**Example entries—review dispositions, not approved copy:**

| ID | Existing/proposed claim | Evidence assessment | Required disposition |
|---|---|---|---|
| C-01 | “VSC is one token for all companies.” | Contradicts issuer-separation ADR. [L2] | Block; use protocol/issuer distinction. |
| C-02 | “We can guarantee these returns.” | Historical CEBA claim, not verified promise; incompatible with current Phase 1 publication boundaries. [L9][L1] | Block reuse; issuer/counsel review source history and any public exposure. |
| C-03 | “Sell your tokens anytime.” | ERC20 transferability does not prove market, buyer, legal recognition, or liquidity. [L10][L5] | Block; resolve transferability/legal contradiction. |
| C-04 | “We have served 10,000 customers.” | Several archive variants say customers/people/happy people; no underlying records checked. [L9][L13] | Verify definition, period, duplicate counting, and evidence owner. |
| C-05 | “Tokens are available after finalization.” | Incomplete: baseline requires **successful** finalization and separate entitlement settlement. [L1][L18] | Rewrite only after state mapping; do not imply automatic delivery. |
| C-06 | “Open-source protocol.” | Documented licensing contradiction remains unresolved. [L1][L5] | Do not publish licensing claim until owner/legal resolution. |
| C-07 | “Your contribution has been confirmed.” | Could mean chain receipt, app record, or email. Working tree tracks these separately. [L20] | Define exact evidence and state; never infer all succeeded. |

### Approval routing

**High-risk gate before public drafting is finalized:** returns/forecasts, ownership/certificates/voting, buybacks/redemption/liquidity, valuation/price/fees, eligibility and geography, scarcity/deadlines, tax, security/audit, privacy/KYC data handling, sustainability, licensing, provider/regulatory status.

Issuer-authorized reviewer and qualified counsel must determine applicable entity, instrument classification, offering/promotion rules, jurisdictions, audience restrictions, and required disclosures. This research **does not determine whether MiCA, securities, crowdfunding, or other regimes apply**. EUR-Lex attempts returned empty HTTP 202 responses; attempted ESMA page returned navigation without target article. No legal proposition relies on those failed fetches. Local Phase 1 document itself requires separate legal/operational approvals. [L1]

**Release gate:** exact source wording/version and translations; named approvers; permitted channels/audiences/countries; dated availability evidence; documents accessible before commitment; no omitted material limitation. Footer disclaimer cannot cure conflicting headline. If disagreement persists, narrow claim or withhold publication. Record decision, not only “legal reviewed.”

**State gate:** runtime data controls state text; legal/content approval controls whether public action is offered. Neither substitutes for other. Real deposits require separate full operational process outside this editorial workflow. [L1][L5]

## Conversion copy and UX states

Goal is **informed, appropriate action**, including choosing not to proceed—not maximum clicks. Match action to real availability: read story/docs, inspect terms, contact support, or continue approved invite journey. Do not invent waitlist, booking, contribution, or download endpoint because button would look useful.

**Direct evidence:** inspected join working tree already separates blockchain, app record, and email status, and provides recovery labeled “no new payment.” It also says “confirm once” although code can request payment approval and contribution confirmations; settlement explanation says “after finalization” without “successful.” These are candidate editorial discrepancies requiring implementation review, not live-bug claims. [L20][L18]

### Minimum state copy matrix

| State / evidence | Copy must establish | Action / forbidden implication |
|---|---|---|
| Demo, unavailable, deposits disabled | Environment, limitation, what can be explored. | No public investment CTA or suggestion disabled gate merely temporary technical inconvenience. |
| Disconnected / wrong network | Required connection/network and why; current environment. | Connect/switch only where supported; never request private keys or seed phrase. |
| Identity not started / pending / rejected / expired / revoked | Distinguish provider verification from action-point eligibility; what happens next. | Approved support/retry route; no invented SLA or sensitive rejection details. |
| Registration submitted / authorization pending | Request is not eligibility approval. | Refresh/wait/help; do not promise every verified identity qualifies. |
| Quote / review | Issuer, amount, Payment Asset, quote vs maximum, fees/gas where applicable, price-change rule, conditions, wallet/network. | Edit or confirm; no EUR/USD equivalence or mock asset real-money implication. |
| Allowance request / allowance confirmed | Spending permission and payment are different steps. | Explain next wallet request; not “investment complete.” |
| Wallet rejected / on-chain reverted | Which step stopped; known fund/fee effects only. | Retry after state check; do not claim “no charge” without evidence, including gas. |
| Submitted / pending / status unknown | Submission not confirmation; original reference and refresh/recovery path. | Do not prompt duplicate payment. Distinguish not known from failed. |
| Replaced transaction | Track replacement/cancellation evidence where implementation supports it. | Never interpret missing original receipt as safe to pay again. |
| Chain confirmed, app record pending/failed | Payment evidence and recording problem separately. | Recover same contribution; no new payment. |
| App record confirmed, email failed | Receipt notification failed, not necessarily contribution. | Retry notification only if available; support otherwise. |
| Contribution accepted into escrow | Conditional entitlement recorded; tokens not yet issued. | No company-ownership or immediate token-delivery celebration. |
| Round paused | New contributions blocked; pause alone does not create refund rights. | Status/help, not unconditional refund promise. |
| Successful finalization / settlement pending | Success transition distinct from per-beneficiary mint settlement. | Claim/settlement path only when supported. |
| Cancelled / deadline failure / refund available | Required state transition and refund process; original contributor destination. | No instant fiat refund promise; separate available, submitted, confirmed states. |

Matrix is **coverage requirement proposal**, not assertion all states/screens exist today. Contract reads should determine canonical chain state; events aid synchronization. Review copy with frontend/protocol owners using mocked state fixtures before production work. [L5][L18]

For financial review screens, GOV.UK “Check answers” pattern offers practical review/edit precedent. WCAG 3.3.4 requires at least one of reversible, checked, or confirmed mechanisms for covered submissions; it does **not** require blockchain reversibility or prove a review screen alone makes whole flow conformant. [E15][E5]

### State template

```text
State ID + trigger/evidence:
What happened / what did NOT happen:
User money, entitlement, identity, and notification status:
Next safe action + precondition:
Recovery/help route + retained reference:
Uncertainty / timing wording (no invented SLA):
Visible text + accessible announcement + locale:
Frontend/protocol reviewer + test fixture:
```

## AI-assisted drafting with human control

**Recommendation:** AI acts as assistant editor, never source owner, founder surrogate, legal reviewer, or simulated audience evidence. NIST explicitly identifies confidently false content and recommends verifying sources/citations in outputs. [E7]

Use AI for:

- Extracting candidate themes with verbatim passage references; human checks extraction.
- Comparing drafts against approved term/claim lists and finding contradictions across pages/locales.
- Producing two bounded lead variations, shortening sentences without removing conditions, and drafting state variants.
- Preparing translation drafts for native/domain review and generating test questions for human refinement.

Do not use AI to invent founder quotes, metrics, customer research, legal approvals, audits, production status, token rights, or “typical” transaction outcomes. Do not let another model’s agreement count as verification.

**Security and privacy:** Do not send KYC records, wallet secrets, identity documents, private commercial data, or confidential legal advice to an AI service without an explicitly approved data-handling basis. Use redacted source packs and minimum necessary excerpts. Consent to an interview does not automatically authorize uploading its recording to an external model.

### Reusable drafting prompt

```text
Task: draft [page/state] for [reader/task], using attached approved brief.
Authority: allowed claim IDs [list], source excerpts [list], terminology [version].
Founder intent: approved summary + permitted quotations [IDs].
Scope: [demo/public/internal], locale [x], current status [verified source].
Do not add facts, promises, numbers, quotes, rights, availability, or urgency.
Preserve conditions, entity distinctions, risk context, and state semantics.
If evidence missing/conflicting, write [NEEDS OWNER: reason]; do not fill gap.
Return: draft; sentence-to-source map; changes in meaning; unresolved questions.
No publication, approval, legal conclusion, or simulated user endorsement.
```

Human editor reviews every material sentence against original source, not model’s source summary. Record model/tool and date when useful for provenance, but retain only necessary redacted inputs. Founder approves voice/meaning; subject owner approves facts; authorized reviewer approves scope. AI draft remains draft after all automated checks pass.

## Accessibility and plain-language gate

Use WCAG 2.2 AA as proposed implementation target, not claim of current compliance. Relevant criteria: 1.1.1 text alternatives; 1.2.2 prerecorded captions; 1.3.1 relationships; 2.4.4 link purpose; 2.4.6 headings/labels; 2.5.3 label in name; 3.1.1 page language; 3.1.2 language of parts; 3.2.4 consistent identification; 3.3.1 error identification; 3.3.2 labels/instructions; 3.3.3 error suggestions; 3.3.4 financial/legal error prevention; 3.3.7 redundant entry; 3.3.8 accessible authentication; 4.1.3 status messages. **Reading Level 3.1.5 is AAA, not AA.** [E5]

Editorial checklist:

- Frontload identity, task, status, and required conditions. Use descriptive headings and explicit link destinations, not repeated “Learn more.”
- Explain specialist terms at first useful occurrence; retain necessary technical precision. Use short active sentences, not arbitrary word-count or grade-level target. GOV.UK explicitly allows specialist terms when explained. [E8]
- Write labels, instructions, validation messages, disabled-state reasons, status announcements, and help together—not placeholder-only fields.
- State error and safe recovery without blaming user. Avoid technical error dumps and false assurances.
- Describe informative images by purpose; use empty alternative for decorative imagery. Supply captions/transcripts for story videos; do not place essential promises/risks only in images or PDFs.
- Review screen-reader order, keyboard flow, accessible names, dynamic announcements, and third-party wallet/KYC transitions in context. Good words cannot repair inaccessible interaction alone.
- Readability tools can flag complexity; human comprehension testing decides whether meaning survived. Do not remove “successful,” “conditional,” or “not guaranteed” to improve score.

WAI recommendations are practical authoring guidance; only full-process implementation evaluation can support conformance claim. [E6][E5]

## Test comprehension, justified trust, and correct action

### Lean test plan

Run one moderated prototype round, revise, then retest critical problems with new participants. Recruit likely readers and distinguish financial/domain experience; include relevant locales and access needs. Let people read in silence; ask neutral follow-ups after they finish. NN/G specifically warns that interrupting reading alters behavior and recommends audience-matched, open-ended content tasks. [E12][E13]

| Test | Example task | Observe | Proposed gate |
|---|---|---|---|
| Identity / positioning | “Explain this to someone who has not seen it.” | Company, protocol, token/category, purpose; unsupported inferences. | No unresolved material issuer/protocol confusion in retest. |
| Relevance | “What would you look for next, given your situation?” | Missing information, vocabulary, wrong surface, irrelevant founder detail. | Priority need can be met without facilitator explaining page. |
| Trust calibration | “Which statements would you check before deciding? Show where.” | Evidence/disclosure finding; reasons for confidence or doubt. | Reader can distinguish aspiration, fact, promise, and unknown—not merely say page looks trustworthy. |
| Participation understanding | “What would happen to a contribution before and after round outcome?” | Escrow, conditional entitlement, success/settlement, refunds, absent guarantees. | Any material false belief triggers revision and retest. |
| Next action | “Show what you would do now, or why you would stop.” | CTA expectation and destination; eligibility/availability; ability to decline. | No unavailable action implied; appropriate stop counts as valid outcome. |
| Recovery | Present pending, rejected, and chain-confirmed/app-pending screens. | Duplicate-payment risk; distinction between payment, record, and email. | No unresolved recovery copy directing unsafe repeat action. |
| Locale/access | Repeat key tasks using relevant language/assistive technology. | Financial-term drift, language fallback, labels/announcements, findability. | No critical equivalent-meaning or access failure left open. |

These are **proposed qualitative release gates**, not measured outcomes or statistical benchmarks. Track actual counts and examples (“3 of 6 confused issuer and protocol”), not unsupported percentages generalized to all users. One observed high-consequence misunderstanding deserves investigation; zero in small sample does not prove universal understanding.

Use short teach-back after reading: “What does this mean in your own words?” Avoid leading quizzes like “You understand returns are not guaranteed, right?” Test message comprehension separately from visual preference. Test navigation labels with realistic finding tasks before commissioning large IA study.

When real traffic, lawful availability, and instrumentation exist, track qualified task completion, correct document access, support themes, recovery success, and inappropriate attempts—not clicks alone. A/B test only reviewed variants with same facts/disclosures and predefined outcome/sample plan. Never A/B test removal of material risk information. No traffic baseline or conversion data inspected here.

**Mobbin:** optional UI context for sequence, disclosure placement, and state coverage. No Mobbin availability/access assumed; no screenshots inspected. Pattern popularity is not evidence copy works, complies, or suits CEBA.

## Ownership, versioning, and maintenance

**Recommendation:** keep one shared editorial control document in coordination layer; canonical domain decisions stay protocol-local, DApp copy stays DApp-local. Cross-repo terminology/state changes later need one coordination issue, explicit dependencies, and compatibility checks in both repositories, as root instructions require. No issue created during this research. [L0][L19]

Minimum content record:

```text
Content ID | canonical owner | source path/revision | claim IDs
Audience/surface | locale + controlling-source revision
Status | exact approval scope + approvers + timestamp
Dependent pages/strings/PDFs/emails | review date + event triggers
Test evidence | release reference | withdrawal/rollback owner
```

- Name one accountable owner per page/claim cluster. Founder need not approve typo fixes; must review altered meaning. Protocol owner reviews mechanics; counsel reviews changed legal/economic promise; locale reviewer checks equivalence.
- Review financial/availability content before every release and immediately on relevant source/state/terms changes. Use quarterly review as initial proposal for evergreen story—not universal interval or substitute for event triggers.
- Source changes should flag dependent page summaries, translations, metadata, email templates, and documents. Small inventory/manual PR checklist sufficient initially; automate stale-reference checks only when needed.
- Keep historical content labeled and separated where retaining it serves legitimate archival purpose; remove misleading current navigation/summaries when authorized. Avoid silently rewriting history or letting archived promises remain current offer evidence.
- Respect generated docs: update NatSpec/source or handwritten guide, not generated reference by hand. [L17]
- For future offer acknowledgments, bind exact approved content version/hash to process only through separately scoped product/legal work. Existing `ackHash` name is not evidence of reader consent or legal signature.
- Maintain change log stating what changed and why. GOV.UK recommends ongoing usefulness/findability checks and updating or retiring outdated content; apply principle without importing its publishing bureaucracy. [E10]

## Limited illustrative message—not approved, not publishable

**Purpose:** show division of message responsibilities. Founder has not approved wording; legal, audience, locale, status, and operational checks remain outstanding. CEBA heading/positioning below are researcher-created interpretations of archive, not founder quotation or verified business outcome. [L8][L12][L13]

> **CEBA / company-story draft**  
> **Food traditions. More reasons to come together.**  
> Calçotada’s story begins with sharing a Catalan meal. Its ambition is to bring cultural food experiences to more people. Start with the founder’s story and what the company is working to build.  
> **Illustrative action:** Read the founder’s story — only if an approved, working destination exists.
>
> **VSC / protocol-entry draft**  
> **Fundraising infrastructure. Separate issuers.**  
> VSC Protocol defines contract mechanics for funding rounds, eligibility checks, escrow, and settlement. Calçotada is its first issuer. VSC is not one investment token shared across companies.  
> **Illustrative action:** Explore protocol scope and limitations.
>
> **Internal prototype context label:** This example describes repository Phase 1 scope. It is not a live offer or authorization to accept funds.

This avoids unverified traction, economics, licensing, production availability, and benefit promises. It deliberately leaves exact CEBA naming and final public-status wording undecided. Final copy should be more specific once founder priorities and evidence permit it.

## Prioritized research topics and why they matter

| Priority | Research topic | Best evidence / owner | Decision enabled |
|---|---|---|---|
| **P0** | Current publication authority, exact issuer/entity names, intended public posture. | Issuer owner; approved documents; qualified counsel; operations. | Prevent false launch/offer/entity claims; decide allowed CTAs and channels. |
| **P0** | Legacy claim exposure and supersession. | Route/string/PDF/email inventory; current deployed content if later authorized. | Determine which historical promises require correction, withdrawal, or archive treatment. |
| **P0** | Content-pack provenance/hash failure. | Protocol/content owner; validator inputs; source history. | Establish reliable reusable source before drafting from pack. |
| **P1** | Founder’s intended cultural/business/financing relationship. | Interview, approved transcript excerpts, archive comparison. | Distinctive message rather than generic food/crypto pitch. |
| **P1** | Priority audience decisions and confusion. | Likely-reader interviews; real support/invite questions. | Choose homepage lead, terminology, page order, and first slice. |
| **P1** | Proof behind strongest differentiators. | Customer/operations records, permissioned stories, IP/qualification evidence. | Replace vague “proven/unique/sustainable” assertions with bounded proof. |
| **P1** | Transaction-state semantics and recovery. | Current code, contract state, integration fixtures, support procedures. | Prevent false completion, duplicate payment, and eligibility confusion. |
| **P1** | Rights/classification/geography/licensing/transferability. | Current issuer instruments and qualified review; canonical unresolved decisions. | Decide permissible rights, risk, provider, and licensing language. |
| **P1** | Locale priorities and terminology. | Actual reader demand; native reviewers; existing source-locale policy. | Avoid six-language volume without equivalent meaning or approval. |
| **P2** | Comprehension and trust calibration. | Moderated task tests and teach-back. | Validate revised messages and critical disclosures before release. |
| **P2** | Navigation/search demand. | Real site/search/support data when available; label testing. | Improve findability, not manufacture blog topics or SEO claims. |
| **P3** | Optional external UI references and later optimization. | Available first-party patterns; Mobbin only if accessible; sufficient traffic later. | Refine context after meaning, facts, states, and approvals work. |

## Contradictions

1. **Issuer/protocol identity:** legacy “Calçotada Protocol” vs current VSC separation; root “CEBA DApp” repository label vs protocol’s generic “VSC DApp” term. Keep mapping explicit. [L2][L3][L19][L23]
2. **Rights and promises:** voting, guaranteed returns, buybacks, easy trading, ownership/urgency claims vs non-voting domain model, deferred payout/liquidity scope, and no launch approval. No migration without resolution. [L1][L3][L5][L9][L10][L14]
3. **Transferability vs legal readiness:** ERC20 transfer behavior retained; canonical research/baseline warns certificate/secondary mechanics unresolved. Copy cannot resolve product/legal contradiction. [L1][L5]
4. **Open-source wording vs licensing intent:** known unresolved contradiction. Avoid licensing recommendation or claim until resolved. [L1][L5]
5. **Founder emphasis/tone:** belonging and invitation vs market/IP-led ambition and exclusionary ending. Not factual contradiction; real editorial tension requiring founder decision. [L8][L11][L12]
6. **Locale policy:** DApp route locales include Catalan; Phase 1 pack does not; blog archive also contains French/German. Separate file presence from supported production language. [L6][L21]
7. **Integrity promise vs check result:** structured source advertises validation/hash guardrails, but current checks fail. [L6][L7][L22]
8. **Join explanation vs mechanics:** “confirm once” and unqualified “after finalization” need reconciliation with allowance/contribution steps and successful-finalization requirement. Working-tree observation, not verified deployment defect. [L20][L18]

External approaches differ by context rather than directly contradict: government task-first style, brand-led voice, and commercial value-proposition methods serve different purposes. No comparative effectiveness study for CEBA/VSC found or claimed.

## Missing evidence and unresolved decisions

- Founder’s current preferred meaning, voice, source language, primary audience, and permissioned quotations.
- Verified company names/roles, corporate records, trademark position, qualified legal conclusions, signed offering/promotion approvals, exact rights documents, and approved public posture.
- Production deployment/availability, actual live-site exposure, current provider agreements, approved Payment Asset, support SLAs, or audit/security approval.
- Business metrics, customer/partner permissions, market-size evidence, IP ownership, environmental substantiation, and current operational roadmap.
- Audience research, search/analytics/support data, conversion baseline, translation completeness, and accessibility results.
- Root cause and authorized correction of content-pack hash mismatch.
- Whether separate VSC public gateway is needed; whether CEBA remains public brand/ticker, umbrella name, or specific participation label.
- Which locales/channels/jurisdictions may publish which content; who owns editorial releases and withdrawal.

Fresh retrieval does not make old local claims current. Historical founder/about material is dated 2025; prior audit dated February 2026. This report’s October 2026 inspection confirms repository contents, not renewed approval or current commercial truth.

## Next steps

1. **Assign editorial lead and decision owners.** Confirm permitted publication scope, issuer naming, priority audience, and who can block release. Keep financial CTAs out of draft assumptions.
2. **Reconcile source integrity and claims first.** Owner investigates `p1.campaign.collaborator-story` provenance/hash mismatch. Editor inventories legacy promises across body, metadata, locale strings, PDFs, and emails. No hash-only “fix.”
3. **Run founder discovery and first audience batch.** Produce signed-off intent brief and evidence-labeled need cards. Use questionnaire above; no further broad web research required before this step.
4. **Create shared message/terms/claims control sheet and first three briefs.** CEBA orientation, participation/status, and VSC entry; include associated join/recovery states. Reuse existing docs/content structure after repair.
5. **Draft, review, test, revise.** Human-led, source-linked drafts; targeted legal/domain checks; comprehension/recovery test; source-frozen translations. Publish only through separately approved release process.

Useful follow-up external research is narrow: qualified jurisdiction-specific review once instrument/entity/channel are settled, and accessibility evaluation of actual wallet/KYC journey. More generic copywriting articles will not resolve founder intent or missing evidence.

## Sources and validation register

All external sources below retrieved **21 October 2026**. Kept external links returned HTTP 200 with substantive content; redirects resolved to final URLs. Publisher passages inspected manually. No dedicated `source_check` registration/tool existed; no automated factual-validation claim made. Some servers required browser-style User-Agent; a later default-agent NIST request returned 403 after successful substantive fetches. Local links use absolute workspace paths because report lives outside repository; they are machine-local and need rebasing if report moves.

### Kept external primary sources

| ID | Source / owner | Inspected support and reason kept | Evidence class / limit |
|---|---|---|---|
| E1 | [Identify user needs — Government Digital Service][E1] | Evidence review; “As a… I need… So that…”; acceptance criteria; ownership records. | Official method, not CEBA user research. |
| E2 | [Using in-depth interviews — GOV.UK Service Manual][E2] | Informed consent, open neutral questions, real examples, follow-ups, secure recordings. Page states published 21 February 2017. | Older but directly relevant first-party method; not effectiveness benchmark. |
| E3 | [Voice and Tone — Mailchimp][E3] | Stable voice, changing tone; clarity over entertainment. | First-party editorial policy; brand-specific personality not copied. |
| E4 | [Writing for Translation — Mailchimp][E4] | Cultural differences, clarity before brevity, active syntax, consistent terms, avoid idioms. | First-party editorial policy, not translation-quality evidence. |
| E5 | [WCAG 2.2 — W3C][E5] | Normative criteria; especially 3.3.4, 3.3.8, 4.1.3 and 3.1.5. Retrieved document identifies W3C Recommendation 12 December 2024. | Standard; no current-site conformance assessment. |
| E6 | [Writing for Web Accessibility — W3C WAI][E6] | Headings, labels, links, alternatives, captions, instructions, clear writing. | Authoring guidance; not substitute for whole-flow testing. |
| E7 | [AI RMF: Generative AI Profile, NIST AI 600-1 — NIST][E7] | §2.2 confabulation; MS-2.5-003 “Review and verify sources and citations”; oversight/data risks. | First-party risk framework; July 2024 publication, not model benchmark or legal compliance finding. |
| E8 | [Use clear language — Government Digital Service][E8] | Plain language for specialists; explain necessary terms on first use. | Official editorial guidance. Secondary statistics on page not reused. |
| E9 | [Create a clear structure — Government Digital Service][E9] | Frontload important information; descriptive headings; structured lists. | Official method, not universal marketing formula. |
| E10 | [Manage existing GOV.UK content — Government Digital Service][E10] | Audit, review metadata, monitor usefulness/findability, update or retire. | Official maintenance guidance; adapt principle, not tooling. |
| E11 | [Value Proposition Canvas — Strategyzer][E11] | Customer jobs/pains/gains; value map; “Fit is a claim until customers confirm it.” | Method owner’s explanation; commercial source, no independent superiority claim. |
| E12 | [Testing Content with Users — Kate Moran, Nielsen Norman Group][E12] | Audience-matched recruitment, content tasks, silence while reading. Metadata: published 7 February 2021; modified 31 October 2024. | First-party practitioner-method publication, not controlled causal study. |
| E13 | [Using moderated usability testing — GOV.UK Service Manual][E13] | Likely users, realistic non-leading tasks, understanding and completion, assistive technology. | Official research method. |
| E14 | [Creating helpful, reliable, people-first content — Google Search Central][E14] | Intended audience/purpose, first-hand expertise, source trust; financial-stability sensitivity. Explicitly says E-E-A-T is not specific ranking factor. | Search owner guidance, not ranking guarantee or reason to write SEO-first. |
| E15 | [Check answers — GOV.UK Design System][E15] | Review and change submitted information; practical confirmation pattern. | Official pattern; no uplift statistic generalized to CEBA. |

### Kept local primary sources

| ID | Source | Why kept |
|---|---|---|
| L0 | [Root instructions][L0], [research skill][L24], [existing audit][L25] | Required scope and prior inventory; audit not current evidence substitute. |
| L1 | [Phase 1 focused-integration baseline][L1] | Controlling scope, economic/state boundaries, unresolved questions, no launch approval. |
| L2 | [Issuer/steward/operator separation ADR][L2] | VSC identity and separate issuer assets/responsibilities. |
| L3 | [Protocol CONTEXT][L3] | Canonical domain vocabulary; older generic scope subordinate to Phase 1. |
| L4 | [Developer docs entry][L4] | Explicit CEBA ticker/brand and issuer relationship. |
| L5 | [Known limitations][L5] | Entitlement, liquidity, transferability, licensing, deployment boundaries. |
| L6–L7 | [Phase 1 pack README][L6], [structured JSON][L7] | Existing provenance, locales, statuses, and hashes; current validation failure disclosed. |
| L8 | [Founder letter][L8] | Founder/business/cultural intent prompts, not independently verified biography. |
| L9–L10 | [CEBA project][L9], [token benefits][L10] | Exact historical financial/promotional claims requiring reconciliation. |
| L11–L13 | [Personal story][L11], [food mission][L12], [ambition][L13] | Cultural purpose, origin scenes, tone/intent tensions, unverified metric variants. |
| L14–L16 | [English translations][L14], [join route][L15], [landing component][L16] | Source strings, metadata, route binding, current content surface. |
| L17 | [Developer documentation PRD][L17] | Developer-only scope, generated-source authority, deferred publication decisions. |
| L18 | [FundingRoundManager.sol][L18] | Contribution/finalization/refund/settlement mechanics; source inspection, not full code/security audit. |
| L19 | [Shared glossary][L19], [shared domain ownership][L26] | Cross-repo terms and authority boundaries. |
| L20 | [Join component working tree][L20] | Wallet requests, chain/app/email separation, recovery, hard-coded strings. Modified relative to HEAD; not deployment evidence. Inspected SHA-256: `987a6d56e6c84c83781d3711a9780643cd2e45fdb5aae1a8d62eb7b1e5648268`. |
| L21 | [DApp locale config][L21], [content collection schema][L27] | Locale/fallback and content structure; directories inspected for language inventory. |
| L22 | [Content validator][L22], [validator tests][L28] | Existing integrity checks; failures independently reproduced. |
| L23 | [Historical About Us][L23] | Old protocol naming and corporate assertions needing current verification. |

### Rejected / deprioritized

- Google/DuckDuckGo search responses: bot challenges; Bing results: irrelevant/broad for several queries. Discovery limitation, not evidence.
- GOV.UK search API results: mostly broad; used original guidance pages/navigation instead.
- [EUR-Lex MiCA HTML](https://eur-lex.europa.eu/eli/reg/2023/1114/oj/eng) and [PDF endpoint](https://eur-lex.europa.eu/legal-content/EN/TXT/PDF/?uri=CELEX:32023R1114): empty HTTP 202 bodies. No statutory claim based on them.
- [Attempted ESMA qualification news URL](https://www.esma.europa.eu/press-news/esma-news/esma-publishes-final-guidelines-qualification-crypto-assets-financial-instruments): HTTP 200 navigation-only response, no target article text. Not substantive evidence.
- Old GOV.UK writing URL: moved through HTML redirect to new writing-guidelines index; cited substantive final pages E8/E9 instead.
- Incorrect WAI `/standards-guidelines/writing/` path: HTTP 404; replaced with verified E6.
- Extra GOV.UK planning/translation guidance: inspected but largely redundant; kept smaller core set.
- SEO listicles, unsourced conversion heuristics, generic token marketing, and unverified commercial promises: not used.
- Mobbin: not accessed; availability unknown. UI references would not establish copy effectiveness.

### Checks performed and limitations

- Read canonical local sources and exact working-tree statuses; no source edits.
- Retrieved kept external sources and inspected supporting passages; checked correct publisher/final destination, not merely HTTP status.
- `node content/phase1/validate.mjs`: **failed**, acknowledgment hash mismatch above.
- `node --test content/phase1/validate.test.mjs`: **failed**, 0 passed / 2 failed, same mismatch.
- Independent Python SHA-256 of validator’s acknowledgment payload: **confirmed mismatch**. Root cause not inferred.
- No full app build, live browser render, user interviews, legal review, accessibility audit, production transaction, or Mobbin test performed. They would exceed research evidence available here.
- Report checks: all 44 source IDs resolve; all 29 local source paths exist; all 15 kept external sources returned substantive HTTP 200 responses on final recheck. Rejected/inaccessible URLs remain labeled, not counted as verified evidence. All three repository indexes had no staged files. HTTP checks establish retrieval, not factual correctness; supporting passages were separately inspected above.

[E1]: https://guidance.publishing.service.gov.uk/writing-to-gov-uk-standards/plan-manage-content/identify-user-needs/
[E2]: https://www.gov.uk/service-manual/user-research/using-in-depth-interviews
[E3]: https://styleguide.mailchimp.com/voice-and-tone/
[E4]: https://styleguide.mailchimp.com/writing-for-translation/
[E5]: https://www.w3.org/TR/WCAG22/
[E6]: https://www.w3.org/WAI/tips/writing/
[E7]: https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf
[E8]: https://guidance.publishing.service.gov.uk/writing-to-gov-uk-standards/writing-guidelines/clear-language/
[E9]: https://guidance.publishing.service.gov.uk/writing-to-gov-uk-standards/writing-guidelines/clear-structure/
[E10]: https://guidance.publishing.service.gov.uk/writing-to-gov-uk-standards/plan-manage-content/manage-existing-govuk-content/
[E11]: https://www.strategyzer.com/library/the-value-proposition-canvas
[E12]: https://www.nngroup.com/articles/testing-content-websites/
[E13]: https://www.gov.uk/service-manual/user-research/using-moderated-usability-testing
[E14]: https://developers.google.com/search/docs/fundamentals/creating-helpful-content
[E15]: https://design-system.service.gov.uk/patterns/check-answers/
[L0]: /home/juli/Devel/ceba-matt/AGENTS.md
[L1]: /home/juli/Devel/ceba-matt/workspace/repos/vsc-protocol/docs/domain/phase-1-focused-integration-baseline.md
[L2]: /home/juli/Devel/ceba-matt/workspace/repos/vsc-protocol/docs/adr/0004-separate-vsc-protocol-stewardship-from-issuers.md
[L3]: /home/juli/Devel/ceba-matt/workspace/repos/vsc-protocol/CONTEXT.md
[L4]: /home/juli/Devel/ceba-matt/workspace/repos/vsc-protocol/apps/docs-site/src/content/docs/index.md
[L5]: /home/juli/Devel/ceba-matt/workspace/repos/vsc-protocol/apps/docs-site/src/content/docs/guides/known-limitations.md
[L6]: /home/juli/Devel/ceba-matt/workspace/repos/vsc-protocol/content/phase1/README.md
[L7]: /home/juli/Devel/ceba-matt/workspace/repos/vsc-protocol/content/phase1/phase1-content.json
[L8]: /home/juli/Devel/ceba-matt/workspace/repos/ceba-dapp-clean/src/content/blog/en/founder-letter.md
[L9]: /home/juli/Devel/ceba-matt/workspace/repos/ceba-dapp-clean/src/content/sections/en/ceba-project.md
[L10]: /home/juli/Devel/ceba-matt/workspace/repos/ceba-dapp-clean/src/content/sections/en/token-benefits.md
[L11]: /home/juli/Devel/ceba-matt/workspace/repos/ceba-dapp-clean/src/content/sections/en/personal-story.md
[L12]: /home/juli/Devel/ceba-matt/workspace/repos/ceba-dapp-clean/src/content/sections/en/about-food.md
[L13]: /home/juli/Devel/ceba-matt/workspace/repos/ceba-dapp-clean/src/content/sections/en/ambition.md
[L14]: /home/juli/Devel/ceba-matt/workspace/repos/ceba-dapp-clean/public/locales/en/translation.json
[L15]: /home/juli/Devel/ceba-matt/workspace/repos/ceba-dapp-clean/src/pages/[lang]/founders/[slug].astro
[L16]: /home/juli/Devel/ceba-matt/workspace/repos/ceba-dapp-clean/src/components/pages/LandingGWG.astro
[L17]: /home/juli/Devel/ceba-matt/workspace/repos/vsc-protocol/docs/prd/developer-documentation.md
[L18]: /home/juli/Devel/ceba-matt/workspace/repos/vsc-protocol/product/protocol/contracts/FundingRoundManager.sol
[L19]: /home/juli/Devel/ceba-matt/GLOSSARY.md
[L20]: /home/juli/Devel/ceba-matt/workspace/repos/ceba-dapp-clean/src/components/react/vsc-protocol-join.tsx
[L21]: /home/juli/Devel/ceba-matt/workspace/repos/ceba-dapp-clean/astro-i18next.config.ts
[L22]: /home/juli/Devel/ceba-matt/workspace/repos/vsc-protocol/content/phase1/validate.mjs
[L23]: /home/juli/Devel/ceba-matt/workspace/repos/ceba-dapp-clean/src/content/blog/en/about-us.mdx
[L24]: /home/juli/Devel/ceba-matt/.agents/skills/research/SKILL.md
[L25]: /home/juli/Devel/ceba-matt/docs/audits/ceba-vsc-documentation-storytelling-audit.md
[L26]: /home/juli/Devel/ceba-matt/docs/agents/domain.md
[L27]: /home/juli/Devel/ceba-matt/workspace/repos/ceba-dapp-clean/src/content.config.ts
[L28]: /home/juli/Devel/ceba-matt/workspace/repos/vsc-protocol/content/phase1/validate.test.mjs
