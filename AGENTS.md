# Agent skills

## Issue tracker

Cross-repo issues and specs live in GitHub Issues for `jdelos/ceba-matt`; use `gh`. See `docs/agents/issue-tracker.md`.

### Triage labels

Use `needs-triage`, `needs-info`, `ready-for-agent`, `ready-for-human`, and `wontfix`. See `docs/agents/triage-labels.md`.

### Domain docs

Multi-context setup: shared decisions live here; contract and DApp context docs remain in their source repos. See `docs/agents/domain.md`.

## Repositories

- Protocol root: `workspace/repos/vsc-protocol` (`jdelos/vsc-protocol`)
- DApp root: `workspace/repos/ceba-dapp-clean` (`jdelos/ceba-dapp-clean`)
- Worktrees: `workspace/implementations/<feature>/<worktree>`

Treat these nested repositories as canonical local roots. Do not use repositories outside this workspace. Cross-repo changes need one coordination issue, explicit dependency edges, and compatibility checks in both repositories.

## Audit rule

Before new feature work, audit both repositories and record findings under `docs/audits/`. Treat contract interfaces, deployment artifacts, network configuration, wallet/KYC/payment flows, and user-visible transaction states as one system.
