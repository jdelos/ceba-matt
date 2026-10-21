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

One coordination issue owns each cross-repo slice. Create it with the **Cross-repository coordination** issue form. Create one **Cross-repository implementation** issue in each affected source repository.

Use full GitHub issue URLs; bare `#123` references are ambiguous across repositories. Every issue must contain:

- parent coordination URL;
- implementation issue URLs;
- explicit `blocked by` edges, or `None`;
- contract/API and artifact compatibility criteria;
- exact acceptance evidence.

Create the parent first, create child issues with its URL, then replace any `pending` entries in the parent with child URLs. Implementation starts only after this graph is complete. Close the parent only after every child closes and cross-repository evidence is attached.

## Pull requests as request surface

PRs as a request surface: no.
