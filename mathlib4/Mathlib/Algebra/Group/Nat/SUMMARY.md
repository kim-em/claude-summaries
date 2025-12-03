---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Group/Nat
generated: 2025-12-01T22:30:00Z
git_sha: dc19f2a67ff55a2078ba23a4c1740a5eb0d50e41
git_branch: master
status: complete
files_count: 6
subdirs_count: 0
---

# Nat

## Overview

This folder contains specialized group-theoretic constructions and properties for natural numbers (ℕ). It establishes the fundamental monoid instances for ℕ (additive commutative monoid and multiplicative commutative monoid), proves parity and evenness properties, characterizes homomorphisms from ℕ via their behavior on 1, and establishes that 1 is the only multiplicative unit in ℕ. These files provide the bridge between Lean's core natural number type and mathlib's algebraic hierarchy.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core monoid instances for ℕ: `AddCancelCommMonoid ℕ` and `CommMonoid ℕ` with torsion-freeness; includes short-circuit instances to prevent non-computable constructions |
| Even.lean | Parity theory for natural numbers: decidability of `Even` and `IsSquare`, characterization via modulo 2, and `parity_simps` lemmas for automated parity reasoning |
| Hom.lean | Extensionality and characterization of homomorphisms from ℕ: shows additive homomorphisms are determined by `f 1` via `multiplesHom` and `powersHom` equivalences |
| Range.lean | Interaction between `Finset.range` and addition: disjointness and decomposition lemmas for ranges under addition embeddings |
| TypeTags.lean | Lemmas for `Multiplicative ℕ`: conversion between addition and exponentiation via `toAdd_pow` and `ofAdd_mul` |
| Units.lean | Uniqueness of units in ℕ: proves `1` is the only multiplicative unit and `0` is the only additive unit, with `Unique` instances |

## Subdirectories

(none)

## Search Tags

natural-numbers nat monoid additive-monoid multiplicative-monoid parity even odd decidability homomorphism extensionality units additive-character finset range torsion-free commutative type-tags multiplicative
