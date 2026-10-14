# Approved CEBA investment UI restoration audit

Date: 2026-10-14
Coordination issue: https://github.com/jdelos/ceba-matt/issues/8
DApp implementation issue: https://github.com/jdelos/ceba-dapp-clean/issues/23

## Cause

`jdelos/ceba-dapp-clean` PR #18 merged the approved investment layout into `fm/ceba-contribute-ux-ship-s9`, not `main`. PR #19 later squash-merged secure Contribution intake into `main`. Its integration branch retained granular commits but had the same final tree as `main`; neither line contained PR #18's UI.

## DApp audit

- Ported PR #18's layout, story, checkout styling, routes, and approved-layout test onto current `main`.
- Resolved overlapping React components by preserving PR #19's accepted-payment maximum, durable browser recovery, cross-tab exclusion, authenticated confirmation, KYC gate, and separate blockchain/app-record/email states.
- Updated position/account displays to consume canonical `paymentAmount` and configured payment decimals rather than obsolete `quote` assumptions.
- Production deposit safety remains unchanged.

## VSC Protocol audit

Canonical protocol checkout inspected at `origin/main` commit `8e4a84b`. This restoration changes no contract source, ABI, deployment artifact, address, chain ID, network configuration, or protocol behavior. No protocol implementation issue needed.

## Required evidence

- DApp protocol typecheck and focused protocol tests.
- Approved investment layout test.
- Production build.
- Prettier check.
- Relevant browser smoke where local environment permits.
- Desktop and mobile screenshots on DApp PR.
