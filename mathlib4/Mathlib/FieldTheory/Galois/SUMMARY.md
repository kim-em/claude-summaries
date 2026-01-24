---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/FieldTheory/Galois
generated: 2026-01-24T23:45:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 8
subdirs_count: 0
---

# Galois

## Overview

This directory contains the core formalization of Galois theory in Mathlib. It defines Galois extensions as field extensions that are both separable and normal, establishes the fundamental theorem of Galois theory (the Galois correspondence between intermediate fields and subgroups of the Galois group), and extends this to infinite Galois extensions via profinite topology. The directory also includes results on abelian extensions, Galois closures, the normal basis theorem, and the `IsGaloisGroup` predicate for general group actions on field extensions.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core Galois theory: defines `IsGalois F E` (separable + normal), `fixedField`/`fixingSubgroup` operations, the Galois correspondence `intermediateFieldEquivSubgroup` for finite extensions, and proves key results like `card_aut_eq_finrank` (|Gal(E/F)| = [E:F]) |
| Notation.lean | Provides the `Gal(L/K)` notation for the Galois group `L ≃ₐ[K] L`, including a custom pretty printer that displays this notation when both types are fields |
| Abelian.lean | Defines `IsAbelianGalois K L` for Galois extensions with commutative Galois group; proves tower properties and that cyclic Galois groups yield abelian extensions |
| GaloisClosure.lean | Defines `FiniteGaloisIntermediateField` - the type of intermediate fields that are finite and Galois over the base; provides lattice structure and the `adjoin` construction for creating minimal Galois intermediate fields |
| Infinite.lean | Fundamental theorem of infinite Galois theory: extends the Galois correspondence to arbitrary (not necessarily finite) Galois extensions using closed subgroups in the Krull topology; proves `IntermediateFieldEquivClosedSubgroup` |
| Profinite.lean | Realizes `Gal(K/k)` as a profinite group: constructs the inverse limit over finite Galois intermediate fields and proves `continuousMulEquivToLimit` giving a topological group isomorphism |
| IsGaloisGroup.lean | General predicate `IsGaloisGroup G K L` for when a group G acts faithfully on L with fixed field K; useful in algebraic number theory for actions on rings of integers |
| NormalBasis.lean | Proves the normal basis theorem: every finite Galois extension has a basis that is an orbit under the Galois group action; constructs `IsGalois.normalBasis` |

## Subdirectories

(none)

## Search Tags

galois-theory galois-extensions galois-group galois-correspondence fundamental-theorem fixed-field fixing-subgroup separable normal field-extensions intermediate-fields profinite krull-topology infinite-galois abelian-extensions galois-closure normal-basis finite-galois algebraic-number-theory
