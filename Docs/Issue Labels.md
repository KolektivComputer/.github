# Issue labels

Org-wide label prefixes for KolektivComputer repositories. Projects may add their own labels. Keep these prefixes consistent.

## Prefixes

| Prefix | Meaning | Examples |
| --- | --- | --- |
| `c/` | **Category** — what kind of work | `c/bug`, `c/feature`, `c/enhancement`, `c/chore`, `c/epic` |
| `t/` | **Target** — where it lands | `t/android`, `t/ios`, `t/desktop`, `t/web`, `t/server`, `t/docs`, `t/repo`, `t/cloudflare` |
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
- Add `t/` when the change is platform-specific or lands in a named place.
- `t/docs` is the docs tree and the words that ship with the repo: `docs/`, README, changelog, `llms.txt`. It is a target, not a kind of work. Do not add `c/docs`.
  - a docs bug is `c/bug` + `t/docs`
  - a docs feature is `c/feature` + `c/enhancement` + `t/docs`
  - a docs chore is `c/chore` + `t/docs`
- `t/repo` is repo metadata that is not that tree: workflows, license, issue templates, `CODEOWNERS`, community files. README is `t/docs`, not `t/repo`. Use both only when one change touches both.
- `t/cloudflare`: Cloudflare Workers / Pages / related edge deploy (create on repos that have them).
- Add `i/` when the work is about a named integration.
- `a/blocked`: work cannot proceed (link the blocker in GitHub relationships). `a/needs-design`: product or UX must decide before build.
- `a/wontfix`, `a/invalid`, or `a/duplicate`: close-as-not-planned, then close the issue (usually as not planned). Do not leave those open.

### Types and priority
- Use GitHub’s built-in issue types (Bug / Feature / Task), priority, and estimate — not `p/` or `size/` labels.
- Questions go in Discussions. Do not use a `question` or `c/question` label on issues.

## Keel-only targets

In addition to the org core `t/` set (except `t/ios` / `t/desktop` / `t/android` — not used on Keel):

| Examples |
| --- |
| `t/svelte`, `t/react`, `t/vue`, `t/solid`, `t/preact`, `t/lit`, `t/angular`, `t/vanilla`, `t/ktor`, `t/compose` |

Use `t/ktor` for host and call-site work. Use the framework tags for pack and adapter work. `t/compose`: Compose as a Keel protocol client (seed, visits, realtime). Not HTML packs. Ids match FrameworkPicker where applicable. Other repos stay on the org core `t/` set unless they add their own stack tags.


Project-specific labels are fine. Prefer extending `i/` or `t/` over inventing a new prefix without updating this doc.
