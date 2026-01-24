---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/FieldTheory/PurelyInseparable
generated: 2026-01-24T23:45:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# PurelyInseparable

## Overview

The `PurelyInseparable/` directory provides a comprehensive formalization of purely inseparable field extensions in Lean. A purely inseparable extension E/F is one where every element not in F has an inseparable minimal polynomial. The directory covers basic theory, exponents of purely inseparable extensions, the relationship to perfect closures, and tower laws for separable and inseparable degrees. Key results include characterizations via powers (x^(q^n) ∈ F), minimal polynomial forms, and the fundamental fact that purely inseparable extensions are categorical epimorphisms.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions and results: `IsPurelyInseparable` typeclass, characterizations via power membership, minimal polynomial forms (X^(q^n) - C y), relationship to separable closure, tower properties (transitivity), finite separable/inseparable degree formulas, and epimorphism property in the category of fields |
| Exponent.lean | Exponent theory for purely inseparable extensions: defines `HasExponent` typeclass and `exponent` function (smallest n such that all elements satisfy x^(p^n) ∈ K), element-wise exponents (`elemExponent`), iterated Frobenius maps (`iterateFrobenius`, `iterateFrobeniusₛₗ`) acting as x ↦ x^(p^n) with codomain in base field |
| PerfectClosure.lean | Relative perfect closure: defines `perfectClosure F E` as maximal purely inseparable subextension (elements x with x^(q^n) ∈ F for some n), proves it's purely inseparable over F, characterization via minimal polynomial separable degree, preservation under algebra homomorphisms, and relationship to separable/perfect fields |
| Tower.lean | Tower laws for field extensions: proves separable and inseparable degrees satisfy multiplicativity in towers ([E:F]ₛ[K:E]ₛ = [K:F]ₛ and [E:F]ᵢ[K:E]ᵢ = [K:F]ᵢ), linear independence preservation, minimal polynomial equality across purely inseparable extensions, and irreducibility preservation of separable polynomials |

## Subdirectories

## Search Tags

purely-inseparable field-extensions separable-degree inseparable-degree exponent perfect-closure tower-law minimal-polynomials frobenius characteristic-p field-theory algebraic-extensions epimorphisms separable-closure linear-disjoint
