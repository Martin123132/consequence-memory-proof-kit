# Evidence Review Guide

Start with the suite evidence:

- [v0.8.0 release evidence](../proofs/v0.8.0-release-evidence/README.md)
- [artifact hashes](artifact-hashes.md)
- [defensive disclosure](defensive-disclosure.md)

Then inspect the benchmark cards:

- [warehouse evidence](../proofs/v0.8.0-release-evidence/warehouse/evidence_card.md)
- [organism evidence](../proofs/v0.8.0-release-evidence/organism/evidence_card.md)

## Reading The Evidence

Use the suite evidence for the release-readiness answer.

Use the warehouse card for route behaviour:

- delivered packages
- harm
- post-shift harm
- energy per delivery
- recovery steps

Use the organism card for internal-state behaviour:

- survived steps
- food events
- harm events
- final damage

## What Passed

The public-safe `v0.8.0` evidence shows:

- thresholds passed
- regressions passed
- warehouse delivery stayed at 30.00
- warehouse harm reduced by 21.7%
- organism survived steps improved by 66.12
- organism harm reduced by 23.1%

## What To Ask For Privately

If you need to review implementation, benchmark internals, or private release artifacts, use [ACCESS_REQUEST.md](../ACCESS_REQUEST.md).
