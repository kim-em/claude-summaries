---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Finset/Lattice
generated: 2025-12-09T12:00:00Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: complete
files_count: 6
subdirs_count: 0
---

# Lattice

## Overview

The `Lattice/` subdirectory provides lattice-theoretic operations on finsets, focusing on supremum (`sup`) and infimum (`inf`) folding operations. While `Basic.lean` defines the fundamental lattice structure on `Finset α` itself (using union as `⊔` and intersection as `⊓`), this directory extends to folding lattice operations *over* finset elements. The `Fold.lean` file is the centerpiece, defining `sup` and `inf` functions that fold a binary lattice operation over all elements of a finset, mapping each element through a function and combining results. These operations are then specialized for product types, dependent products (Pi types), and interact with `biUnion`.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core lattice structure on `Finset α`: defines `Union`, `Inter`, and proves `Finset α` is a distributive lattice with union as `⊔` and intersection as `⊓`; fundamental lemmas on union and intersection |
| Fold.lean | Supremum/infimum folding over finsets: defines `Finset.sup` and `Finset.inf` to fold lattice operations (e.g., `s.sup f` computes `f a₁ ⊔ f a₂ ⊔ ... ⊔ ⊥`); includes bounded versions `sup'`/`inf'` for semilattices without bot/top; distribution laws, monotonicity, induction principles |
| Lemmas.lean | Additional lemmas about lattice operations on finsets: interaction between insert, union, intersection; singleton intersections; union and intersection properties with membership conditions |
| Pi.lean | Lattice operations on finsets of dependent functions (Pi types): key theorem `inf_sup` relates nested inf-sup to a single operation over the Pi product `s.pi t` |
| Prod.lean | Lattice operations on finsets of product types: `sup_product_left`/`sup_product_right` decompose supremum over Cartesian products; `sup_inf_sup` distributes sup and inf over products |
| Union.lean | Relationship between `Finset.biUnion` and lattice operations: shows `sup_biUnion` and proves `sup_eq_biUnion` (supremum of finsets equals their biUnion when `DecidableEq`) |

## Subdirectories

*(No subdirectories)*

## Search Tags

lattice finset supremum infimum sup inf fold union intersection distributive-lattice semilattice bounded-lattice product-types pi-types dependent-functions biUnion lattice-homomorphism order-theory
