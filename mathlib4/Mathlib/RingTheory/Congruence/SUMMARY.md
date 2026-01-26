---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Congruence
generated: 2026-01-26T20:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# Congruence

## Overview

The `Congruence/` directory formalizes congruence relations on rings and semirings, which are equivalence relations that preserve both addition and multiplication. These generalize the familiar notion of congruence modulo an ideal and provide the foundation for quotient rings. The directory includes core definitions, quotient construction, lattice structure, universal properties, isomorphism theorems (first, second, and third), interactions with big operators (sums and products), and opposite ring constructions. While `Ideal.Quotient` provides a more convenient API for most applications, this infrastructure offers general congruence relation machinery that extends beyond ideals and supports both ring homomorphisms and algebra homomorphisms.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: `RingCon R` structure combining `Con` and `AddCon`, `ringConGen` for generating smallest congruence containing a relation, quotient construction with ring structure, coercion and comap operations |
| Basic.lean | Fundamental properties: scalar multiplication on quotients, lattice structure (infimum, supremum, complete lattice), Galois insertion between congruences and binary relations, nontriviality conditions |
| Hom.lean | Ring homomorphism theory: kernel as congruence, lift/liftₐ for quotient universal property, map/factorₐ between quotients, first/second/third isomorphism theorems for semirings/rings/algebras, quotient equivalences |
| BigOperators.lean | Preservation of finite sums and products: congruences respect list sums, multiset sums, and finset sums by delegating to underlying `AddCon` |
| Opposite.lean | Opposite ring constructions: `op` and `unop` functors giving order isomorphism between `RingCon R` and `RingCon Rᵐᵒᵖ` |

## Subdirectories

(none)

## Search Tags

ring-congruence congruence-relation equivalence-relation quotient-ring kernel universal-property isomorphism-theorem first-isomorphism-theorem second-isomorphism-theorem third-isomorphism-theorem lattice complete-lattice Galois-insertion lift factor opposite-ring algebraic-structure semiring commutative-algebra
