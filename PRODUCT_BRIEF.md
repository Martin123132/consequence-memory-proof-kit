# Product Brief

## What It Is

Consequence Memory is a private-core memory layer for agents and decision systems that need to adapt from outcomes.

Instead of relying only on a fresh prompt, a scalar reward, or a retrained model, the private engine records consequences in explicit memory structures. Harm, success, routes, candidate routes, stale behaviour, and decision explanations become inspectable parts of the next decision.

## The Problem

Many agent systems can generate actions, but they do not have a clean product layer for remembering what happened after those actions.

That creates recurring problems:

- harmful routes are rediscovered instead of avoided
- useful routes are not reused reliably
- weakly promising options are treated as proven too early
- stale behaviours keep being trusted after the world changes
- reviewers cannot easily see why one action was chosen over another
- release decisions lack readable evidence

## The Product Position

Consequence Memory sits between raw model output and application action.

It is not a full reinforcement-learning framework. It is a consequence-memory layer that can be embedded into simulations, agent loops, routing systems, game AI, logistics prototypes, safety benchmarks, or other decision systems that need explicit memory of outcomes.

## What The Private Engine Does

The private engine includes:

- danger memory for harmful outcomes
- success memory for useful outcomes
- route memory for paths that worked
- candidate route memory for provisional routes
- stale demotion when trusted behaviour becomes harmful
- action scoring that can combine base value, danger, success, route memory, and internal state
- guided explanations for chosen and rejected actions
- benchmark and release evidence tooling
- local first-use walkthrough tooling

## Public Evidence

The `v0.8.0` private release produced public-safe proof materials:

| Evidence | Result |
| --- | --- |
| Product-gates suite | thresholds and regressions passed |
| Warehouse benchmark | delivery preserved, harm reduced by 21.7% |
| Organism benchmark | survival improved by 66.12 steps, harm reduced by 23.1% |
| Interface screenshots | guided walkthrough shown on desktop and mobile |
| Artifact hashes | private wheel, sdist, and evidence bundle committed by SHA-256 |

## Who Should Care

Potential reviewers include:

- agent builders who need memory of consequences
- safety and evaluation teams
- simulation and benchmark developers
- robotics or routing prototype teams
- game AI developers
- research groups evaluating explicit agent memory
- commercial teams considering private pilot access

## What Is Public

This proof kit publishes:

- product narrative
- public-safe evidence cards
- screenshots
- defensive disclosure
- artifact hash commitments
- access request process
- commercial and NDA boundary

## What Remains Private

The private repository keeps:

- engine source code
- implementation details
- private package artifacts
- benchmark internals
- threshold configurations
- unpublished notebooks
- private release evidence bundles
- commercial pilot materials

## Access Path

Start with the public proof kit. If deeper review is needed, request private access using [ACCESS_REQUEST.md](ACCESS_REQUEST.md).

Private access may require written approval and an NDA. Commercial use requires separate written terms.
