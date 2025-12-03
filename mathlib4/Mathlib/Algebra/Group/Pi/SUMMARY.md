---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Group/Pi
generated: 2025-12-01T21:40:00Z
git_sha: dc19f2a67ff55a2078ba23a4c1740a5eb0d50e41
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# Pi

## Overview

The `Pi/` directory provides the foundation for pointwise group-theoretic operations on dependent function types (pi types), enabling families of algebraic objects `∀ i, f i` to inherit algebraic structures from their components. Basic.lean establishes core typeclass instances showing that pi types automatically form semigroups, monoids, groups, and their commutative variants when each component has such structure, with operations defined pointwise (e.g., `(f * g) i = f i * g i`). Lemmas.lean extends this with homomorphism constructions (`Pi.mulHom`, `Pi.monoidHom`) that lift families of homomorphisms into the product space, evaluation and constant maps, and the crucial `Pi.mulSingle` operations for updating single components while leaving others as identity. Units.lean completes the picture by establishing the fundamental equivalence `MulEquiv.piUnits : (∀ i, M i)ˣ ≃* ∀ i, (M i)ˣ` showing that units in a product are exactly the product of units, with the characterization `Pi.isUnit_iff : IsUnit x ↔ ∀ i, IsUnit (x i)`. This infrastructure is essential for working with direct products throughout algebra, enabling component-wise reasoning about families of group-like structures.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core typeclass instances for pi types defining pointwise group operations; provides `Pi.semigroup`, `Pi.monoid`, `Pi.group`, `Pi.commGroup` and their additive variants, along with cancellation instances and operations on `Function.extend` and `Sum.elim` |
| Lemmas.lean | Extended lemma library for pi group structures requiring additional imports; includes `Pi.mulHom`, `Pi.monoidHom`, evaluation and constant homomorphisms, `Pi.mulSingle` operations and properties, and lemmas for semiconjugacy, commutativity, and set piecewise operations |
| Units.lean | Units in pi types; defines `MulEquiv.piUnits` establishing the multiplicative equivalence between units of a product `(∀ i, M i)ˣ` and the product of units `∀ i, (M i)ˣ`, with characterization `Pi.isUnit_iff` |

## Subdirectories

(No subdirectories)

## Search Tags

pi-types dependent-types product-types group-structures pointwise-operations function-types homomorphisms evaluation units mul-single typeclass-instances to-additive
