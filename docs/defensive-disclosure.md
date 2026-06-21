# Defensive Disclosure

Published: 2026-06-21

This page is a public, high-level disclosure of the Consequence Memory architecture and proof position. It is intended to establish a dated public description without publishing the private engine source code.

This is not a patent filing, legal opinion, open-source grant, commercial licence, or waiver of rights. Legal advice should be taken before relying on this document for patent, enforcement, licensing, investment, or commercial decisions.

## Name

Consequence Memory

## Owner

Motion-TimeSpace / Martin Ollett

## Private Engine

The private engine is maintained separately from this public proof kit. The private engine reached release `v0.8.0` with packaged artifacts, tests, type checks, install smoke checks, benchmark evidence, and public-safe proof materials.

## Public Problem Statement

Agent systems often need to adapt from consequences without retraining a model after every outcome.

The problem is not only reward maximisation. A useful agent should be able to remember:

- where harm happened
- which routes worked
- which routes only weakly appeared promising
- when trusted routes became stale or dangerous
- why one candidate action beat another
- what evidence supports a release decision

## Public Architecture Summary

Consequence Memory is a private-core agent memory layer that records outcome traces into separate memory structures and uses them to score, explain, and benchmark later decisions.

The public architecture includes these concepts:

- danger memory for harmful outcomes
- success memory for useful outcomes
- route memory for paths that worked
- candidate route memory for weakly observed or provisional routes
- stale route demotion when trusted behaviour becomes harmful
- action scoring that can combine base value, danger, success, route memory, and internal state
- explanation output for chosen and rejected actions
- guided first-use walkthrough tooling
- evidence cards for benchmark and release review

## Public Behavioural Claim

The public proof materials show a private `v0.8.0` engine that can generate release-readable evidence in two seeded benchmark domains:

- warehouse routing, where consequence-aware routing preserved delivery and reduced harm
- organism/internal-state behaviour, where consequence-aware behaviour improved survival and reduced harm

The public proof kit does not claim that every domain will produce the same deltas. It claims the architecture exists, has been packaged privately, and has produced the public-safe evidence included here.

## Difference From Nearby Existing Work

Consequence Memory is near several known research families:

- reinforcement learning
- episodic memory for agents
- case-based reasoning
- safe reinforcement learning and shielding
- model-based planning and evidence replay

The public position is not that every ingredient is new. The public position is that this project combines explicit consequence memories, route/candidate/stale behaviour, guided explanations, benchmark evidence cards, and private-core/public-proof packaging into a specific implementation and product workflow.

## Public Proof Materials

Start with:

- [v0.8.0 release evidence](../proofs/v0.8.0-release-evidence/README.md)
- [artifact hashes](artifact-hashes.md)
- [architecture overview](architecture-overview.md)
- [interface screenshots](interface-screenshots.md)
- [access request path](../ACCESS_REQUEST.md)

## Rights Reserved

This disclosure does not grant permission to copy, implement, host, sell, embed, sublicense, train on, or commercially use the private engine or a derivative implementation.

See [LICENSE.md](../LICENSE.md), [COMMERCIAL_USE.md](../COMMERCIAL_USE.md), and [NDA_ACCESS.md](../NDA_ACCESS.md).
