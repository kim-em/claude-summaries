---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RepresentationTheory/Homological/GroupCohomology
generated: 2026-01-26T19:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 7
subdirs_count: 0
---

# GroupCohomology

## Overview

This directory develops the theory of group cohomology for `k`-linear `G`-representations. The core definition models `Hⁿ(G, A)` as the cohomology of the complex of inhomogeneous cochains `0 → Fun(G⁰, A) → Fun(G¹, A) → Fun(G², A) → ...` with explicit combinatorial differentials involving the representation action and face maps. The development establishes the equivalence `Hⁿ(G, A) ≅ Extⁿ(k, A)` via the bar resolution, provides specialized API for low degrees (0, 1, 2), proves functoriality with respect to group homomorphisms and representation morphisms, develops the long exact sequence in cohomology, and establishes major theorems including Shapiro's lemma for coinduced representations and Hilbert's Theorem 90 for Galois extensions. Special treatment is given to finite cyclic groups with explicit descriptions of cohomology in terms of kernels and cokernels involving the norm map and `ρ(g) - Id`.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines group cohomology `Hⁿ(G, A)` as cohomology of inhomogeneous cochains complex with differential `d^n(f)(g₀,...,gₙ) = ρ(g₀)f(g₁,...,gₙ) + Σ(-1)^{i+1}f(...,gᵢgᵢ₊₁,...) + (-1)^{n+1}f(g₀,...,gₙ₋₁)`, proves isomorphism to bar resolution complex via `inhomogeneousCochainsIso`, establishes `groupCohomologyIsoExt` showing `Hⁿ(G, A) ≅ Extⁿ(k, A)` in `Rep k G`, provides cocycles and basic constructions |
| FiniteCyclic.lean | Group cohomology of finite cyclic groups: proves `H⁰(G, A) ≅ Ker(ρ(g) - Id)` via `groupCohomologyIso₀`, for odd `i` proves `Hⁱ(G, A) ≅ Ker(N)/Im(ρ(g) - Id)` via `groupCohomologyIsoOdd` using short complex `A --(ρ(g) - Id)--> A --N--> A`, for positive even `i` proves `Hⁱ(G, A) ≅ Ker(ρ(g) - Id)/Im(N)` via `groupCohomologyIsoEven` using `A --N--> A --(ρ(g) - Id)--> A`, provides quotient maps `groupCohomologyπEven` and `groupCohomologyπOdd` with characterizations of equality |
| Functoriality.lean | Functoriality of group cohomology: given group homomorphism `f : G →* H` and representation morphism `φ : Res(f)(A) ⟶ B`, defines cochain map `cochainsMap f φ` sending `x : Hⁿ → A` to `(g : Gⁿ) ↦ φ(x(f ∘ g))`, induces maps `Hⁿ(H, A) ⟶ Hⁿ(G, B)`, proves functoriality `map_comp` and identity laws, provides specialized maps for degrees 1, 2, 3, constructs natural transformations `resNatTrans` and `infNatTrans`, proves inf-res exact sequence `H¹(G/S, A^S) ⟶ H¹(G, A) ⟶ H¹(S, A)` exact via `H1InfRes_exact` with monomorphism on left |
| Hilbert90.lean | Hilbert's Theorem 90: proves Noether's generalization that `H¹(Aut_K(L), L×) = 0` for finite field extension `L/K` via `H1ofAutOnUnitsUnique`, establishes that every 1-cocycle `f : Aut_K(L) → L×` is a coboundary using Dedekind's linear independence of characters to find `β : L×` with `g(β)/β = f(g)`, deduces classical Hilbert 90 for cyclic Galois extensions: if `N_{L/K}(x) = 1` then `x = y/σ(y)` for some `y : L×` via `exists_div_of_norm_eq_one`, provides integral version `exists_mul_galRestrict_of_norm_eq_one` for integral closures |
| LongExactSequence.lean | Long exact sequence in group cohomology: proves short exact sequence `0 → X₁ → X₂ → X₃ → 0` of representations induces short exact sequence of cochain complexes via `map_cochainsFunctor_shortExact`, defines connecting homomorphism `δ hX i j hij : Hⁱ(G, X₃) → Hʲ(G, X₁)`, proves exactness of three short complexes in long exact sequence via `mapShortComplex₁_exact`, `mapShortComplex₂_exact`, `mapShortComplex₃_exact`, provides criteria for `δ` to be epi/mono/iso when certain cohomology vanishes |
| LowDegree.lean | Low-degree cohomology API: defines explicit differentials `d₀₁ : A → Fun(G, A)` sending `(a, g) ↦ ρ(g)(a) - a`, `d₁₂ : Fun(G, A) → Fun(G², A)` sending `(f, (g₁, g₂)) ↦ ρ(g₁)(f(g₂)) - f(g₁g₂) + f(g₁)`, `d₂₃` for second differential, establishes isomorphisms `cochainsIsoₙ` identifying `Cⁿ(G, A)` with `Fun(Gⁿ, A)`, proves `H⁰(G, A) ≅ A^G` (invariants) via `H0Iso`, defines submodules `cocycles₁`, `cocycles₂`, `coboundaries₁`, `coboundaries₂` with quotient maps `H1π`, `H2π`, provides support for additive/multiplicative cocycle predicates `IsMulCocycle₁`, proves `H¹(G, A) ≅ Hom(G, A)` when representation is trivial via `H1IsoOfIsTrivial` |
| Shapiro.lean | Shapiro's lemma for group cohomology: given subgroup `S ≤ G` and `S`-representation `A`, proves `Hⁿ(G, Coind_S^G(A)) ≅ Hⁿ(S, A)` via `coindIso`, uses that restriction functor `Res(S)` preserves projective objects (since `Coind_S^G` preserves epimorphisms and is right adjoint), establishes isomorphism `Hom(Res(S)(P), A) ≅ Hom(P, Coind_S^G(A))` for projective resolution `P` via `linearYonedaObjResProjectiveResolutionIso`, applies to bar resolution to obtain cohomology isomorphism |

## Subdirectories

(none)

## Search Tags

group-cohomology inhomogeneous-cochains bar-resolution ext-functor representation-theory cocycles coboundaries low-degree-cohomology h0-invariants h1-homomorphisms h2-extensions functoriality restriction-corestriction inflation coinduction shapiro-lemma hilbert-theorem-90 galois-cohomology finite-cyclic-groups norm-map long-exact-sequence connecting-homomorphism differential-graded projective-resolutions homological-algebra
