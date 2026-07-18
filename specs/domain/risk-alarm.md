---
title: Risk Alarm
author: wasdal
last_update: 2026-07-18
status: approved
summary: Risk Alarm concept
---

## Definition

An event triggered with the intention to notify humans and lead their attention to some Risk Condition identified by the system.

## Attributes

- timestamp: when the alarm was issued
- risk: Risk Condition detected

## Business Rules

- Whenever a Risk Condition is detected, a Risk Alarm should be issued.
- All Risk Alarms issued should be logged for audit purposes.

## References

- Risk Condition
