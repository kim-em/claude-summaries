---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Homology/Embedding
generated: 2025-12-02T08:30:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 16
subdirs_count: 0
---

# Embedding

## Overview

The `Embedding/` directory provides a comprehensive framework for embeddings between complex shapes in homological algebra. It defines how one complex shape can be embedded into another via injective maps that preserve the differential relations, enabling operations like extending complexes (padding with zeros), restricting complexes (projecting onto subindices), and canonical truncations (both "greater than or equal" and "less than or equal"). These constructions are essential for relating complexes with different index types (e.g., ℕ-indexed to ℤ-indexed chain complexes) and for implementing truncation functors that create subcomplexes supported in certain degree ranges while preserving homological information.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `ComplexShape.Embedding c c'` as an injective map `f : ι → ι'` preserving differential relations, with type classes `IsRelIff` (relation equivalence), `IsTruncGE`/`IsTruncLE` (truncation conditions), and standard embeddings like `embeddingUpNat : up ℕ → up ℤ` and `embeddingUpIntGE p : up ℕ → up ℤ` (sends `n` to `p + n`) |
| Extend.lean | Extension functor `extendFunctor C : HomologicalComplex C c ⥤ HomologicalComplex C c'` that embeds complexes by padding with zero objects outside the image of the embedding map, with morphism `extendMap φ e` preserving chain maps and opposite complex constructions |
| Restriction.lean | Restriction functor `restrictionFunctor C : HomologicalComplex C c' ⥤ HomologicalComplex C c` (requires `e.IsRelIff`) that projects complexes onto the image of the embedding, dual to extension |
| TruncGE.lean | Canonical "≥" truncation functors `truncGE'Functor` and `truncGEFunctor` (requires `e.IsTruncGE`): replaces complex entries below the embedding range with opcycles (cokernels of incoming differentials), creating subcomplexes supported on `≥` degrees with epimorphism `πTruncGE : K ⟶ K.truncGE e` |
| TruncLE.lean | Canonical "≤" truncation functors `truncLE'Functor` and `truncLEFunctor` (requires `e.IsTruncLE`): dual to TruncGE, replaces entries above the range with cycles (kernels of outgoing differentials), with monomorphism `ιTruncLE : K.truncLE e ⟶ K` |
| TruncGEHomology.lean | Homology computations for `truncGE` truncations, proving quasi-isomorphism properties |
| TruncLEHomology.lean | Homology computations for `truncLE` truncations, proving quasi-isomorphism properties |
| StupidTrunc.lean | "Stupid truncation" functor as composition `restrictionFunctor ∘ extendFunctor`, simplest truncation that doesn't preserve homology |
| CochainComplex.lean | Specialized truncation abbreviations for ℤ-indexed cochain complexes: `truncLE n`, `truncGE n`, conditions `IsStrictlyGE n`/`IsStrictlyLE n` (strict support bounds), `IsGE n`/`IsLE n` (cohomological bounds via exactness), with short exact sequence constructions and shift compatibility |
| AreComplementary.lean | Complementary embeddings `e₁.AreComplementary e₂` when image ranges partition the target index set, with quasi-isomorphism `shortComplexTruncLEX₃ToTruncGE` relating cokernel of `ιTruncLE` to `truncGE` |
| Connect.lean | Connecting chain complexes and cochain complexes: given `K : ChainComplex C ℕ`, `L : CochainComplex C ℕ`, and connecting map `d₀ : K.X 0 ⟶ L.X 0`, constructs ℤ-indexed cochain complex `... ⟶ K.X 1 ⟶ K.X 0 ⟶ L.X 0 ⟶ L.X 1 ⟶ ...` with homology isomorphisms at positive/negative degrees |
| Boundary.lean | Boundary conditions for embeddings and truncations |
| HomEquiv.lean | Equivalences between Hom-sets for embedded/restricted complexes |
| IsSupported.lean | Support conditions for complexes relative to embeddings |
| ExtendHomology.lean | Homology behavior of the extend functor |
| RestrictionHomology.lean | Homology behavior of the restriction functor |

## Subdirectories

(No subdirectories)

## Search Tags

complex-shape embedding homological-complex truncation extension restriction functor chain-complex cochain-complex degree-bound support quasi-isomorphism natural-transformation index-type cokernel kernel cycles opcycles strict-support cohomological-bound complementary-embedding connecting-morphism
