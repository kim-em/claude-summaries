---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/Finsupp
generated: 2026-01-25T23:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 8
subdirs_count: 0
---

# Finsupp

## Overview

The `Finsupp/` directory contains the linear algebra theory for finitely supported functions (`α →₀ M`), which are functions from a type `α` to an `R`-module `M` that are zero at all but finitely many points. This is a fundamental construction in linear algebra, providing the bridge between abstract modules and concrete coordinate representations. The directory covers linear map versions of finsupp operations (lsingle, lapply, lsum), linear combinations and their bilinear variants, supported submodules and restriction operations, basis constructions from finsupp, equivalences with pi types and product types, vector space dimension theory, and linear independence results.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core linear map definitions for finsupp: lsingle (embedding single elements), lapply (evaluation at a point), lsubtypeDomain (restriction to subtype), restrictDom (filter as linear map), lmapDomain (domain mapping), linearEquivFunOnFinite (equivalence α →₀ M ≃ₗ α → M for finite α), and extensionality lemmas (lhom_ext, lhom_ext') |
| LSum.lean | lsum as linear map: Finsupp.lsum constructs linear maps (α →₀ M) →ₗ[R] N from families of linear maps (∀ a, M →ₗ[R] N), generalizing sum operations with semilinear variants and composition properties |
| LinearCombination.lean | Linear combination framework: linearCombination R v sends l : ι →₀ R to Σᵢ (l i) • (v i), with restricted version linearCombinationOn for supported subsets, bilinear variants (bilinearCombination for commutative scalar action), and Fintype.linearCombination for finite types with function domains |
| Supported.lean | Supported submodules: Finsupp.supported R M s is the submodule of functions with support contained in s, with restrictDom as linear map to supported submodules, supportedEquivFinsupp equivalence between (α →₀ M) supported on s and (s →₀ M), domLCongr for domain equivalences, and congr for equivalent support sets |
| Span.lean | Span relationships for finsupp linear maps: kernel/range results (ker_lsingle is trivial, lsingle_range_le_ker_lapply for disjoint sets, iSup_lsingle_range = ⊤, iInf_ker_lapply_le_bot), establishing that lsingle and lapply form dual operations with respect to suprema/infima of ranges/kernels |
| VectorSpace.lean | Basis and free module structure: Finsupp.basis constructs bases on ι →₀ M from families of bases on M, DFinsupp.basis for dependent versions, linearIndependent_single for linear independence of single-element embeddings, and Module.Free.dfinsupp showing direct sums of free modules are free |
| Pi.lean | Pi type equivalences for finite types: LinearEquiv.finsuppUnique (equivalence (α →₀ M) ≃ₗ M when α is singleton), FunOnFinite.map and FunOnFinite.linearMap for functoriality of finite function spaces under domain morphisms |
| SumProd.lean | Sum and product type equivalences: sumFinsuppLEquivProdFinsupp giving (α ⊕ β →₀ M) ≃ₗ (α →₀ M) × (β →₀ M), and sigmaFinsuppLEquivPiFinsupp giving ((Σ j, ιs j) →₀ M) ≃ₗ (j : η) → (ιs j →₀ M) for finite η, with explicit formulas for components |

## Subdirectories

(none)

## Search Tags

finsupp finitely-supported-functions linear-combinations basis free-modules linear-maps lsingle lapply lsum supported-submodules vector-spaces pi-types product-types sum-types equivalences linear-independence span kernel range semilinear bilinear-combinations
