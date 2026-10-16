# Agent rules — tech-demos sticky monorepo

You work inside this single sticky Bun monorepo. Follow these rules strictly.

## Scope

- **Only touch** `apps/<kebab-slug>/` for the demo you are building.
- **Never** create a new GitHub repository. All demos stay in this monorepo.
- Do **not** touch other apps, `tracking/`, or the repo root unless required for workspace wiring (e.g. root package workspace entry).

## App requirements

- Each demo must be **self-contained**: from `apps/<slug>/`, `bun install && bun run dev` must work.
- Use **Bun** as the package manager and runtime.
- Before `bun install` in an app, ensure that app has a `bunfig.toml` with:

  ```toml
  [install]
  minimumReleaseAge = 259200
  ```

- Prefer `bunx create-*` scaffolds for bootstrapping.
- Prefer **shadcn/ui** when the demo needs UI.

## Planning

- Follow `skills/project-planning/` before writing feature code.
- Write `apps/<slug>/PLAN.md` (short) before coding.

## Pull requests

- Open **one PR** per demo.
- The PR **MUST** attach at least **one screenshot** and **one video** of the running app.
