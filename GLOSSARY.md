# Glossary

Shared terms for `vsc-protocol` and `ceba-dapp-clean`.

| Term | Meaning |
| --- | --- |
| VSC Protocol | Smart-contract protocol implemented in `vsc-protocol`. |
| CEBA DApp | User-facing Astro/React application implemented in `ceba-dapp-clean`. |
| Phase 1 | Invite-only €120k escrow baseline currently defined by the protocol repository. |
| Funding Round Manager | Contract coordinating round state, eligibility, contributions, escrow, and refunds. |
| Economic Share Token | Non-voting token issued by the protocol. |
| Participant Eligibility Registry | Contract and application boundary controlling participant eligibility. |
| Deployment artifact | Contract ABI and bytecode/address data consumed by the DApp. |
| Local stack | Hardhat node, deployed VSC contracts, synchronized DApp environment, and Astro app. |
| Cross-repo slice | One user-visible capability requiring coordinated changes in both repositories. |
| Compatibility check | Automated proof that protocol artifacts, addresses, network settings, and DApp calls agree. |
| Transaction state | User-visible lifecycle: wallet request, submitted, confirmed, failed, replaced, or rejected. |

Add or revise terms when a decision needs stable shared language. Record hard-to-reverse choices in `docs/adr/`.
