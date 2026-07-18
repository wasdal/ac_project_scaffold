---
title: Alarm Channel
author: wasdal
last_update: 2026-07-18
status: approved
summary: Alarm Channel concept
---

## General Diagram

┌────────────────────────────┐
│  Perception (edge)         │
│                            │
└────────────────────────────┘
        │  normalized PerceptionEvents

┌────────────────────────┐
│    Risk Detection      │
└───────────┬────────────┘


▼
▲

```mermaid
graph TD

Runtime --> Application
Application --> Domain
Infrastructure --> Domain
Presentation --> Application
```
