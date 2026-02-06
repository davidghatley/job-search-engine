# Proof Project 1: Connector Sync

## Summary
Build a single “gold‑standard” connector that syncs records from a source system into a destination with idempotency and incremental updates.

## Scope
- Source: CSV/S3 or demo API.
- Destination: Airtable or Postgres.
- Sync Mode: full + incremental.

## Key Capabilities
- **Idempotency**: Upsert by external ID.
- **Incremental sync**: track cursor/last updated.
- **Field mapping**: declarative mapping config.
- **Metrics**: records created/updated/skipped.

## Deliverables
- CLI or minimal UI to configure + run sync.
- README with setup + demo steps.
- Sample dataset + mapping config.

## Acceptance Criteria
- Demonstrate idempotent upserts with duplicate input.
- Incremental sync respects last_updated cursor.
- Clear metrics output with created/updated/skipped counts.
