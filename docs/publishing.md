# Publishing (KolektivComputer)

Epic: [#2](https://github.com/KolektivComputer/.github/issues/2)

## Maven (dual)
1. Existing Yuri Capital / Nexus (keep)
2. GitHub Packages: `https://maven.pkg.github.com/KolektivComputer/<repo>`
   - Job: `permissions.packages: write`, env `GITHUB_ACTOR` + `GITHUB_TOKEN`

Org Gradle plugin (in progress): [gradle-conventions](https://github.com/KolektivComputer/gradle-conventions) → `computer.kolektiv.publishing`

## npm `@kolektiv/*`
- Scope all packages under `@kolektiv/`
- Dual: Yuri Capital npm **and** `https://npm.pkg.github.com` with `@kolektiv:registry=…`

## JSR
- JSR scope is **`@kolektiv`** (owned). Link each package to its GitHub repo for OIDC publish
- `jsr.json` + OIDC from Actions (`id-token: write`) — **not** a replacement for npm publish

## Reusable workflow templates
Copy from `workflow-templates/` into a repo’s `.github/workflows/` (org token may lack `workflows` scope to write them here as live reusable workflows).
