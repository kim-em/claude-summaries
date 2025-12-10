---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/QPF
generated: 2025-12-11T08:30:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: preliminary
files_count: 0
subdirs_count: 2
---

# QPF

## Overview

Quotients of Polynomial Functors (QPFs) provide a compositional framework for defining inductive and coinductive types, their quotients, and nesting. QPFs generalize polynomial functors by allowing quotienting, enabling the construction of data types that Lean cannot natively express, such as unordered trees (trees with multisets of children) or coinductive types nested inside quotients. The theory is based on the paper "Data Types as Quotients of Polynomial Functors" by Avigad, Carneiro, and Hudon.

## Key Files

| File | Purpose |
|------|---------|
| (no files directly in this folder) | |

## Subdirectories

- [ ] `Multivariate/` - Multivariate QPFs operating on type vectors (TypeVec n -> Type); defines MvQPF class and provides constructions for Fix, Cofix, Comp, Quot, Sigma, Prj, and Const
- [ ] `Univariate/` - Univariate QPFs operating on single types (Type -> Type); defines QPF class with Fix (initial algebra), Cofix (final coalgebra), composition, and quotient constructions

## Search Tags

qpf quotient-polynomial-functor inductive coinductive initial-algebra final-coalgebra fix cofix functor-composition quotient-types data-types categorical
