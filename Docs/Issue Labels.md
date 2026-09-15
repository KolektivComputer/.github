# Issue labels

Org-wide label prefixes for KolektivComputer repositories. Projects may add their own labels. Keep these prefixes consistent.

## Prefixes

| Prefix | Meaning | Examples |
| --- | --- | --- |
| `c/` | **Category** — what kind of work | `c/bug`, `c/feature`, `c/enhancement`, `c/chore`, `c/epic` |
| `t/` | **Target** — where it lands | `t/android`, `t/ios`, `t/desktop`, `t/web`, `t/server`, `t/repo`, `t/cloudflare` |
| `i/` | **Integration** — external system | `i/discord`, `i/gcal`, `i/microsoft`, `i/oauth` (project-specific as needed) |
| `a/` | **Attention** — triage status or disposition | `a/blocked`, `a/needs-design`, `a/wontfix`, `a/invalid`, `a/duplicate` |

## How to use

### Category
- Give every issue a `c/` label.
- **`c/feature` always pairs with `c/enhancement`** (a feature is an enhancement). Do not strip either.
- A feature epic may use `c/feature` + `c/enhancement` + `c/epic` together.
- A large bug may use `c/bug` + `c/epic`.
- Otherwise prefer a single `c/` unless a project says otherwise.

### Target, integration, attention
- Add `t/` when the change is platform-specific.
- `t/repo`: repo metadata — workflows, license, README, other repo docs.
- `t/cloudflare`: Cloudflare Workers / Pages / related edge deploy (create on repos that have them).
- Add `i/` when the work is about a named integration.
- `a/blocked`: work cannot proceed (link the blocker in GitHub relationships). `a/needs-design`: product or UX must decide before build.
- `a/wontfix`, `a/invalid`, or `a/duplicate`: close-as-not-planned, then close the issue (usually as not planned). Do not leave those open.

### Types and priority
- Use GitHub’s built-in issue types (Bug / Feature / Task), priority, and estimate — not `p/` or `size/` labels.
- Questions go in Discussions. Do not use a `question` or `c/question` label on issues.

Project-specific labels are fine. Prefer extending `i/` or `t/` over inventing a new prefix without updating this doc.
