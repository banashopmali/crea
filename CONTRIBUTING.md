# Contributing to CREA

CREA follows an evidence-driven engineering process.

## Branch Model

- `main` — production authority
- `develop` — integration authority
- `feature/*` — new features
- `fix/*` — bug fixes
- `security/*` — security changes
- `release/*` — release preparation
- `chore/*` — repository and tooling work
- `docs/*` — documentation
- `spike/*` — temporary technical exploration

Direct pushes to `main` and `develop` are not allowed once branch protection is enabled.

## Pull Requests

All changes must be submitted through a Pull Request.

Default merge strategy:

- Squash merge
- Green CI required
- Relevant review completed
- Review conversations resolved

Critical changes require stronger review and evidence.

Critical domains include:

- Authentication
- Authorization
- Payments
- Ledger
- Payouts
- KYC / KYB
- Admin permissions
- Secrets
- Production infrastructure
- Premium media access
- Cryptography
- Audit logging

## Commit Convention

Use:

`<type>(<scope>): <description>`

Accepted types:

- feat
- fix
- docs
- test
- refactor
- perf
- build
- ci
- chore
- security
- revert

Example:

`feat(auth): add creator session validation`

## Security

Never commit:

- API keys
- passwords
- private keys
- `.env` files
- production credentials
- payment credentials
- KYC documents
- real personal data
- licensed third-party source archives

## Engineering Principles

- Flutter is the primary mobile client.
- Laravel is the initial backend platform.
- CREA Money is the financial authority.
- Client-side balances are never authoritative.
- Payment redirects never grant access by themselves.
- Premium media is private by default.
- Financial values must not use floating-point arithmetic.
- Generated code must have an explicit source of truth.
- AI-generated code follows the same review rules as human-written code.

## Evidence

Critical merges should preserve evidence such as:

- branch
- target branch
- commit SHA
- CI run
- test results
- review status
- known exceptions
