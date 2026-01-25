---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/MulChar
generated: 2026-01-25T21:50:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# MulChar

## Overview

The `MulChar/` directory contains the theory of multiplicative characters on commutative monoids and rings. A multiplicative character is a monoid homomorphism that sends non-units to zero, forming a key tool in analytic number theory and harmonic analysis. The directory establishes the group structure of multiplicative characters, their equivalence with homomorphisms on unit groups, quadratic characters, duality theory for finite monoids, and comprehensive results for finite fields including character orders, roots of unity, and primitive root relationships.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of multiplicative characters, equivalence with unit group homomorphisms (`MulChar.equivToUnitHom`), commutative group structure, quadratic characters (values in {0,1,-1}), vanishing sums for nontrivial characters, and fundamental properties |
| Duality.lean | Duality theory for finite monoids with sufficient roots of unity: character separation of units, group isomorphism between characters and unit groups, and cardinality results |
| Lemmas.lean | Additional results including character equality criteria for cyclic unit groups, complex conjugation of characters, root of unity representations, equivalence between characters and roots of unity for cyclic groups, and comprehensive finite field character theory (existence, orders, primitive roots) |

## Subdirectories

*(None)*

## Search Tags

multiplicative-characters character-theory quadratic-characters duality roots-of-unity finite-fields unit-groups monoid-homomorphisms harmonic-analysis analytic-number-theory cyclic-groups primitive-roots character-sums
