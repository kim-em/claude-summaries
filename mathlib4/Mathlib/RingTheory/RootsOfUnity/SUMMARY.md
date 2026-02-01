---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/RootsOfUnity
generated: 2026-02-01T21:30:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 8
subdirs_count: 0
---

# RootsOfUnity

## Overview

The `RootsOfUnity/` directory formalizes the theory of roots of unity in commutative monoids and rings. It defines roots of unity as elements `ζ` satisfying `ζ^n = 1`, provides the predicate `IsPrimitiveRoot` for primitive roots (those whose order is exactly `n`), and develops their algebraic properties. The directory includes specialized results for complex roots of unity, cyclotomic units (sums of powers of roots), minimal polynomials, and instances for algebraically closed fields. A key result is that roots of unity in integral domains form cyclic groups.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: `rootsOfUnity n M` as a subgroup of units, fundamental properties, proves `rootsOfUnity.isCyclic` (roots of unity in integral domains are cyclic) |
| PrimitiveRoots.lean | Predicate `IsPrimitiveRoot ζ k` for primitive roots, `primitiveRoots k R` finset, `autToPow` monoid homomorphism, equivalences like `zmodEquivZPowers`, cardinality results (`card_primitiveRoots = φ k`) |
| Complex.lean | Complex-specific theory: shows `n`-th roots are exactly `exp(2πi·j/n)` for `j < n`, proves cardinality equals `n`, shows all complex roots of unity have norm 1 |
| AlgebraicallyClosed.lean | Instances of `HasEnoughRootsOfUnity` for separably closed fields (contains primitive roots and cyclic root groups) when characteristic doesn't divide `n` |
| CyclotomicUnits.lean | Cyclotomic units theory (units formed from sums of powers of roots): association results for `ζ^i - 1` and `ζ^j - 1` when `i,j` coprime to `n` |
| EnoughRootsOfUnity.lean | Typeclass `HasEnoughRootsOfUnity M n` asserting `M` contains primitive `n`-th roots and the root group is cyclic, used for duality in groups of exponent `n` |
| Lemmas.lean | Additional results on primitive roots, proves `∏(1≤k<n)(1-μ^k) = n` for primitive `n`-th roots, divisibility results for `(μ-1)^k` in `ℤ[μ]` |
| Minpoly.lean | Minimal polynomial theory for roots of unity: shows roots are integral over `ℤ`, proves degree bounds `totient n ≤ deg(minpoly μ)` for primitive `n`-th roots |

## Subdirectories

(No subdirectories)

## Search Tags

roots-of-unity primitive-root cyclotomic-unit IsPrimitiveRoot rootsOfUnity complex-roots exp cyclic-group totient Euler-phi minimal-polynomial integral algebraically-closed separably-closed HasEnoughRootsOfUnity ZMod equivalence automorphism norm Kummer-extension divisibility associated-elements units subgroup
