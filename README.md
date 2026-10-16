# tech-demos / 技术 Demo 单体仓库

**EN:** Sticky Bun monorepo for weekday X-bookmark tech demos. Each demo lives in `apps/<slug>/`. One repo forever — never one repo per demo. PRs must include at least one screenshot **and** one video of the running app.

**ZH:** 固定使用本 Bun 单体仓库承载工作日从 X 书签挑出的新技术 demo。每个 demo 放在 `apps/<slug>/`。永远只用这一仓库，不要为每个技术新建仓库。PR 必须附上至少一张截图和一段运行中应用的视频。

## Quick layout

```
apps/<slug>/     # one self-contained demo app each
skills/          # agent skills (e.g. project-planning)
tracking/        # seen bookmarks ledger
AGENTS.md        # rules for coding agents
```

## Per-app workflow

```bash
cd apps/<slug>
bun install
bun run dev
```
