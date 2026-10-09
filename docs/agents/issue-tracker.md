# Issue tracker: GitHub

Cross-repo issues and specs live in GitHub Issues for `jdelos/ceba-matt`. Use `gh` from this coordination repository.

## Conventions

- Create: `gh issue create --repo jdelos/ceba-matt --title "..." --body "..."`
- Read: `gh issue view <number> --repo jdelos/ceba-matt --json number,title,body,labels,comments`
- List: `gh issue list --repo jdelos/ceba-matt --state open`
- Comment: `gh issue comment <number> --repo jdelos/ceba-matt --body "..."`
- Labels: `gh issue edit <number> --repo jdelos/ceba-matt --add-label "..."`
- Close: `gh issue close <number> --repo jdelos/ceba-matt --comment "..."`

## Cross-repo rule

One coordination issue owns each cross-repo slice. Link implementation issues in `jdelos/vsc-protocol` and `jdelos/ceba-dapp-clean` from its body. Record blocking edges before implementation. Each implementation issue names affected repo, contract/API compatibility checks, and acceptance evidence.

## Pull requests as request surface

PRs as a request surface: no.
