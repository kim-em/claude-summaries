---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/Cyclotomic
generated: 2026-01-25T22:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 9
subdirs_count: 0
---

# Cyclotomic

## Overview

The `Cyclotomic/` directory contains the theory of cyclotomic field extensions—extensions obtained by adjoining primitive roots of unity. It defines the general class `IsCyclotomicExtension S A B` for ring extensions obtained by adding `n`-th primitive roots for `n ∈ S`, along with specialized constructions `CyclotomicField n K` (splitting field of the `n`-th cyclotomic polynomial) and `CyclotomicRing n A K` (integral closure). The directory includes structural results (finiteness, Galois theory, power bases), arithmetic invariants (discriminants, norms), and the cyclotomic character mapping field automorphisms to units in `ZMod n` or `ℤₚ`.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of `IsCyclotomicExtension S A B`, proving it's closed under composition, generates number fields when finite, and provides splitting field characterizations |
| PrimitiveRoots.lean | Defines canonical primitive root `zeta n A B`, proves dimension equals totient, computes norms of primitive roots and their powers, establishes equivalence between embeddings and primitive roots |
| CyclotomicCharacter.lean | Defines cyclotomic character as group homomorphism `(L ≃+* L) →* (ZMod n)ˣ` and p-adic version `(L ≃+* L) →* ℤ_[p]ˣ` measuring how automorphisms permute roots of unity |
| Discriminant.lean | Computes discriminants of cyclotomic field power bases, proving `discr = (-1)^((p^(k+1)).totient/2) * p^(p^k * ((p-1)*(k+1)-1))` for prime powers |
| Gal.lean | Proves Galois group of `K(ζₙ)` is isomorphic to `(ZMod n)ˣ` when the `n`-th cyclotomic polynomial is irreducible, shows cyclotomic extensions are abelian |
| Embeddings.lean | Deprecated module (since 2025-10-14) importing unrelated components (matroids, Bochner integration, arithmetic functions, positivity tactic) |
| PID.lean | Deprecated module (since 2025-10-14) importing gamma functions, category theory, matroids, double factorials, arithmetic functions |
| Rat.lean | Deprecated module (since 2025-10-14) with same imports as PID.lean |
| Three.lean | Deprecated module (since 2025-10-14) with same imports as PID.lean and Rat.lean |

## Subdirectories

(No subdirectories)

## Search Tags

cyclotomic-fields cyclotomic-extensions primitive-roots roots-of-unity galois-group cyclotomic-polynomial discriminant cyclotomic-character number-fields splitting-fields power-basis totient zeta irreducible-cyclotomic abelian-extensions primitive-root-norm field-automorphisms algebraic-extensions
