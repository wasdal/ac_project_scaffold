# AGENTS.md

Compact guide for OpenCode sessions in this repo.

## Repository layout (intended)

This is a scaffolded project. Directories are placeholders until populated:

- `packages/` — code modules/packages live here (currently empty)
- `scripts/` — executable dev commands, one per concern:
  - `build.sh` — build
  - `lint.sh` — lint
  - `check.sh` — typecheck / static checks
  - `test.sh` — run tests
- `tests/` — test files (currently empty)
- `specs/` — specifications / requirements (currently empty)
- `prompts/` — reusable workflow prompts:
  - `implement.md`, `bugfix.md`, `refactor.md`, `review.md` — read the matching one before that task
- `docs/` — project docs (`architecture.md`, `conventions.md`, `coding-style.md`, `api.md`, `domain.md`, `glossary.md`, `common-pitfalls.md`, `lessons-learned.md`, and `adr/`)
- `tasks/` — task workflow, split into `backlog/`, `in-progress/`, `review/`, `completed/`

## Conventions to follow (expected, not yet enforced)

- Dev workflow is script-driven: prefer `scripts/*.sh` over invoking tools directly.
- Before implement/bugfix/refactor/review work, read the matching `prompts/*.md`.
- Track work as files under `tasks/` (move between `backlog` → `in-progress` → `review` → `completed`).
- Capture non-obvious learnings in `docs/lessons-learned.md` and `docs/common-pitfalls.md`.

## Unknown / not yet defined

- Exact build/test/lint/check commands — the `scripts/*.sh` files are empty. Run them after they are populated; do not assume tooling (language, framework) yet.
- No package manager, language, or CI config exists yet. Confirm before assuming.
- Not a git repo yet; initialize and establish conventions when first committing.

## References

- `docs/architecture.md`, `docs/conventions.md`, `docs/coding-style.md` — once written, prefer these over this file.
- `docs/adr/` — architecture decision records.
