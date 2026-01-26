---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/DiscreteValuationRing
generated: 2026-01-26T20:00:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# DiscreteValuationRing

## Overview

This directory contains the theory of discrete valuation rings (DVRs). The main file `Basic.lean` defines DVRs as local PIDs that are not fields, develops their core properties including the equivalence with being a PID with a unique non-zero prime ideal, constructs the additive valuation, and provides a non-canonical Euclidean domain structure. The file `TFAE.lean` proves that seven equivalent characterizations of DVRs hold for Noetherian local domains (including being a valuation ring, Dedekind domain, having principal maximal ideal, and having cotangent space dimension 1).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core DVR definition and theory; defines `IsDiscreteValuationRing` as local PID not a field; proves uniformizers exist and are characterized by irreducibility; constructs additive valuation `addVal R : AddValuation R ℕ∞`; provides non-canonical Euclidean domain structure via `toEuclideanDomain` |
| TFAE.lean | Equivalent characterizations of DVRs; proves seven conditions are equivalent for Noetherian local domains: DVR, valuation ring, Dedekind domain, integrally closed with unique non-zero prime, principal maximal ideal, cotangent space dimension 1, all nonzero ideals are powers of maximal ideal |

## Subdirectories

*(none)*

## Search Tags

discrete-valuation-ring DVR local-ring PID principal-ideal-domain valuation additive-valuation uniformizer irreducible prime-ideal maximal-ideal Noetherian Dedekind-domain valuation-ring integrally-closed cotangent-space Euclidean-domain TFAE equivalent-characterizations
