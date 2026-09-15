# Issue labels

Org-wide label prefixes for KolektivComputer repositories. Projects may add their own labels. Keep these prefixes consistent.

## Prefixes

| Prefix | Meaning | Examples |
| --- | --- | --- |
| `c/` | **Category** — what kind of work | `c/bug`, `c/feature`, `c/enhancement`, `c/chore`, `c/epic` |
| `t/` | **Target** — where it lands | `t/android`, `t/ios`, `t/desktop`, `t/web`, `t/server` |
| `i/` | **Integration** — external system | `i/discord`, `i/gcal`, `i/microsoft`, `i/oauth` (project-specific as needed) |
| `a/` | **Attention** — triage status or disposition | `a/blocked`, `a/needs-design`, `a/wontfix`, `a/invalid`, `a/duplicate` |

## How to use

- Give every issue exactly one `c/` label.
- Add `t/` when the change is platform-specific.
- Add `i/` when the work is about a named integration.
- Use `a/blocked` when work cannot proceed (link the blocker). Use `a/needs-design` when product or UX must decide before build.
- Use `a/wontfix`, `a/invalid`, or `a/duplicate` for close-as-not-planned outcomes, then close the issue (usually as not planned). Do not leave those open.
- Questions belong in Discussions. Do not use a `question` or `c/question` label on issues.
- Do not add `p/` or `size/` labels. Use GitHub’s built-in priority, estimate, and issue types (Bug / Feature / Task) instead.

Project-specific labels are fine. Prefer extending `i/` or `t/` over inventing a new prefix without updating this doc.
