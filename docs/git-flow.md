# 🚀 Git Flow for ML Portal

## 📌 Branching Strategy

| Branch      | Purpose                         |
| ----------- | ------------------------------- |
| `main`      | Stable, production-ready code   |
| `develop`   | Active development (merged PRs) |
| `feature/*` | New features in progress        |
| `fix/*`     | Bugfixes                        |
| `docs/*`    | Documentation-only updates      |
| `chore/*`   | Minor tweaks, tooling, CI, etc. |

> PRs should always be made **from a `feature/*` branch into `develop`**, not directly into `main`.

## ✅ Naming Examples

- `feature/{section}-{issue}/unit-card`
- `fix/{section}-{issue}/fix-useUnit-hook`
- `docs/{section}-{issue}/add-structure.md`
- `chore/{section}-{issue}/update-types`

> - {section} - project [section](architecture.md##Structure) name
> - {issue} - GitHub issue number (if applicable, otherwise use 0)

## 🧪 Local Checklist before PR

- [ ] Type check passes (`npm run typecheck`)
- [ ] Linter passes (`npm run lint`)
- [ ] Tested locally (`npm run dev`)

## 📅 Releases

- Merge `develop → main` only when a new version is ready
