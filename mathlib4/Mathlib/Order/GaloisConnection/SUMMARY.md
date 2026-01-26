---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/GaloisConnection
generated: 2026-01-26T19:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# GaloisConnection

## Overview

The `GaloisConnection/` folder contains foundational definitions and theory for Galois connections, insertions, and coinsertions in Lean's order theory library. Galois connections are order-theoretic adjoints consisting of a pair of functions `l` and `u` satisfying `l a ≤ b ↔ a ≤ u b`, which are special cases of adjoint functors from category theory but don't depend on the category theory library. The folder includes core definitions, monotonicity properties, compositions, duality results, and importantly provides infrastructure for lifting order structures (lattices, complete lattices, bounded orders) from one type to another via Galois insertions and coinsertions.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions for GaloisConnection (order-theoretic adjoints), GaloisInsertion (`l ∘ u = id`), and GaloisCoinsertion (`u ∘ l = id`); includes basic properties like monotonicity, transitivity, uniqueness, construction methods (monotone_intro, compose, dfun), and commutativity results |
| Basic.lean | Advanced results and applications: operations on bounds/suprema/infima (upper/lower bounds transformations, `l_iSup`, `u_iInf`), lifting order structures via Galois insertions (liftSemilatticeSup, liftLattice, liftCompleteLattice with choice functions), concrete examples (gc_sSup_Iic, Nat.galoisConnection_mul_div, WithBot.giUnbotDBot), and Galois coinsertion lifting operations |

## Subdirectories

(none)

## Search Tags

Galois-connection Galois-insertion Galois-coinsertion order-adjoint monotone closure-operator order-lifting lattice-lifting complete-lattice infimum supremum bounds choice-function left-adjoint right-adjoint
