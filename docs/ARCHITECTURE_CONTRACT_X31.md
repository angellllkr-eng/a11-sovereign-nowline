# X31 Architecture Contract

**Responsibility:** Nowline monitoring/action UI provenance module

**Repository status:** LEGACY / SOURCE-FREEZE

## Domain boundary
Owns historical Nowline/A11 monitoring-surface material only. It is not a current production authority.

## Typed agent/operator contract
Monitoring/action inputs and outputs must be typed and explicitly distinguish observation from requested action. Reusable capability must be reconciled into the canonical destination before activation.

## Layer separation
Domain: historical monitoring and action-surface logic. Interface: typed monitoring/action contract. Shared: schemas/utilities. Tests: deterministic state fixtures plus UI/integration tests when applicable.

## Auditability
Observed state, requested action, actor/approval context, and resulting evidence must remain distinguishable.

## Repository rule
This contract standardizes the repository boundary without creating a duplicate implementation. Existing capability is reconciled in place when this repository is canonical; legacy/source-freeze repositories remain provenance sources until reusable material is migrated and verified in its canonical destination.

## X31 invariant
**Domain → Agent/Operator Interface → Shared → Tests → Audit/Evidence**

No secret material belongs in Git. No production claim is valid without runtime evidence from the canonical deployment authority.
