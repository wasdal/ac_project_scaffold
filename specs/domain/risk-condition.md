---
title: Risk Condition
author: wasdal
last_update: 2026-07-18
status: approved
summary: Risk Condition concept
---

## Definition

A specific ambient state that could be considered risky to humans from some perspective.

## Examples

- The human pilot is out of its seat and the automatic pilot is off.
- The gas valve for the burner is open and there is no body in the room.
- The elderly person's caregiver is using inappropriate language with him.

## Attributes

- detection_timestamp: when the condition was detected
- timestamp: estimation of when the condition started
- description: textual description of the condition
- rationale: rationale on why the risk condition was considered detected
- severity: risk severity level (Negligible -> Minor -> Moderate -> Major -> Severe)

## Business Rules

- All Risk Conditions detected should be logged for audit purposes.
