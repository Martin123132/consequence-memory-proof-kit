# Consequence Memory Proof Kit

Consequence Memory is a private-core agent memory technology for systems that need to learn from what their actions do.

It records harmful outcomes as danger memory, useful outcomes as success and route memory, weak routes as candidates, and stale routes as demotion targets when trusted paths become harmful. The private engine packages those behaviours into reusable Python primitives, benchmarks, evidence cards, and guided first-use tooling.

This public repository is not the product source code and is not an open-source release. It is a proof kit: public-safe evidence, screenshots, evaluation notes, and an access path for people who want to request private review.

## Public Proof Release

The current private engine release is `v0.8.0`.

Public-safe proof materials in this repo show:

- guided consequence-aware decision explanation
- a local walkthrough interface concept
- warehouse routing benchmark evidence
- organism/internal-state benchmark evidence
- release-grade product-gates evidence
- private-core/public-proof publication boundary

## Locked Results

The `v0.8.0` product-gates evidence bundle passed thresholds and regressions.

| Proof | What it shows | Headline result |
| --- | --- | ---: |
| [Suite evidence](proofs/v0.8.0-release-evidence/README.md) | Combined release-readiness gates | passed |
| [Warehouse routing](proofs/v0.8.0-release-evidence/warehouse/evidence_card.md) | Delivery preserved while harm reduced | 30.00 delivered, 21.7% harm reduction |
| [Organism state](proofs/v0.8.0-release-evidence/organism/evidence_card.md) | Survival improved while harm reduced | +66.12 survived steps, 23.1% harm reduction |
| [Walkthrough UI](docs/interface-screenshots.md) | Guided first-use interface concept | desktop and mobile screenshots |

## What This Proves

- Consequence Memory can produce release-readable benchmark evidence.
- Consequence-aware routing can preserve delivery while reducing harm in a seeded warehouse benchmark.
- Consequence-aware internal-state behaviour can improve survival while reducing harm in a seeded organism benchmark.
- The project has a guided explanation and walkthrough path for first-time users.
- The private engine reached a packaged `v0.8.0` checkpoint with local tests, type checks, build checks, install smoke checks, and product-gates evidence.

## What This Does Not Prove

- It does not publish the private Consequence Memory implementation.
- It does not grant an open-source licence.
- It does not grant a commercial licence.
- It does not grant a patent licence, trademark licence, hosted-service right, model-provider right, or AI-platform integration right.
- It does not claim every environment will produce the same benchmark deltas.
- It does not replace a private pilot, technical review, or customer-specific evaluation.

## Private Engine Access

The private implementation remains closed. Access to the private repository, private wheel, source distribution, benchmark internals, or commercial evaluation requires written permission from Motion-TimeSpace / Martin Ollett and may require a signed NDA.

Start with:

- [Access Request](ACCESS_REQUEST.md)
- [NDA Access Path](NDA_ACCESS.md)
- [Commercial Use](COMMERCIAL_USE.md)
- [Public Materials License](LICENSE.md)

## Buyer And Reviewer Materials

- [Public proof one-pager](docs/public-proof-one-pager.md)
- [Evidence review guide](docs/evidence-review-guide.md)
- [Architecture overview](docs/architecture-overview.md)
- [Interface screenshots](docs/interface-screenshots.md)
- [Access request checklist](docs/access-request-checklist.md)
- [Proof scope](PROOF_SCOPE.md)

## Publication Boundary

This repository exists so interested people can understand the shape of the work without receiving the private engine.

The public proof kit can be cited, reviewed, and linked for evaluation. The implementation, private release artifacts, benchmark internals, and commercial use rights remain private unless granted separately in writing.

