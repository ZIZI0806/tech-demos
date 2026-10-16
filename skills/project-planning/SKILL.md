# Project planning — Bun / shadcn MVP demos

Vendored skill for planning single-user sticky demos in this monorepo.

## When to use

Before coding any new `apps/<slug>/` demo. Produce a short `PLAN.md` in that app directory, then implement.

## Workflow

1. **One-sentence goal** — what the demo proves in one line.
2. **Single-user MVP + outs** — list the smallest set of features for one user; explicitly list what is out of scope.
3. **Outcome tasks** — break work into outcome-oriented tasks (not vague chores).
4. **Research prebuilts in parallel** — look for existing scaffolds, libraries, and shadcn patterns before inventing.
5. **Scaffold with `bunx create-*`** — prefer official / well-known create commands over hand-rolled setup.
6. **`bunfig.toml` before install** — add:

   ```toml
   [install]
   minimumReleaseAge = 259200
   ```

   then run `bun install`.
7. **Opinionated framework** — pick one clear stack (e.g. Vite + React + TypeScript) and stick to it.
8. **shadcn init** — when UI is needed, initialize shadcn/ui and reuse components.
9. **Structure** — keep a clear `apps/<slug>/` layout (src, components, routes as needed).
10. **Minimal tests / hooks** — only what proves the core path; skip ceremony.
11. **Short `PLAN.md`** — write the plan into `apps/<slug>/PLAN.md` before coding.

## Rules

- **One user first** — design for a single user; no multi-tenant / auth sprawl unless the bookmark topic requires it.
- **Bun default** — Bun for install, scripts, and runtime.
- **Prebuilt over bespoke** — prefer scaffolds and libraries over custom infrastructure.
- **Cut features before clarity** — if the demo is unclear, remove features rather than adding abstractions.
