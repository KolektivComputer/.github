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

AI tools are welcome. Code can be AI-assisted to any degree as long as the human responsible can explain it in the PR without using AI to write the PR. That is the whole policy. The rules below are what it means in practice.

- Allowed at any level: autocomplete, first drafts, refactors, tests, explanations.
- You must explain every change yourself in review.
- Write the PR description and review replies yourself. Do not paste AI-generated PR text.
- Disclose AI usage in the PR (tools and what they helped with). Honest disclosure is never penalized.
- “The AI wrote it” is not an acceptable review answer. If you cannot explain a hunk, remove it or learn it before resubmitting.
- You are responsible for correctness, tests, licensing, and security of what you submit.
- If you use a coding agent, point it at that repository’s `AGENTS.md` when one exists.

## Licensing

Each repository has its own license (for example Apache-2.0 on Keel, AGPL on Kalendee). By opening a pull request you agree that your contribution may be distributed under that repository’s license. Only submit code you can license that way. Do not paste from incompatible or proprietary sources.

Inbound equals outbound for that repo. There is no org-wide CLA unless a repository says otherwise.

## Community

- Issues and pull requests are the main place to talk.
- Be patient and kind. Reviewers are people.
- Ask early. No question is too small.
