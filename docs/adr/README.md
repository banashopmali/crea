# CREA Architecture Decision Records

This directory contains Architecture Decision Records (ADRs) for material technical decisions in CREA.

## Purpose

ADRs preserve the context, decision, consequences, and status of significant architectural choices.

They complement the higher-level governance documentation by recording decisions close to the implementation.

## When an ADR Is Required

Create or update an ADR when a change materially affects:

- system boundaries,
- API contracts,
- authentication or authorization,
- payment architecture,
- ledger architecture,
- payout architecture,
- KYC / KYB,
- trust and moderation,
- premium media access,
- storage architecture,
- infrastructure topology,
- deployment strategy,
- database technology,
- critical dependencies,
- cryptography,
- observability,
- availability or resilience,
- major third-party platform coupling.

Minor implementation details do not require an ADR unless they create a durable architectural constraint.

## ADR Statuses

Use one of:

- PROPOSED
- ACCEPTED
- SUPERSEDED
- DEPRECATED
- REJECTED

## Naming Convention

Use:

`ADR-XXXX-short-decision-title.md`

Example:

`ADR-0001-api-first-platform-boundary.md`

## Required Structure

Each ADR should include:

1. Title
2. Status
3. Date
4. Context
5. Decision
6. Alternatives Considered
7. Consequences
8. Security Impact
9. Financial Integrity Impact
10. Operational Impact
11. Migration / Rollback
12. Related Evidence
13. Supersedes / Superseded By

## Governance

An ADR must not silently override a ratified higher-level CREA decision.

If an implementation requires changing an authoritative governance decision, the governing decision must be explicitly reviewed and updated first.

## Evidence

Accepted ADRs should reference, where applicable:

- Pull Request
- commit SHA
- CI run
- tests
- benchmarks
- security review
- migration plan
- rollback plan
