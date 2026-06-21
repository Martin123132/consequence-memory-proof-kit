# Consequence Memory Evidence Card

Benchmark: `organism`
Mode: `consequence`
Generated: `2026-06-20T23:17:04.652062+00:00`
Commit: `9166cab`

## Headline

`consequence` survived 327.12 steps versus reward baseline 261.00, while reducing harm by +23.1%.

## Reader Guide

- Use the headline to see whether consequence memory improved survival while reducing harm.
- Use Metrics to compare reward-only behavior with consequence-aware behavior.
- Use Mode Comparison when tuning internal-state or cue-response behavior.

## Decision Guidance

Thresholds passed. This card is ready for review; use a suite run with regressions for release evidence.

## Benchmark Config

| Field | Value |
| --- | ---: |
| size | 24 |
| steps | 500 |
| seed_count | 8 |

## Metrics

| Metric | Reward | Candidate | Delta |
| --- | ---: | ---: | ---: |
| Survived steps | 261.00 | 327.12 | +66.12 |
| Food events | 249.12 | 279.38 | +30.25 |
| Harm events | 11.38 | 8.75 | -2.62 |
| Final damage | 1.08 | 0.75 | -0.33 |

## Relative To Reward

- Survival delta: +66.12
- Food delta: +30.25
- Harm reduction: +23.1%
- Final damage reduction: +30.8%

## Thresholds

Status: **passed**

## What To Inspect Next

- Open `summary.json` for exact threshold values, seed metadata, and machine-readable metrics.
- Open `results.csv` when you need per-seed rows instead of means.
- Run the product-gates suite when you need release-grade combined evidence.
- For internal-state behavior, inspect survival, food events, harm events, and final damage together.

## Mode Comparison

| Mode | Survived | Food | Harm | Final damage |
| --- | ---: | ---: | ---: | ---: |
| `consequence` | 327.12 | 279.38 | 8.75 | 0.75 |
| `reward` | 261.00 | 249.12 | 11.38 | 1.08 |
