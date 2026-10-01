# CREA Security Policy

Security is a release requirement for CREA.

## Reporting a Security Issue

Do not disclose suspected vulnerabilities publicly through GitHub Issues, Discussions, or Pull Requests.

Security findings must be reported privately to the CREA technical authority.

Until a dedicated security contact and private disclosure channel are established, vulnerabilities must be handled through the project owner and restricted engineering channels.

## Critical Security Domains

The following areas require elevated review and evidence:

- Authentication
- Authorization
- Session management
- Payments
- Ledger
- Payouts
- Refunds and chargebacks
- KYC / KYB
- Admin privileges
- Secrets and credentials
- Premium media authorization
- Production infrastructure
- Cryptography
- Webhooks
- Audit logging
- Personally identifiable information
- Financial data

## Secrets

Never commit:

- API keys
- passwords
- access tokens
- refresh tokens
- private keys
- payment provider credentials
- database credentials
- production `.env` files
- signing secrets
- webhook secrets
- KYC provider secrets
- cloud credentials

If a real secret is committed, treat it as compromised.

Removing the secret from Git history is not sufficient by itself.

The credential must be:

1. revoked or rotated,
2. replaced,
3. reviewed for unauthorized use,
4. documented in the incident evidence.

## Payment Security

The client application must never be the authority for payment success.

CREA must not grant paid access from:

- client redirects,
- client-side flags,
- screenshots,
- unverified callback parameters,
- local device state.

Paid entitlements may only be granted after server-side verification and authoritative transaction processing.

Payment operations must be idempotent and auditable.

## Financial Integrity

Financial values must not use floating-point arithmetic.

Ledger records must be append-oriented and auditable.

A mutable displayed balance must never replace authoritative ledger evidence.

## Premium Content

Premium media must be private by default.

Access must depend on server-authorized entitlement checks.

Permanent public URLs for protected content are prohibited.

## Personal and KYC Data

Real KYC documents, identity records, payment credentials, or production personal data must never be used in:

- source control,
- test fixtures,
- CI artifacts,
- screenshots committed to Git,
- documentation examples.

Use synthetic or properly anonymized data.

## Dependencies

Critical dependencies require security review.

Do not introduce custom cryptography where established and reviewed primitives or libraries exist.

Dependency vulnerabilities affecting critical runtime paths must be remediated or explicitly documented with:

- advisory reference,
- exposure analysis,
- mitigation,
- owner,
- expiry or remediation deadline.

## AI-Generated Code

AI-generated code receives the same security review as human-written code.

AI output is never considered trusted solely because it compiles or passes generated tests.

## Incident Handling

Security incidents should preserve evidence including:

- affected component,
- discovery time,
- severity,
- impacted environment,
- related commit SHA,
- credentials involved,
- containment actions,
- remediation,
- rotation actions,
- follow-up controls.

## Disclosure Status

A dedicated security mailbox, responsible security contact, response SLA, and coordinated vulnerability disclosure process will be established before production launch.
