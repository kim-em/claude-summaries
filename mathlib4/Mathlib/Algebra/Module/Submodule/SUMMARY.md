---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Module/Submodule
generated: 2025-12-01T17:55:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 16
subdirs_count: 0
---

# Submodule

## Overview

The `Submodule/` directory contains the comprehensive theory of submodules: subsets of modules that are closed under addition, scalar multiplication, and contain zero. This includes the core `Submodule R M` structure definition with its `SetLike` interface, the complete lattice structure on submodules (with `⊥ = {0}` and lattice operations via set intersection/span), fundamental operations on submodules (kernel, range, image, preimage of linear maps), equivalences and linear maps involving submodules, pointwise operations (negation, scalar actions), specialized submodules (equality locus, invariant submodules under endomorphisms), and results about unions of submodules over fields.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core `Submodule R M` structure: subset of module closed under addition, scalar multiplication, zero; extends `AddSubmonoid` and `SubMulAction`, includes `Subspace k M` abbreviation for field case |
| Basic.lean | Extended submodule theory: monotonicity, sum operations, central scalar actions, `NoZeroSMulDivisors` instance, additive actions by submodules |
| Lattice.lean | Complete lattice structure on submodules: `⊥ = {0}`, `⊓` as intersection, `⊔` and `⨆` via span, `CompleteLattice` instance, lattice homomorphisms |
| Map.lean | Pushforward `map f p` and pullback `comap f p` operations for submodules under linear maps, Galois insertion/coinsertion properties for surjective/injective maps |
| Ker.lean | Kernel of linear map: `LinearMap.ker f` defined as `comap f ⊥`, characterization as `{x | f x = 0}`, basic kernel properties |
| Range.lean | Range of linear map: `LinearMap.range f` as submodule, characterization as `map f ⊤`, range properties and composition results |
| LinearMap.lean | Linear maps involving submodules: `Submodule.subtype` embedding, `LinearMap.domRestrict`, `LinearMap.restrict`, `Submodule.inclusion` for submodule inclusions |
| Equiv.lean | Linear equivalences between submodules: `LinearEquiv.ofEq` for equal submodules, `ofSubmodules` for mapped submodules, `ofSubmodule'` for preimages |
| Pointwise.lean | Pointwise operations on submodules: negation `Submodule.pointwiseNeg`, `DistribMulAction` and `MulActionWithZero` instances, set actions on submodules |
| Bilinear.lean | Images of submodule pairs under bilinear maps: `Submodule.map₂ f p q` for bilinear `f`, characterization as span of `Set.image2` |
| EqLocus.lean | Equality locus submodule: `LinearMap.eqLocus f g = {x | f x = g x}` as submodule where two linear maps agree |
| Invariant.lean | Invariant submodules under endomorphisms: `Module.End.invtSubmodule f` as sublattice of `f`-invariant submodules (satisfying `p ≤ p.comap f`) |
| IterateMapComap.lean | Iterated map/comap operations: `LinearMap.iterateMapComap f i n K` for establishing strong rank condition in Noetherian rings, non-decreasing sequence properties |
| RestrictScalars.lean | Restriction of scalars: `Submodule.restrictScalars S V` converts `R`-submodule to `S`-submodule when `S` acts on `R` compatibly |
| Union.lean | Union results for submodules: `Submodule.iUnion_ssubset_of_forall_ne_top_of_card_lt` showing finite union of proper submodules over large field is proper |
| Order.lean | Ordered instances on submodules: `IsOrderedAddMonoid` and `IsOrderedCancelAddMonoid` instances for submodules of ordered modules |

## Subdirectories

*No subdirectories*

## Search Tags

submodule subspace lattice-structure map comap kernel range linear-map bilinear-map galois-insertion pointwise-operations equality-locus invariant-submodule restrict-scalars ordered-submodule union-bound
