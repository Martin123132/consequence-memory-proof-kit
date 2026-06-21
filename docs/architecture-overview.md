# Architecture Overview

This is a public-safe architecture overview. It describes the shape of the private engine without publishing its implementation.

## Core Idea

Consequence Memory stores outcome traces in separate memory surfaces and uses those surfaces to influence later decisions.

The private engine currently contains these product concepts:

- danger memory for harmful outcomes
- success memory for useful outcomes
- route memory for paths that worked
- candidate route memory for weakly observed routes
- stale demotion when trusted routes become harmful
- action scoring that can combine base value, danger, success, route memory, and internal state
- guided explanations for chosen and rejected actions
- evidence tooling for benchmark and release-gate review

## Public Benchmark Domains

The proof kit uses two public-safe domains:

- warehouse routing, where the system tries to preserve delivery while reducing harm
- organism/internal-state behaviour, where the system tries to improve survival while reducing harm

These are reference benchmarks and proof surfaces. They are not the only possible use cases.

## Private Implementation Boundary

This repository does not include:

- source code
- algorithms
- benchmark internals
- private package artifacts
- private release automation
- unpublished notebooks

The architecture overview is intentionally high level.

