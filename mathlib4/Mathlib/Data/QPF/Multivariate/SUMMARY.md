---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/QPF/Multivariate
generated: 2025-12-11T18:15:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 1
subdirs_count: 1
---

# Multivariate

## Overview

Multivariate Quotients of Polynomial Functors (MvQPF) operating on type vectors (`TypeVec n → Type`). This module defines the `MvQPF` class, which generalizes polynomial functors by allowing quotienting, enabling the construction of inductive and coinductive types that Lean cannot natively express. Examples include unordered trees (trees with multiset children) and coinductive types nested inside quotients. The theory is based on "Data Types as Quotients of Polynomial Functors" by Avigad, Carneiro, and Hudon.

The core abstraction uses `abs`/`repr` functions to relate QPFs to their underlying polynomial functor representations. Every MvQPF is proven to be a lawful functor, with lifting lemmas for predicates (`LiftP`) and relations (`LiftR`), and uniformity properties (`IsUniform`, `LiftPPreservation`, `SuppPreservation`).

The Constructions subfolder provides the essential building blocks: `Fix` for initial algebras (inductive types), `Cofix` for final coalgebras (coinductive types with bisimulation principles), `Comp` for functor composition, `Quot` for taking quotients, `Sigma`/`Pi` for dependent sums and products, `Prj` for projection functors, and `Const` for constant functors. Together these enable expressing complex recursive and corecursive data structures.

## Key Files

| File | Purpose |
|------|---------|
| `Basic.lean` | Defines the `MvQPF` class with `abs`/`repr` abstraction-representation functions, proves every MvQPF is a lawful functor, provides lifting lemmas for predicates (`LiftP`) and relations (`LiftR`), defines uniformity properties (`IsUniform`, `LiftPPreservation`, `SuppPreservation`), and shows every `MvPFunctor` is trivially an `MvQPF` |

## Subdirectories

- [x] `Constructions/` - QPF-preserving constructions: Fix (initial algebra), Cofix (final coalgebra/coinductive types), Comp (functor composition), Quot (quotients), Sigma, Prj (projection), and Const (constant functors)

## Search Tags

mvqpf multivariate-qpf quotient-polynomial-functor type-vector functor-abstraction abs repr liftP liftR supp uniform lawful-functor inductive coinductive initial-algebra final-coalgebra fix cofix w-type m-type bisimulation corec recursor composition sigma pi quotient
