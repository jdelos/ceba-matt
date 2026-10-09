# Domain docs

This coordination repository uses a multi-context layout.

- `GLOSSARY.md`: shared language for the VSC protocol and CEBA DApp.
- `docs/adr/`: system-wide decisions spanning both repositories.
- `docs/architecture/`: integration contracts, deployment compatibility, and cross-repo maps.
- `/home/juli/Devel/kun-agent-workspace/projects/vsc-protocol/CONTEXT.md` and its `docs/` remain authoritative for protocol-local domain rules.
- `/home/juli/Devel/kun-agent-workspace/projects/ceba-dapp-clean/README.md`, `AGENTS.md`, and source docs remain authoritative for DApp-local behavior.

Before cross-repo work, read this repository's glossary and relevant ADRs, then read both source repositories' steering and domain docs. Use glossary terms in issues, specs, tests, and audit findings. Flag conflicts with existing source-repo ADRs instead of silently overriding them.
