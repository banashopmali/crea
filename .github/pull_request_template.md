# CREA Pull Request

## Summary

Describe what this Pull Request changes and why.

## Change Type

- [ ] Feature
- [ ] Fix
- [ ] Security
- [ ] Refactor
- [ ] Documentation
- [ ] CI / Build
- [ ] Infrastructure
- [ ] Repository governance
- [ ] Other

## Affected Areas

- [ ] Mobile
- [ ] Public Web
- [ ] Admin
- [ ] Backend
- [ ] Contracts
- [ ] Payments
- [ ] Ledger
- [ ] Payouts
- [ ] Identity / Auth
- [ ] KYC / KYB
- [ ] Risk / Moderation
- [ ] Infrastructure
- [ ] Documentation
- [ ] Repository policy

## Risk Class

- [ ] Class A — Low Risk
- [ ] Class B — Standard
- [ ] Class C — Critical
- [ ] Class D — Emergency

## Critical Domain Check

Does this change affect any of the following?

- [ ] Authentication
- [ ] Authorization
- [ ] Payments
- [ ] Ledger
- [ ] Payouts
- [ ] KYC / KYB
- [ ] Admin permissions
- [ ] Secrets
- [ ] Production infrastructure
- [ ] Premium media access
- [ ] Cryptography
- [ ] Audit logging

If yes, explain the additional review and evidence below.

## Verification

- [ ] Formatting passed
- [ ] Lint passed
- [ ] Static analysis passed where applicable
- [ ] Unit tests passed
- [ ] Integration tests passed where applicable
- [ ] Negative cases tested where applicable
- [ ] No secrets introduced
- [ ] No prohibited production or KYC data introduced
- [ ] Documentation updated where required

## Evidence

Provide relevant evidence:

- Branch:
- Target branch:
- HEAD SHA:
- CI run:
- Test results:
- Review status:
- Known exceptions:

## Security Notes

Describe any security impact, new dependency, secret handling change, permission change, or externally exposed surface.

If none:

`No known security impact.`

## Financial Integrity Notes

For changes affecting payments, ledger, payouts, refunds, chargebacks, or financial reporting, document:

- idempotency behavior
- replay behavior
- mismatch handling
- ledger impact
- reconciliation impact
- rollback or remediation path

If not applicable:

`Not applicable.`

## Rollback

Describe how this change can be safely rolled back or mitigated.

## Checklist

- [ ] The change is scoped and understood.
- [ ] The implementation follows CREA architecture boundaries.
- [ ] Required tests are included.
- [ ] Required CI checks are green.
- [ ] Critical findings are resolved.
- [ ] No direct production shortcut was introduced.
- [ ] Evidence is sufficient for the declared risk class.
