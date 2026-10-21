# Local workspace

This directory holds local source checkouts, feature worktrees, and runtime state. Root repository coordinates work but does not own nested repository content.

## Layout

- `repos/vsc-protocol` — canonical local checkout of `jdelos/vsc-protocol`.
- `repos/ceba-dapp-clean` — canonical local checkout of `jdelos/ceba-dapp-clean`.
- `implementations/<feature>/<worktree>` — disposable feature worktrees.
- `runtime/` — local environment files, databases, logs, and generated state.

## Git ownership

Commit protocol changes inside `workspace/repos/vsc-protocol` or its worktrees. Commit DApp changes inside `workspace/repos/ceba-dapp-clean` or its worktrees. Commit shared audits, ADRs, architecture maps, and coordination documents in repository root.

Never add nested repositories, `.env` files, databases, `node_modules`, build output, or runtime artifacts to root repository.

## Bootstrap

```bash
git clone git@github.com:jdelos/vsc-protocol.git workspace/repos/vsc-protocol
git clone git@github.com:jdelos/ceba-dapp-clean.git workspace/repos/ceba-dapp-clean
```
