---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RepresentationTheory/Homological/GroupHomology
generated: 2026-01-26T09:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 6
subdirs_count: 0
---

# GroupHomology

## Overview

The `GroupHomology/` directory implements the theory of group homology for k-linear G-representations. It defines group homology Hₙ(G, A) as the homology of the complex of inhomogeneous chains (bigoplus over Gⁿ), establishes the fundamental isomorphism Hₙ(G, A) ≅ Torₙ(A, k), and provides comprehensive API for working with homology in low degrees (0, 1, 2). The directory covers functoriality properties (maps induced by group homomorphisms), specialized results for finite cyclic groups (periodic resolutions), long exact sequences from short exact sequences of representations, and Shapiro's lemma relating homology of induced representations.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: Rep.Tor functor (left-derived functors from (A, B) ↦ (A ⊗ B)_G), inhomogeneousChains complex with differentials dₙ, groupHomology as homology of inhomogeneousChains, fundamental isomorphism groupHomologyIsoTor: Hₙ(G, A) ≅ Torₙ(A, k), establishes d² = 0 by relating inhomogeneousChains to (A ⊗ P)_G where P is bar resolution |
| FiniteCyclic.lean | Specialized homology for finite cyclic groups: for G = ⟨g⟩ finite cyclic, provides groupHomologyIso₀: H₀(G, A) ≅ Coker(ρ(g) - Id), groupHomologyIsoEven: Hᵢ(G, A) ≅ H(A --(ρ(g) - Id)--> A --N--> A) for even i > 0, groupHomologyIsoOdd: Hᵢ(G, A) ≅ H(A --N--> A --(ρ(g) - Id)--> A) for odd i, uses coinvariantsTensorResolutionIso to relate (A ⊗ P)_G to periodic chain complexes |
| Functoriality.lean | Functoriality of group homology: chainsMap sends group homomorphism f: G →* H and representation morphism φ: A ⟶ Res(f)(B) to chain map inhomogeneousChains A ⟶ inhomogeneousChains B, induces groupHomology.map: Hₙ(G, A) ⟶ Hₙ(H, B), defines corestriction and coinflation natural transformations, proves exactness of H₁CoresCoinf sequence: H₁(S, A) ⟶ H₁(G, A) ⟶ H₁(G ⧸ S, A_S) for normal subgroup S, provides extensive API for composition, mono/epi preservation |
| LongExactSequence.lean | Long exact sequences in group homology: proves short exact sequence 0 ⟶ X₁ ⟶ X₂ ⟶ X₃ ⟶ 0 of representations induces short exact sequence of inhomogeneousChains complexes, defines connecting homomorphism δ: Hᵢ(G, X₃) ⟶ Hⱼ(G, X₁), establishes exactness of three-term sequences mapShortComplex₁, mapShortComplex₂, mapShortComplex₃, provides explicit formulas δ₀_apply and δ₁_apply for low-degree connecting maps |
| LowDegree.lean | Specialized API for low-degree homology: provides isomorphisms chainsIsoₙ relating (inhomogeneousChains A).X n to concrete finsupps (A for n=0, G →₀ A for n=1, G² →₀ A for n=2), defines explicit differentials d₁₀, d₂₁, d₃₂ with computational lemmas, establishes H0Iso: H₀(G, A) ≅ A_G (coinvariants), defines cycles₁, cycles₂ and epimorphisms H1π, H2π to homology, proves H₁(G, A) ≃+ Gᵃᵇ ⊗ A when A is trivial representation (45KB file with extensive low-degree machinery) |
| Shapiro.lean | Shapiro's lemma for group homology: proves Hₙ(G, Ind_S^G(A)) ≅ Hₙ(S, A) for subgroup S ≤ G and S-representation A, uses fact that restriction functor Res(S) preserves projectives (since coinduction Coind_S^G preserves epis and is right adjoint), establishes coinvariantsTensorResProjectiveResolutionIso: (A ⊗ Res(S)(P))_S ≅ (Ind_S^G(A) ⊗ P)_G, applies to any projective resolution P of trivial representation |

## Subdirectories

(none)

## Search Tags

group-homology homological-algebra representation-theory k-linear-representations inhomogeneous-chains tor-functors left-derived-functors coinvariants projective-resolutions bar-resolution functoriality finite-cyclic-groups periodic-resolutions long-exact-sequences connecting-homomorphism shapiro-lemma induced-representations corestriction coinflation low-degree-homology abelianization tensor-products normal-subgroups quotient-groups exact-sequences
