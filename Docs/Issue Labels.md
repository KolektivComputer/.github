# Issue labels

Org-wide label prefixes for KolektivComputer repositories. Projects may add their own labels; keep these prefixes consistent.

## Prefixes

| Prefix | Meaning | Examples |
| --- | --- | --- |
| `c/` | **Category** — what kind of work | `c/bug`, `c/feature`, `c/enhancement`, `c/chore`, `c/epic` |
| `t/` | **Target** — where it lands | `t/android`, `t/ios`, `t/desktop`, `t/web`, `t/server` |
| `i/` | **Integration** — external system | `i/discord`, `i/gcal`, `i/microsoft`, `i/oauth` (project-specific as needed) |
| `a/` | **Attention** — triage status | `a/blocked`, `a/needs-design` |

## How to use

- Every issue should get exactly one `c/` label.
- Add `t/` when the change is platform-specific.
- Add `i/` when the work is about a named integration.
- Use `a/blocked` when work cannot proceed (link the blocker). Use `a/needs-design` when product/UX must decide before build.

## Suggested (not required org-wide yet)

- `p/p0` … `p/p2` — priority
- `size/S` · `size/M` · `size/L` — rough effort

Project-specific labels are fine; prefer extending `i/` / `t/` over inventing a new prefix without updating this doc.
