# Local stack shipping audit: VSC Protocol + CEBA DApp

Date: 2026-10-21  
Scope: internal Local stack only; shared network compatibility, DApp isolation, contribution reliability, KYC fallback, and browser proof. No Amoy or production-pilot scope.

## Evidence inspected

### Coordination repository

- `AGENTS.md`, `GLOSSARY.md`, ADR-0001, repository map, issue-tracker rules, and triage labels.
- `origin/main..main`: `30bcf11`, `9f69004`, `20b3cf1`; no root working-tree changes before this audit.
- Coordination issues `https://github.com/jdelos/ceba-matt/issues/7` and `https://github.com/jdelos/ceba-matt/issues/8`.

### VSC Protocol

- `main` is one commit ahead of `origin/main`: `d510141 deployed new contracts after restart`.
- Working tree has 29 modified files and 8 untracked entries. It includes canonical artifact changes, deployed addresses, and Ignition journal data.
- Existing Phase 1 fingerprint schema establishes useful fields for chain ID, addresses, bytecode artifact hashes, timestamp, and safe local defaults.
- Current deployment output and Ignition journal encode restart-specific chain state. They cannot become shared source truth without approved artifact policy.
- Protocol instructions require cross-repository compatibility evidence and prohibit scope expansion beyond Phase 1 boundaries.

### CEBA DApp

- Active branch: `feat/prisma-pnpm-update`, at pushed commit `7b2d9f5 Upgraded to prisma 7`.
- Working tree has 17 modified files plus untracked tooling, skills, and `tests/localVscRpc.test.ts`.
- Existing launcher copies deployment addresses from Protocol into DApp `.env` and writes fixed RPC variables.
- Uncommitted changes force `VSC_PROTOCOL_CLIENT_RPC_URL=https://ceba.home.lacalcotada.com`; this conflicts with approved loopback-default policy and overwrites developer-selected client RPC.
- DApp already has local configuration tests, contribution recovery browser coverage, real Local purchase browser coverage, DIDit/KYC tests, and contribution-state seams.
- Simulated KYC remains supported when DIDit credentials are absent; DIDit sandbox requires credentials and public callback reachability.

## Findings

### F1 — no shared-stack compatibility contract

Protocol has artifact exports, deployment output, and an isolated-validation fingerprint, but no approved current shared-stack status contract that DApp can consume read-only. DApp therefore cannot deterministically reject missing, stale, mismatched, or bytecode-incompatible shared deployments.

**Required outcome:** Protocol publishes read-only compatibility data with deployment ID or timestamp/fingerprint, chain ID, loopback RPC URL, contract addresses, ABI/bytecode hashes, and artifact identity. DApp validates it before contribution behavior. Owner PID remains excluded unless Protocol also owns process lifecycle on same host.

### F2 — restart-specific artifacts currently look committable

Protocol dirty state contains deployed addresses and Ignition journal records from a restart. These values are not reproducible canonical ABI/build artifacts and leak mutable operational state into source control.

**Required outcome:** canonical `main` policy permits reproducible ABI/build artifacts only. Local addresses and Ignition journals stay runtime state. Compatibility publication must not require redeploying or resetting shared network.

### F3 — client RPC policy violates approved Local default

DApp dirty state changes `.env.example` and deployment sync to force tunnel URL as client RPC. This makes remote tunnel default and overwrites selected values.

**Required outcome:** loopback remains default. Tunnel is explicit opt-in. Address synchronization updates deployment-derived fields only and preserves a developer-selected client RPC.

### F4 — worktree runtime surfaces need isolation

Current Local configuration assumes shared default SQLite path, Astro port, and browser storage. Concurrent DApp worktrees can collide even when network is correctly shared.

**Required outcome:** each DApp worktree derives unique database path, Astro port, and browser-storage namespace. Shared chain and contract addresses remain read-only common data. DApp commands never stop, reset, redeploy, or kill shared network.

### F5 — proof must cover recovery and compatibility, not only happy path

Existing browser tests cover real Local purchase and contribution recovery, but acceptance must prove approved Local stack behavior as a whole.

**Required outcome:** automated browser evidence covers successful contribution, reverted-transaction recovery, amount-mode switching, RPC failure, and shared Local-stack compatibility. One compatibility check runs against current shared stack. Normal tests append unique participants and contribution IDs; destructive lifecycle coverage uses isolated node.

## Issue selection

- `https://github.com/jdelos/ceba-matt/issues/7` only governs issue-form linkage. It is not parent for shipping Local stack behavior.
- `https://github.com/jdelos/ceba-matt/issues/8` restores investment UI while preserving prior protocol configuration. It explicitly excludes Protocol and network changes. It is not parent for this scope.
- New coordination issue required under ADR-0001 and issue-tracker rules.

## Compatibility contract acceptance criteria

- Protocol compatibility data identifies deployment identity, chain ID, loopback RPC, contract addresses, ABI/bytecode hashes, and fingerprint or timestamp.
- DApp accepts only complete, current, bytecode-compatible data for expected Local chain; otherwise blocks contribution before wallet/payment action.
- Canonical artifacts are reproducible ABI/build outputs. Restart-specific addresses and Ignition journals are excluded.
- DApp worktrees isolate SQLite, Astro port, and browser storage without controlling shared network lifecycle.
- Loopback RPC is default; tunnel use requires explicit developer opt-in and address sync does not overwrite it.

## Limits

This audit does not run deployment, browser, build, typecheck, contract, or KYC-provider checks. It does not approve real deposits, production deployment, Amoy, legal/compliance behavior, or any dirty source-repository change.

## Next step

Coordination spec published: https://github.com/jdelos/ceba-matt/issues/10.

Next: propose Protocol, DApp implementation, and DApp browser-proof tracer-bullet tickets with explicit blocking edges.
