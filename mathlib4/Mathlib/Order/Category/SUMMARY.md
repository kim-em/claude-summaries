---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/Category
generated: 2026-01-25T23:13:00Z
git_sha: ffb766c85c7ad82861131c2f10a0669884e4fd5f
git_branch: HEAD
status: complete
files_count: 19
subdirs_count: 0
---

# Category

## Overview

The `Category/` directory provides the categorical interface for order theory, systematically organizing the various order-theoretic structures from `Mathlib/Order/` into concrete categories. Each file bundles a specific order type (preorders, partial orders, lattices, Boolean algebras, frames, etc.) into a category where objects are types equipped with the corresponding order structure and morphisms are the appropriate structure-preserving maps (monotone functions, lattice homomorphisms, frame homomorphisms, etc.). This spans the full hierarchy from basic preorders through complete Boolean algebras, including specialized categories for finite orders, linear orders, omega-complete partial orders, and Heyting algebras. The NonemptyFinLinOrd category serves as the standard index category for simplicial objects in algebraic topology, while ωCPO provides the categorical foundation for programming language semantics.

## Key Files

| File | Purpose |
|------|---------|
| Preord.lean | Category of preorders with monotone maps as morphisms; foundational category for order theory |
| PartOrd.lean | Category of partial orders with monotone maps (OrderHom); includes antisymmetrization and adjunctions |
| PartOrdEmb.lean | Category of partial orders with order embeddings as morphisms (not just homomorphisms); includes filtered colimit constructions |
| LinOrd.lean | Category of linear orders with monotone maps |
| NonemptyFinLinOrd.lean | Category of nonempty finite linear orders; index category for simplicial objects; includes BoundedOrder instances |
| FinPartOrd.lean | Category of finite partial orders with monotone maps |
| Lat.lean | Category of lattices with lattice homomorphisms; note: doesn't require bounds (differs from nLab Lat definition which is BddLat) |
| Semilat.lean | Category of semilattices with semilattice homomorphisms |
| BddOrd.lean | Category of bounded orders (partial orders with top and bottom) with monotone functions |
| BddLat.lean | Category of bounded lattices with bounded lattice homomorphisms |
| BddDistLat.lean | Category of bounded distributive lattices |
| DistLat.lean | Category of distributive lattices |
| FinBddDistLat.lean | Category of finite bounded distributive lattices |
| CompleteLat.lean | Category of complete lattices with complete lattice homomorphisms (preserve arbitrary sups and infs) |
| BoolAlg.lean | Category of Boolean algebras with bounded lattice homomorphisms |
| FinBoolAlg.lean | Category of finite Boolean algebras |
| HeytAlg.lean | Category of Heyting algebras with Heyting homomorphisms |
| Frm.lean | Category of frames (complete lattices where meet distributes over arbitrary joins) with frame homomorphisms |
| OmegaCompletePartialOrder.lean | Category ωCPO of omega-complete partial orders with continuous homomorphisms; includes product and equalizer constructions |

## Subdirectories

(No subdirectories)

## Search Tags

category-theory concrete-category preorder partial-order linear-order lattice bounded-lattice distributive-lattice Boolean-algebra Heyting-algebra frame complete-lattice omega-cpo order-homomorphism order-embedding monotone-map simplicial finite-order
