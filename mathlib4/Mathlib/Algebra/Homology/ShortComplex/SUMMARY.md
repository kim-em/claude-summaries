---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Homology/ShortComplex
generated: 2025-12-02T08:30:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 20
subdirs_count: 0
---

# ShortComplex

## Overview

The `ShortComplex/` directory provides the foundational theory for short complexes in category theory: diagrams of the form `X₁ → X₂ → X₃` with composable morphisms `f : X₁ → X₂` and `g : X₂ → X₃` satisfying `f ≫ g = 0`. This structure is fundamental to homological algebra, serving as the basic building block for more complex constructions. The directory implements the category structure on short complexes, develops dual notions of left and right homology data that provide compatible descriptions of homology objects, establishes exactness characterizations (when homology vanishes), proves the snake lemma for extracting long exact sequences from commutative diagrams, and provides specialized theory for preadditive and abelian categories where all short complexes have homology.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `ShortComplex C` structure with three objects `X₁, X₂, X₃` and morphisms `f, g` satisfying `f ≫ g = 0`; category structure with morphisms as commutative diagrams; projection functors `π₁, π₂, π₃`; natural transformations `π₁Toπ₂` and `π₂Toπ₃`; functor `F.mapShortComplex` for lifting functors; opposite category constructions |
| Homology.lean | Central definition of `HomologyData` combining compatible left and right homology data via isomorphism `left.H ≅ right.H` with pentagon commutative diagram; `HasHomology` typeclass; constructors for homology data from kernels/cokernels; homology map data for morphisms; homology of single-degree complexes (54KB) |
| LeftHomology.lean | Left homology data: objects `K` (kernel of `g`) and `H` (homology), morphisms `i : K → X₂` (kernel inclusion), `π : K → H` (projection to homology), `f' : X₁ → K` (lift of `f`); verification that `H` is cokernel of `f'`; dual to right homology using kernel-first approach (45KB) |
| RightHomology.lean | Right homology data: objects `Q` (cokernel of `f`) and `H` (homology), morphisms `p : X₂ → Q` (projection), `ι : H → Q` (homology inclusion), `g' : Q → X₃` (descent of `g`); verification that `H` is kernel of `g'`; dual to left homology using cokernel-first approach (56KB) |
| Exact.lean | Exactness predicate `S.Exact` defined as existence of homology data with zero homology object `IsZero h.left.H`; equivalences to vanishing of left/right homology; preservation under isomorphisms; exactness of special cases (zero maps, isomorphic middle object); characterizations via `i ≫ p = 0` condition (36KB) |
| ShortExact.lean | Short exact sequences: `ShortExact` structure combining exactness with `Mono f` and `Epi g`; characterizations showing `X₁` is kernel of `g` and `X₃` is cokernel of `f` in balanced categories; five-lemma type results; splitting of short exact sequences when `X₁` is injective or `X₃` is projective |
| SnakeLemma.lean | Snake lemma: `SnakeInput C` structure encoding commutative ladder diagram with exact rows where `L₀ → L₁ → L₂ → L₃` are morphisms of short complexes with `L₀` kernel and `L₃` cokernel of `L₁ → L₂`; construction of connecting homomorphism `δ : L₀.X₃ → L₃.X₁`; proof of 6-term exact sequence extendable to 9-term with zeros under additional assumptions (24KB) |
| QuasiIso.lean | Quasi-isomorphisms: `QuasiIso φ` typeclass for morphisms `φ : S₁ → S₂` inducing isomorphism on homology `IsIso (homologyMap φ)`; closure under composition; characterizations via left/right homology map data; dual properties under `opMap`; special cases for zero maps |
| Preadditive.lean | Preadditive structure on `ShortComplex C` when `C` is preadditive: componentwise addition/negation/subtraction on morphisms; `AddCommGroup` instance for hom-sets; compatibility of homology maps with preadditive structure; homology functor is additive (28KB) |
| Abelian.lean | Proof that all short complexes in abelian categories have homology: canonical `LeftHomologyData.ofAbelian` using coimage of `kernel.ι g ≫ cokernel.π f`; canonical `RightHomologyData.ofAbelian` using image of same morphism; compatibility via coimage-image isomorphism; `HasHomology` instance for abelian categories |
| Ab.lean | Short complexes in category of abelian groups `Ab`: concrete computations of homology as quotient `ker(g)/im(f)` using abelian group quotients; explicit element-wise characterizations of exactness |
| ModuleCat.lean | Short complexes in categories of modules `ModuleCat R`: similar concrete homology computations; exactness characterized by `im(f) = ker(g)` at element level; linear algebra perspective on homological algebra |
| Linear.lean | Linear/module structure on short complex categories when underlying category has such structure; homology functors preserve linearity |
| HomologicalComplex.lean | Relationship between short complexes and general homological complexes: extracting short complexes from homological complexes at specific degrees; embedding short complexes into full homological complexes; comparisons of homology theories (32KB) |
| PreservesHomology.lean | Functors preserving homology: `PreservesLeftHomologyOf`, `PreservesRightHomologyOf`, `PreservesHomologyOf` typeclasses; conditions for preservation; examples of homology-preserving functors; preservation of exactness under such functors (40KB) |
| ExactFunctor.lean | Exact functors between short complex categories: functors preserving exactness; left exact functors (preserve kernels); right exact functors (preserve cokernels); characterizations via preservation of homology data |
| Limits.lean | Limits and colimits in categories of short complexes: constructed componentwise from limits/colimits in underlying category; preservation by projection functors; kernels and cokernels of morphisms between short complexes |
| ConcreteCategory.lean | Concrete category structure for `ShortComplex C` when `C` is concrete: forgetful functors; faithful functors; element-wise reasoning when applicable |
| FunctorEquivalence.lean | Equivalences between categories of short complexes induced by equivalences of underlying categories; transport of homology data along equivalences |
| Retract.lean | Retract diagrams for short complexes: when one short complex is a retract of another; implications for homology and exactness |

## Subdirectories

(none)

## Search Tags

short-complex homology homological-algebra exact-sequence kernel cokernel cycles opcycles left-homology right-homology homology-data snake-lemma connecting-homomorphism quasi-isomorphism abelian-category preadditive short-exact five-lemma image coimage balanced-category functorial-homology

