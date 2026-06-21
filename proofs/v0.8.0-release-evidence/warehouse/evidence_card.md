# Consequence Memory Evidence Card

Mode: `consequence_planned`
Generated: `2026-06-20T23:17:03.164035+00:00`
Commit: `9166cab`

## Headline

`consequence_planned` kept delivery at 30.00 versus baseline 30.00, while reducing harm by +21.7%.

## Reader Guide

- Use the headline to see whether consequence memory preserved delivery while reducing harm.
- Use Metrics to compare baseline routing with the candidate mode.
- Use Mode Comparison when tuning route policy tradeoffs.

## Decision Guidance

Thresholds passed. This card is ready for review; use a suite run with regressions for release evidence.

## Benchmark Config

| Field | Value |
| --- | ---: |
| max_steps_per_package | 160 |
| packages | 30 |
| repair_delay | 3 |
| size | 32 |
| seed_count | 8 |

## Metrics

| Metric | Baseline | Candidate | Delta |
| --- | ---: | ---: | ---: |
| Delivered | 30.00 | 30.00 | +0.00 |
| Harm | 130.62 | 102.25 | -28.38 |
| Post-shift harm | 63.75 | 46.25 | -17.50 |
| Energy per delivery | 68.42 | 63.66 | -4.76 |
| Recovery steps | 49.12 | 55.50 | +6.38 |

## Relative To Baseline

- Delivered delta: +0.00
- Harm reduction: +21.7%
- Post-shift harm reduction: +27.5%
- Energy per delivery reduction: +7.0%

## Thresholds

Status: **passed**

## What To Inspect Next

- Open `summary.json` for exact threshold values, seed metadata, and machine-readable metrics.
- Open `results.csv` when you need per-seed rows instead of means.
- Run the product-gates suite when you need release-grade combined evidence.
- For route behavior, inspect recovery steps, candidate locks, and stale demotions together.

## Mode Comparison

| Mode | Delivered | Harm | Post-shift harm | Energy/delivery |
| --- | ---: | ---: | ---: | ---: |
| `baseline` | 30.00 | 130.62 | 63.75 | 68.42 |
| `consequence_efficient` | 5.00 | 357.12 | 163.50 | 1740.94 |
| `consequence_planned` | 30.00 | 102.25 | 46.25 | 63.66 |
| `consequence_safe` | 4.75 | 345.12 | 159.88 | 1844.37 |
