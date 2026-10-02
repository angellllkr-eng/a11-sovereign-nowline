# Agent Repository Contract — A11 Sovereign Nowline

**Status:** SOURCE-FREEZE / LEGACY PROVENANCE
**Domain:** Historical A11/Nowline monitoring and action-surface capability.
**Boundary:** This repository is not a current production authority. Current product/runtime work belongs in its designated canonical repository.

## Typed agent interface
Historical monitoring capabilities should be described as typed status/query/action contracts before reconciliation.

Recommended boundary:
- `domain/`: monitoring state and operator-facing rules.
- `agent/`: typed status/query/action boundary.
- `shared/`: state, errors and evidence types.
- `tests/`: state-machine and UI/API integration tests.

## Auditability
Monitoring output must distinguish observed runtime evidence from configured intent. No UI status is proof of live execution without runtime evidence.

## Verification
Any promoted capability requires destination tests and independent live health/smoke evidence.
