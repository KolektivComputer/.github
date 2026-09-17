# Contributing to Kolektiv

Thanks for contributing. Kolektiv is the org behind Keel, Kalendee, Wake, and related projects at [kolektiv.computer](https://kolektiv.computer) / [github.com/KolektivComputer](https://github.com/KolektivComputer). This guide is org-wide. Each repository may add a local `CONTRIBUTING.md` or a deep `DEVELOPING.md` for project-specific setup.

## Code of Conduct

Projects follow the Contributor Covenant when a `CODE_OF_CONDUCT.md` is present in the repo or this org `.github`. By participating, you agree to uphold it.

## Ways to contribute

- **Code** — features, bug fixes, tests, build and tooling
- **Documentation** — guides, references, typo fixes
- **Bug reports** — clear reproductions
- **Design feedback** — UI, UX, and naming
- **Translations** — when a project has i18n set up

Prefer the repository’s issue templates when they exist. Otherwise open a plain issue with expected vs actual behavior, steps to reproduce, and which component you hit.

## Security issues

Do not open a public issue for security vulnerabilities. Contact the repository maintainers privately (for example via the contact on the org or repo profile) and give them time to fix and release before public disclosure. Include affected versions, reproduction steps, and impact when you can.

## Getting started

1. Read the target repository’s `README.md`, `AGENTS.md` (if present), and `DEVELOPING.md` (if present).
2. Fork or get access, clone, and create a topic branch: `git switch -c feat/my-thing`.
3. Build and test with the commands in that repo’s developing guide before and after your change.

## Pull requests

- Keep PRs focused. One logical change per PR.
- Link related issues (`Closes #123`, `Relates to #456`).
- Describe how you tested: commands, manual steps, screenshots for UI.
- Draft PRs are welcome for early feedback.
- Use the repo’s PR template when it exists.

## Commit conventions

Use [Conventional Commits](https://www.conventionalcommits.org/):

```
feat(host): pass pack ref into respondPage
fix(docs): correct seed entry pack path
docs: clarify Harbor is a testbench
```

Imperative subject. Details in the body. Reference issues in the body or footer.

## Code style

- Match the file you edit. Do not reformat unrelated code.
- Follow that repository’s language and tooling conventions (`AGENTS.md` / `DEVELOPING.md`).
- Do not commit secrets, local IDE state, or build outputs.

## AI-assisted contributions

AI tools are welcome. Code can be AI-assisted to any degree as long as a human owns the change and can explain it. That is the whole policy. The rules below are what it means in practice.

- Allowed at any level: autocomplete, first drafts, refactors, tests, explanations, and agent-opened pull requests.
- **Agent-opened PRs must say so up front** (title or first line of the description: AI-generated). The description must clearly and concisely cover what changed, why, and the implications for the rest of the codebase or project goals.
- A **named human** stays active in the PR discussion so other maintainers can ask questions. That human must be able to explain every hunk. The burden of understanding sits on them, not on the agent or on reviewers. "The AI wrote it" is not an acceptable answer.
- Disclose which tools helped and what they did. Honest disclosure is never penalized.
- You are responsible for correctness, tests, licensing, and security of what you submit.
- If you use a coding agent, point it at that repository's `AGENTS.md` when one exists.

Humans who open PRs themselves still write the description in their own words. Agent-opened PRs are the exception that may ship an AI-written description, so long as it meets the clarity bar above and a human owns the thread.

## Licensing

Each repository has its own license (for example Apache-2.0 on Keel, AGPL on Kalendee). By opening a pull request you agree that your contribution may be distributed under that repository’s license. Only submit code you can license that way. Do not paste from incompatible or proprietary sources.

By opening a pull request you agree your contribution is offered under that repository's existing LICENSE (inbound equals outbound). There is no org-wide CLA unless a specific repo requires one.

## Community

- Issues and pull requests are the main place to talk.
- Be patient and kind. Reviewers are people.
- Ask early. No question is too small.