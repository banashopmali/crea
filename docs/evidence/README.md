# CREA Engineering Evidence

This directory contains curated engineering evidence for CREA.

## Purpose

Evidence demonstrates that a change, gate, release, or technical decision was actually verified.

Evidence must be factual, reproducible where possible, and tied to an identifiable repository state.

## Evidence Principles

Evidence should be:

- linked to an exact commit or branch state,
- attributable,
- timestamped where relevant,
- reproducible where practical,
- free of secrets,
- free of production personal data,
- free of real KYC documents,
- immutable once used for a ratified gate unless superseded explicitly.

## Typical Evidence

Depending on the change, evidence may include:

- commit SHA,
- Pull Request number,
- CI run ID,
- required check results,
- test results,
- static analysis results,
- dependency audit results,
- secret scan results,
- migration validation,
- security review,
- architecture review,
- screenshots of configuration where API verification is unavailable,
- benchmark results,
- rollback verification,
- reconciliation results.

## Evidence Record

Each significant evidence record should capture:

- repository
- branch
- target branch
- HEAD SHA
- date
- author or operator
- scope
- risk class
- CI run
- checks executed
- checks excluded
- result
- known exceptions
- related Pull Request
- related ADR where applicable

## Naming Convention

Use descriptive, traceable names.

Example:

`P0-01E-repository-activation-2026-10-01.md`

or

`PR-0001-bootstrap-evidence.md`

## Security Rules

Never commit evidence containing:

- passwords,
- access tokens,
- private keys,
- webhook secrets,
- API secrets,
- production credentials,
- real payment credentials,
- real KYC documents,
- regulated customer data.

Redact sensitive values before storing evidence.

## Authority

Evidence supports decisions; it does not replace governance.

A green CI run does not automatically make an architectural or security decision acceptable if the governing review has not occurred.

## Retention

Curated evidence required for governance, releases, incidents, security reviews, and financial integrity should remain traceable for the life of the relevant system or decision.
