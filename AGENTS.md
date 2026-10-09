# Agent skills

## Issue tracker

Cross-repo issues and specs live in GitHub Issues for `jdelos/ceba-matt`; use `gh`. See `docs/agents/issue-tracker.md`.

### Triage labels

Use `needs-triage`, `needs-info`, `ready-for-agent`, `ready-for-human`, and `wontfix`. See `docs/agents/triage-labels.md`.

### Domain docs

Multi-context setup: shared decisions live here; contract and DApp context docs remain in their source repos. See `docs/agents/domain.md`.

## Repositories

- Protocol: `/home/juli/Devel/kun-agent-workspace/projects/vsc-protocol` (`jdelos/vsc-protocol`)
- DApp: `/home/juli/Devel/kun-agent-workspace/projects/ceba-dapp-clean` (`jdelos/ceba-dapp-clean`)

Cross-repo changes need one coordination issue, explicit dependency edges, and compatibility checks in both repositories.

## Audit rule

Before new feature work, audit both repositories and record findings under `docs/audits/`. Treat contract interfaces, deployment artifacts, network configuration, wallet/KYC/payment flows, and user-visible transaction states as one system.
