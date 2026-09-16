# Publishing (KolektivComputer)

Epic: [#2](https://github.com/KolektivComputer/.github/issues/2)

## Maven (dual)
1. Existing Yuri Capital / Nexus (keep)
2. GitHub Packages: `https://maven.pkg.github.com/KolektivComputer/<repo>`
   - Job: `permissions.packages: write`, env `GITHUB_ACTOR` + `GITHUB_TOKEN`

**GroupId family (locked):** `computer.kolektiv.*`  
(Not `dev.kolektiv.*`. Migrate remaining `dev.kolektiv.*` / template / legacy groups onto this family.)

Org Gradle plugin: [gradle-conventions](https://github.com/KolektivComputer/gradle-conventions) → `computer.kolektiv.publishing` (registers GH Packages + optional Yuri when `maven-publish` is applied). Fold per-repo publish helpers onto this spine — do not invent a parallel conventions story.

## npm `@kolektiv/*`
- Scope all packages under `@kolektiv/` — **do not invent a second JS scope**
- Dual: Yuri Capital npm **and** `https://npm.pkg.github.com` with `@kolektiv:registry=…`

## JSR
- JSR scope is **`@kolektiv`** (owned). Link each package to its GitHub repo for OIDC / trusted publishing
- `jsr.json` + OIDC from Actions (`id-token: write`) — **no org `JSR_TOKEN`** for Actions
- **not** a replacement for npm publish

## Reusable workflow templates
Copy from `workflow-templates/` into a repo’s `.github/workflows/` (org token may lack `workflows` scope to write them here as live reusable workflows).

Templates: `publish-maven-gh-packages.yml`, `publish-npm-gh-packages.yml`, `publish-jsr.yml`.
