---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Group/Irreducible
generated: 2025-12-01T21:35:00Z
git_sha: dc19f2a67ff55a2078ba23a4c1740a5eb0d50e41
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# Irreducible

## Overview

The `Irreducible/` directory defines the concept of irreducible elements in monoids—elements that are non-units and cannot be factored as a product of two non-units. This generalizes the notion of irreducible elements from ring theory to the monoid setting. The directory provides both the core definition and a collection of lemmas establishing fundamental properties and relationships with other algebraic concepts like units, powers, and multiplicative equivalences.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Defines `Irreducible p` and `AddIrreducible p` structures for monoids; establishes that irreducible elements are non-units that only factor into products where at least one factor is a unit; includes basic characterization lemmas like `irreducible_iff` and `not_irreducible_one` |
| Lemmas.lean | Proves additional properties of irreducible elements including non-irreducibility of powers (≠ 1), preservation under multiplication by units (`irreducible_units_mul`, `irreducible_mul_units`), characterization of irreducible products (`irreducible_mul_iff`), preservation under multiplicative equivalences (`MulEquiv.irreducible_iff`), and incompatibility with square elements (`Irreducible.not_isSquare`) |

## Subdirectories

None

## Search Tags

irreducible monoid non-unit factorization additive-irreducible multiplicative-equivalence units powers squares group-theory prime decomposition to-additive
