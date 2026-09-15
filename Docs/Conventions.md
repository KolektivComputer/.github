# Conventions

Preferred libraries and repo hygiene for KolektivComputer. Scaffold flags (Katalog) map to these sections.


## Rust CLIs (Katalog, Kascade)

- Pure CLI devtools are **Rust** (Cargo crates). Install: `cargo install` / GH Releases binaries.
- Preferred stack: **clap** (derive) · **serde** (+ yaml) for config/graphs · **tokio** only when async (e.g. BSP JSON-RPC) needs it.
- Prefer existing BSP Rust clients/servers before rolling a wire layer (Kascade).
- Optional thin `@kolektiv/*` npm wrappers only for `npx` — not the product story.
- Always spell **Kascade**.

## Kotlin / KMP

Preferred libs · when to use · scaffold flag — *TBD (Researcher matrix)*.

## Compose

Preferred libs · when to use · scaffold flag — *TBD*.

## Ktor / Keel

Preferred libs · when to use · scaffold flag — *TBD*.

## JS / TS (pnpm, Vite+, Vitest)

- Prefer **Vite+ (`vp`)** for Vite-shaped repos (commands: install/dev/check/test/build).
- Formatter/linter with Vite+: **Oxfmt + Oxlint** (not Biome) for those repos.
- **NixOS:** always prefer Nix for Node/tooling — do not use `vp env`.
- Scaffold flag — *TBD*.

## Cloudflare

Workers / wrangler · scaffold flag — *TBD*.

## Repo metadata (labels, templates, LICENSE, AGENTS)

- Org label prefixes: see [Issue Labels](./Issue%20Labels.md).
- YAML issue forms; Questions → Discussions.
- Package scope `@kolektiv/*`; Kotlin packages `computer.kolektiv.*` where applicable.
- Scaffold: Katalog · Monorepo runner: Kascade (always spell **Kascade**).

## Project organization

How multi-module / polyglot trees are laid out (apps, packages, workers, docs) — *TBD from current repos*.
