---
id: TASK-OBS-021
title: Implement Observation Window
status: backlog
priority: high
estimate: small
owner: AI
---

# Objective

Implement the Observation Window domain concept.

## References

Specifications

- FR-OBS-001
- Domain/Observation

Architecture

- Architecture/DDD
- Architecture/Layers

ADR

- ADR-0004

## Context

Observation Window is already specified but has not yet been implemented.

The Telemetry module already produces normalized sensor events.

## Deliverables

- Observation Window implementation
- Unit tests
- Documentation update if necessary

## Constraints

- Must follow DDD
- Must be immutable
- No infrastructure dependencies
- No new third-party libraries

## Acceptance Criteria

- [ ] Observation Window implemented
- [ ] All business rules supported
- [ ] Unit tests added
- [ ] Existing tests still pass
- [ ] Ruff passes
- [ ] MyPy passes

## Validation

Run

uv run pytest

uv run mypy

uv run ruff check

## Expected Files

Create

- packages/core/domain/observation_window.py

Modify

- packages/core/domain/__init__.py

May Modify

- tests/

Must Not Modify

- infrastructure/
- telemetry/

## Agent Guidance

Read before implementing:

1. specs/requirements/FR-OBS-001.md
2. specs/domain/observation.md
3. specs/architecture/principles.md

Implementation order:

1. Implement the domain object.
2. Add business rule validation.
3. Add unit tests.
4. Run validation.

Stop and report if:

- The specification is ambiguous.
- A required architectural decision is missing.
- The task requires changes outside the declared scope.