# Contract Versioning Policy

## Semantic Versioning
- MAJOR: breaking schema changes
- MINOR: backward-compatible additions
- PATCH: clarifications, non-breaking fixes

## Compatibility Rules
1. Core required fields must remain stable within a major version.
2. New optional fields are allowed in minor versions.
3. Field removals or type changes require a major version bump.

## Consumer Guidance
- Pin a major contract line (for example `v1`).
- Validate at system boundaries:
  - API ingress
  - queue publish/consume
  - adapter emit paths

## Initial Compatibility Matrix
- `conn-runtime`: supports `v1`
- `conn-orchestrator`: supports `v1`
- `conn-adapters`: supports `v1`
