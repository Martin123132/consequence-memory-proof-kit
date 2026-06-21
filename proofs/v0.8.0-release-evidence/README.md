# v0.8.0 Release Evidence

This folder contains public-safe evidence from the private `consequence-memory` `v0.8.0` release-readiness run.

The original private evidence bundle was generated from the product-gates suite on 2026-06-20 UTC.

## Suite Result

| Check | Status |
| --- | --- |
| Thresholds | passed |
| Regressions | passed |
| Package version | 0.8.0 |
| Evidence run | v0.8.0-final-20260621 |

Public-safe files:

- [suite evidence card](suite_evidence_card.md)
- [suite results CSV](results.csv)

## Benchmarks

| Benchmark | Thresholds | Failures | Evidence |
| --- | --- | ---: | --- |
| warehouse | passed | 0 | [card](warehouse/evidence_card.md) |
| organism | passed | 0 | [card](organism/evidence_card.md) |

## Regression Snapshot

| Benchmark | Metric | Baseline | Current | Limit | Status |
| --- | --- | ---: | ---: | ---: | --- |
| warehouse | delivered | 30.000 | 30.000 | 29.500 | passed |
| warehouse | harm | 102.250 | 102.250 | 107.362 | passed |
| warehouse | post_shift_harm | 46.250 | 46.250 | 49.950 | passed |
| warehouse | energy_per_delivery | 63.662 | 63.662 | 68.755 | passed |
| warehouse | candidate_locks | 29.875 | 29.875 | 24.875 | passed |
| warehouse | stale_segment_demotions | 14.983 | 14.983 | 11.983 | passed |
| organism | survived_steps | 327.125 | 327.125 | 307.125 | passed |
| organism | food_events | 279.375 | 279.375 | 264.375 | passed |
| organism | harm_events | 8.750 | 8.750 | 10.062 | passed |
| organism | final_damage | 0.746 | 0.746 | 0.858 | passed |

## Public Boundary

This folder intentionally excludes private benchmark implementation, private threshold configuration files, source code, package artifacts, and full private evidence bundles.
