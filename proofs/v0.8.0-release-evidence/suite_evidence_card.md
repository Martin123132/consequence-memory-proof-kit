# Consequence Memory Suite Evidence Card

Suite: `product-gates`
Run: `v0.8.0-final-20260621`
Generated: `2026-06-20T23:15:44.680417+00:00`
Package: `0.8.0`
Commit: `9166cab`

## Status

Thresholds: **passed**
Regressions: **passed**

## Reader Guide

- Use Status for the release-readiness answer.
- Use Benchmarks to open the per-benchmark evidence cards.
- Use Regression Checks before promoting a release candidate.

## Decision Guidance

Thresholds and regressions passed. This bundle is ready to cite as release evidence.

## Benchmarks

| Benchmark | Thresholds | Failures | Evidence |
| --- | --- | ---: | --- |
| `warehouse` | passed | 0 | [card](01-warehouse/evidence_card.md) |
| `organism` | passed | 0 | [card](02-organism/evidence_card.md) |

## Regression Checks

| Benchmark | Mode | Metric | Direction | Baseline | Current | Limit | Status |
| --- | --- | --- | --- | ---: | ---: | ---: | --- |
| `warehouse` | `consequence_planned` | `delivered` | min | 30.000 | 30.000 | 29.500 | passed |
| `warehouse` | `consequence_planned` | `harm` | max | 102.250 | 102.250 | 107.362 | passed |
| `warehouse` | `consequence_planned` | `post_shift_harm` | max | 46.250 | 46.250 | 49.950 | passed |
| `warehouse` | `consequence_planned` | `energy_per_delivery` | max | 63.662 | 63.662 | 68.755 | passed |
| `warehouse` | `consequence_planned` | `candidate_locks` | min | 29.875 | 29.875 | 24.875 | passed |
| `warehouse` | `consequence_planned` | `stale_segment_demotions` | min | 14.983 | 14.983 | 11.983 | passed |
| `organism` | `consequence` | `survived_steps` | min | 327.125 | 327.125 | 307.125 | passed |
| `organism` | `consequence` | `food_events` | min | 279.375 | 279.375 | 264.375 | passed |
| `organism` | `consequence` | `harm_events` | max | 8.750 | 8.750 | 10.062 | passed |
| `organism` | `consequence` | `final_damage` | max | 0.746 | 0.746 | 0.858 | passed |

## What To Inspect Next

- Open `summary.json` for the machine-readable suite result.
- Open a benchmark evidence card when one benchmark needs closer inspection.
- Use `consequence-benchmark-bundle-index` for a compact bundle map.
