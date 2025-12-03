---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Homology/HomotopyCategory
generated: 2025-12-02T10:00:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 14
subdirs_count: 0
---

# HomotopyCategory

## Overview

The `HomotopyCategory/` directory develops the homotopy category of cochain complexes, where homotopic chain maps are identified. It provides the pretriangulated and triangulated structure on the homotopy category via mapping cone constructions following Verdier's thesis, establishes the shift functors with sign conventions, and proves the homotopy category is a homological functor. The framework includes K-injective complexes, degreewise split sequences, homology computations on the homotopy category, and single functors for embedding objects as complexes concentrated in a single degree.

## Key Files

| File | Purpose |
|------|---------|
| HomComplex.lean | Cochain complex of homomorphisms between cochain complexes: defines `Cochain F G n` as families of morphisms `F.X p ⟶ G.X (p + n)` with differential operator δ satisfying δ² = 0, providing foundation for homotopy theory |
| HomComplexCohomology.lean | Cohomology of hom-complexes: identifies `H⁰(HomComplex F G)` with morphisms in homotopy category, relates higher cohomology to extension groups |
| HomComplexInduction.lean | Inductive constructions for hom-complexes |
| HomComplexShift.lean | Shift operations on hom-complexes compatible with shift on source and target complexes |
| MappingCone.lean | Mapping cone construction `mappingCone φ` for morphism `φ : F ⟶ G`: defines direct sum `F.X(i+1) ⊕ G.X(i)` with twisted differential, provides `inl`, `inr`, `fst`, `snd` structure maps, descent/ascent lemmas for universal properties |
| Pretriangulated.lean | Pretriangulated structure on homotopy category: distinguished triangles as images of standard triangles `K ⟶ L ⟶ mappingCone φ ⟶ K⟦1⟧`, rotation isomorphisms, octahedral axiom via composition of mapping cones, following Verdier's formalism with Conrad's sign conventions |
| Triangulated.lean | Triangulated structure proving homotopy category is triangulated: octahedral axiom via `mappingConeCompTriangle` for composable morphisms, establishing `HomotopyCategory C (ComplexShape.up ℤ)` as `IsTriangulated` instance |
| Shift.lean | Shift functors `shiftFunctor C n : CochainComplex C ℤ ⥤ CochainComplex C ℤ` sending `K` to `K⟦n⟧` with `(K⟦n⟧).X i = K.X (i+n)` and differentials multiplied by `(-1)^n`, proves `HasShift (HomotopyCategory C (ComplexShape.up ℤ)) ℤ` with compatibility isomorphisms |
| ShiftSequence.lean | Sequences of complexes related by shifts |
| HomologicalFunctor.lean | Homological functor property: proves `homologyFunctor C (ComplexShape.up ℤ) n` is a homological functor from homotopy category to `C` when `C` is abelian, using degreewise split short exact sequences |
| DegreewiseSplit.lean | Degreewise split short exact sequences of cochain complexes: characterizes distinguished triangles via split exact sequences in each degree, providing computational approach to triangulated structure |
| ShortExact.lean | Short exact sequences in homotopy category and their relation to degreewise exactness |
| KInjective.lean | K-injective complexes: complexes where `Hom(-, K)` is exact on acyclic complexes, dual notion to K-projective, important for deriving contravariant functors |
| SingleFunctors.lean | Single functors `C ⥤ CochainComplex C ℤ` and `C ⥤ HomotopyCategory C (ComplexShape.up ℤ)` sending object `X` to complex concentrated in degree `n`, with shift compatibility forming `SingleFunctors` structure |

## Subdirectories

(No subdirectories)

## Search Tags

homotopy-category cochain-complex chain-homotopy pretriangulated triangulated mapping-cone shift-functor homological-functor distinguished-triangle rotation-axiom octahedral-axiom K-injective degreewise-split single-functor verdier conrad sign-conventions homology-functor exact-sequence
