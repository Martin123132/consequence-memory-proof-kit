# Public Proof One-Pager

## What It Is

Consequence Memory is a private-core agent memory layer for learning from outcomes.

Instead of treating every decision as fresh, it records consequences:

- harm becomes danger memory
- success becomes success and route memory
- weak routes become candidates
- stale trusted routes can be demoted
- scoring can explain why one action beat another

## Why It Matters

Agent systems often need a middle layer between raw reward chasing and full model retraining. Consequence Memory is aimed at that middle layer: explicit, inspectable memory that can influence future choices and produce evidence about what changed.

## Public Evidence

The `v0.8.0` private release produced public-safe release evidence:

- product-gates suite: thresholds passed
- product-gates suite: regressions passed
- warehouse benchmark: delivery preserved, harm reduced
- organism benchmark: survival improved, harm reduced
- guided interface: desktop and mobile screenshots

## Access Boundary

The proof kit is public. The engine is private.

Access to source, private release artifacts, implementation review, or commercial use requires written permission and may require an NDA.

