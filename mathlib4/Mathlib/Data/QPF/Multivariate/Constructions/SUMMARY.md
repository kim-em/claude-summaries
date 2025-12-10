---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/QPF/Multivariate/Constructions
generated: 2025-12-11T11:20:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: complete
files_count: 7
subdirs_count: 0
---

# Constructions

## Overview

QPF-preserving constructions for multivariate quotients of polynomial functors. This folder provides the key building blocks for constructing inductive and coinductive types: fixed points (Fix for initial algebras, Cofix for final coalgebras/coinductive types), functor composition, quotients, dependent sums/products, projections, and constant functors. Together these enable expressing complex recursive and corecursive data structures that Lean cannot natively represent.

## Key Files

| File | Purpose |
|------|---------|
| `Fix.lean` | Initial algebra (least fixed point) of an (n+1)-ary QPF. Defines `Fix F` which satisfies `Fix F α = F α (Fix F α)`. Provides constructor `mk`, destructor `dest`, recursor `rec`, dependent recursor `drec`, and induction principle `ind`. Uses W-types with `WEquiv` quotient. |
| `Cofix.lean` | Final coalgebra (greatest fixed point/coinductive types) of an (n+1)-ary QPF. Defines `Cofix F` with constructor `mk`, destructor `dest`, corecursor `corec` (and variants `corec'`, `corec₁`), and bisimulation principles (`bisim`, `bisim_rel`, `bisim₂`, `bisim'`). Uses M-types with `Mcongr` quotient. Includes `mv_bisim` tactic. |
| `Comp.lean` | Functor composition: composing an n-ary functor F with n m-ary functors G gives an m-ary QPF. Defines `Comp F G` with constructor/destructor and proves it preserves QPF structure. |
| `Const.lean` | Constant functor that ignores its type arguments. `Const n A` maps any n-ary type vector to `A`. Useful for embedding non-functorial types into QPF specifications. |
| `Prj.lean` | Projection functor. `Prj i` is an n-ary functor returning the i-th component of the type vector. Provides polynomial representation using `PUnit` and equality proofs. |
| `Quot.lean` | Quotients of QPFs. Provides `quotientQPF` for transporting QPF structure across surjective functions, and `Quot1`/`relQuot` for taking quotients by equivalence relations that respect the functor structure. |
| `Sigma.lean` | Dependent sum (`Sigma F`) and dependent product (`Pi F`) of QPFs indexed by a type `A`. Both preserve QPF structure, enabling indexed families of functors. |

## Subdirectories

*(none)*

## Search Tags

mvqpf fix cofix initial-algebra final-coalgebra coinductive w-type m-type wequiv mcongr bisimulation corec recursor composition const constant-functor projection sigma pi dependent-sum dependent-product quotient functor-composition mv_bisim tactic
