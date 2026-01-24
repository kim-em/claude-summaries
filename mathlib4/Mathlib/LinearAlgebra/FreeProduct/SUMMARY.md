---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/LinearAlgebra/FreeProduct
generated: 2026-01-25T08:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# FreeProduct

## Overview

The `FreeProduct/` directory contains the formalization of free products of R-algebras, which generalizes the tensor product to the non-commutative setting. The free product is defined as a quotient of the tensor algebra on the direct sum of algebras, modulo relations that preserve multiplication within each component and identify all unit elements. The main result is the universal property establishing the free product as the coproduct in the category of general R-algebras.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Free product construction and universal property: defines `FreeProduct R A` as quotient of tensor algebra on `⨁ i, A i` by relation identifying `aᵢ ⊗ aᵢ' ~ aᵢaᵢ'` and `1ᵢ ~ 1ⱼ`, establishes equivalence with power algebra representation (`asPowersEquiv`), provides canonical injections (`ι i : A i →ₐ[R] FreeProduct R A`), and proves universal property (`lift` establishes equivalence between families of maps `{i : I} → A i →ₐ[R] B` and maps `FreeProduct R A →ₐ[R] B`) |

## Subdirectories

No subdirectories.

## Search Tags

free-product coproduct non-commutative algebras tensor-algebra quotient universal-property category-theory algebra-homomorphisms direct-sum
