---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/Rel
generated: 2026-01-26T08:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# Rel

## Overview

The `Rel/` directory contains theory about Galois connections induced by arbitrary binary relations. Given a relation `R` between types `α` and `β`, this module constructs a Galois connection between the power sets `Set α` and `(Set β)ᵒᵈ`, and establishes a canonical equivalence between the fixed points of the induced closure operators. This work has applications to topos theory and categorical logic.

## Key Files

| File | Purpose |
|------|---------|
| GaloisConnection.lean | Defines `leftDual` and `rightDual` operations that map a relation to adjoint order-preserving functions; proves these form a Galois connection and induce inverse bijections between fixed points |

## Subdirectories

*(No subdirectories)*

## Search Tags

relation binary-relation Galois-connection adjunction fixed-points dual power-set topos-theory categorical-logic closure-operator
