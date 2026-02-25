# conn-contracts

Source-of-truth contracts for connector orchestration, runtime, and adapters.

## Scope
- JSON Schemas for control-plane requests and events
- JSON Schemas for normalized document envelopes
- Versioning and compatibility policy

## Current Version
- `v1` baseline contracts

## Contracts
- `schemas/sync_request.v1.json`
- `schemas/normalized_document.base.v1.json`
- `schemas/sync_run_event.v1.json`
- `schemas/checkpoint.v1.json`

## Design Rules
- Additive changes are preferred.
- Breaking changes require a new major contract version.
- Runtime and orchestrator should validate inbound/outbound messages against these schemas.
