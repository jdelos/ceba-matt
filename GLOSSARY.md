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
| Purchase workflow | One user purchase instance whose state coordinates quote, eligibility, wallet, transaction intake, and authoritative settlement. |
| Workflow state | The explicit user-visible stage and allowed recovery actions for one purchase workflow. |
| Authoritative status | Status accepted from the backend or chain source of truth, not inferred from a wallet callback or local UI state. |
| Requoting | Visible replacement of an expired or invalid quote before payment; unsafe actions remain disabled until a valid quote exists. |
| Unresolved outcome | A submitted transaction whose final chain or backend result is not yet known; it is not safe to resubmit automatically. |

Add or revise terms when a decision needs stable shared language. Record hard-to-reverse choices in `docs/adr/`.
