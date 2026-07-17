# Guide for AI Coding Assistants.

This document explains how the coding agent is expected to work in this repo.

## Directory Map

Scaffolded project — directories are placeholders until populated:

- `packages/` — code modules/packages (empty)
- `scripts/` — dev commands:
  - `build.sh` — build
  - `lint.sh` — lint
  - `check.sh` — typecheck / static checks
  - `test.sh` — run tests
- `tests/` — test files (empty)
- `specs/` — specifications / requirements (empty)
- `prompts/` — reusable workflow prompts:
  - `implement.md`, `bugfix.md`, `refactor.md`, `review.md` — read the matching one before that task
- `docs/` — project docs:
  - `architecture.md`, `conventions.md`, `coding-style.md`, `api.md`, `domain.md`, `glossary.md`
  - `common-pitfalls.md`, `lessons-learned.md`
  - `adr/` — architecture decision records (empty)
- `tasks/` — task workflow: `backlog/` → `in-progress/` → `review/` → `completed/`

Specifications in specs folder conform the complete system contract. It includes:

- Product contract (vision, requirements, domain, use cases).

- Architectural contract (principles, layers, boundaries, quality attributes).

The rest of the repository supports that contract:

- docs/ explains the current implementation.
- adr/ explains why important decisions were made.
- tasks/ defines the incremental work to be done.


## Instructions

- follow directory map
- follow specifications from specs folder with status `approved`
- doc folder and subfolders do not contain any specifications, they are generated documentation after building


- Dev workflow is script-driven: prefer `scripts/*.sh` over invoking tools directly.
- Before implement/bugfix/refactor/review work, read the matching `prompts/*.md`.
- Track work as files under `tasks/` (move between the workflow stages).
- Capture non-obvious learnings in `docs/lessons-learned.md` and `docs/common-pitfalls.md`.

## Unknown / not yet defined---
id: SPEC-DOM-OBS
title: Observation Domain
status: approved
owner: Architecture
last_reviewed: 2026-07-16
depends_on:
  - SPEC-REQ-FUNC
related:
  - workflows/observation-cycle.md
  - acceptance/observation.md
---

- Exact build/test/lint/check commands — `scripts/*.sh` are empty. Run them after they are populated; do not assume tooling.
- No package manager, language, or CI config exists yet. Confirm before assuming.
- Not a git repo yet; initialize when first committing.

## References

- `docs/architecture.md`, `docs/conventions.md`, `docs/coding-style.md` — once written, prefer these over this file.
- `docs/adr/` — architecture decision records.
