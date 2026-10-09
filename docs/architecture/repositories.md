# Repository map

## Source repositories

- `jdelos/vsc-protocol`: Solidity contracts, Hardhat tests, Ignition deployments, exported artifacts.
- `jdelos/ceba-dapp-clean`: Astro/React UI, server routes, wallet/KYC/payment integrations, local launcher and compatibility tests.

## Coordination

`jdelos/ceba-matt` owns cross-repo glossary, ADRs, architecture maps, audit reports, and parent issues. Source repos own code and repository-local implementation issues.

## Required cross-repo evidence

1. Protocol build, typecheck, and tests pass.
2. Fresh artifacts export into DApp contract assets.
3. DApp protocol typecheck, tests, artifact validation, and relevant browser flow pass.
4. User-facing transaction states and failure recovery are tested.
