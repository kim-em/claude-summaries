---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/GroupTheory/Coxeter
generated: 2026-01-24T23:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 4
subdirs_count: 0
---

# Coxeter

## Overview

The `Coxeter/` directory provides a comprehensive formalization of Coxeter groups and Coxeter systems, fundamental objects in geometric group theory and Lie theory. A Coxeter matrix `M : Matrix B B ℕ` is symmetric with diagonal entries 1 and off-diagonal entries ≠ 1 (where 0 represents ∞ in the literature). The associated Coxeter group has presentation `⟨{sᵢ}ᵢ∈B | {(sᵢsⱼ)^Mᵢⱼ}ᵢ,ⱼ∈B⟩` where the `sᵢ` are simple reflections (involutions). A Coxeter system is a group `W` together with an isomorphism to some Coxeter group. The formalization includes the length function (minimum number of simple reflections needed to represent an element), reduced words, descent sets, reflections (conjugates of simple reflections), inversions, and inversion sequences. Standard Coxeter matrices from Lie theory (types A, B, D, E, F, G, H, I) are provided, corresponding to symmetry groups of regular polytopes and root systems. Key theorems include the braid relations (Artin-Tits relations), length function properties (triangle inequality, parity), and characterizations of descents and inversions.

## Key Files

| File | Purpose |
|------|---------|
| Matrix.lean | Coxeter matrices: definition (symmetric, diagonal=1, off-diagonal≠1), reindexing operation, standard types from Lie theory (Aₙ, Bₙ, Dₙ for infinite families; E₆, E₇, E₈, F₄, G₂, H₃, H₄, I₂ₘ for exceptional/sporadic types), with Coxeter-Dynkin diagrams in comments |
| Basic.lean | Core definitions: `CoxeterMatrix.Group` (group with Coxeter presentation via `PresentedGroup`), `CoxeterSystem` (records isomorphism `W ≃* M.Group`), `IsCoxeterGroup`, simple reflections, involution property (s²=1), Coxeter relations (sᵢsⱼ)^Mᵢⱼ=1, universal property `lift` (extend B→G to W→G for liftable functions), words and `wordProd`, `alternatingWord` and `braidWord`, braid relation theorem (alternating words have equal products), induction principles |
| Length.lean | Length function: `length w` (minimum word length representing w), existence of reduced words, length inequalities (ℓ(w₁w₂)≤ℓ(w₁)+ℓ(w₂), triangle inequalities), parity homomorphism `lengthParity : W →* Multiplicative (ZMod 2)`, length characterization for simples (ℓ(sᵢ)=1), length-one iff simple reflection, descents: `IsLeftDescent w i` (ℓ(sᵢw)<ℓ(w)), `IsRightDescent w i` (ℓ(wsᵢ)<ℓ(w)), descent characterizations (descent iff ℓ(sw)=ℓ(w)-1), reduced words (ℓ(π ω)=length ω), non-reduced alternating words beyond Coxeter matrix bound |
| Inversion.lean | Reflections: `IsReflection t` (t=wsᵢw⁻¹ for some w,i), involution (t²=1) and conjugation properties, odd length, inversions: `IsLeftInversion w t` (t reflection and ℓ(tw)<ℓ(w)), `IsRightInversion w t` (t reflection and ℓ(wt)<ℓ(w)), equivalence with descents for simple reflections, inversion sequences: `rightInvSeq ω` (sequence of conjugated simple reflections appearing in word), `leftInvSeq ω` (dual sequence), explicit formulas for nth element, relationship to reduced words, key theorem: reduced words have no duplicate inversions (`nodup_rightInvSeq`, `nodup_leftInvSeq`), product formulas and conjugation properties |

## Subdirectories

(No subdirectories)

## Search Tags

coxeter-group coxeter-system coxeter-matrix simple-reflection length-function reduced-word descent inversion reflection alternating-word braid-relation artin-tits-relation presentation matrix-type lie-theory weyl-group root-system geometric-group-theory polytope-symmetry cox
