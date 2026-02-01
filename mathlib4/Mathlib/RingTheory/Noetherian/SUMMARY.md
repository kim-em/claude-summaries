---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Noetherian
generated: 2026-02-01T06:45:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 7
subdirs_count: 0
---

# Noetherian

## Overview

This directory contains the core theory of Noetherian rings and modules. A module is Noetherian if every submodule is finitely generated, equivalently if every ascending chain of submodules stabilizes (the ascending chain condition). A ring is Noetherian if it is Noetherian as a module over itself, meaning all ideals are finitely generated. The theory is developed for left-modules over possibly non-commutative rings, though most applications are to commutative algebra.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Core definitions: `IsNoetherian R M` class asserting all submodules are finitely generated; `IsNoetherianRing R` abbreviation; equivalence with well-foundedness of `>` on submodules and stabilization of ascending chains; results on submodules and kernel/range disjointness for endomorphisms |
| Basic.lean | Main theorems: Noetherian property preserved by surjections, quotients, products, finite pi-types, exact sequences; transfer across linear equivalences; finite modules over Noetherian rings are Noetherian; induction principle for Noetherian modules; linear independence implies finite index; products of Noetherian rings are Noetherian |
| Filter.lean | Chain stabilization result: `eventuallyConst_of_isNoetherian` proves ascending chains of submodules are eventually constant using filter-based formulation |
| Nilpotent.lean | Nilpotent ideal theory: proves the nilradical of a Noetherian ring is nilpotent (`IsNoetherianRing.isNilpotent_nilradical`); characterizes when finitely generated ideals are nilpotent |
| OfPrime.lean | Cohen's theorem: a ring is Noetherian if all prime ideals are finitely generated; uses Oka property (`Ideal.FG` is Oka); variant `of_prime_ne_bot` excluding the zero ideal |
| Orzech.lean | Orzech's theorem: surjective endomorphisms of Noetherian modules are injective (and hence bijective); if `M x N` embeds into `M` with `M` Noetherian then `N` is trivial; Noetherian rings satisfy the Orzech property |
| UniqueFactorizationDomain.lean | UFD connection: Noetherian integral domains are well-founded divisibility monoids (`WfDvdMonoid`), a key step toward showing Noetherian domains have unique factorization |

## Subdirectories

(none)

## Search Tags

Noetherian module ring ACC ascending-chain-condition finitely-generated submodule ideal well-founded IsNoetherian IsNoetherianRing Cohen-theorem Orzech-theorem nilradical nilpotent WfDvdMonoid UFD exact-sequence quotient product
