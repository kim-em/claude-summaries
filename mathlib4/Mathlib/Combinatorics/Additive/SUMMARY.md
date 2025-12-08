---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/Additive
generated: 2025-12-08T15:42:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: preliminary
files_count: 17
subdirs_count: 2
---

# Additive

## Overview

The `Additive/` directory contains formalized results in additive combinatorics, focusing on sumset theory, density results, and structural theorems for sets with small doubling or tripling. Key results include the Cauchy-Davenport theorem, Plünnecke-Ruzsa inequality, Erdős-Ginzburg-Ziv theorem, and Roth's theorem on 3-term arithmetic progressions. The directory provides tools for studying approximate subgroups, Freiman homomorphisms, additive energy, dissociation, and corner-free sets.

## Key Files

| File | Purpose |
|------|---------|
| ApproximateSubgroup.lean | Approximate subgroups: symmetric sets A where A² is covered by few translates of A; proves they share properties with genuine subgroups (closed under homomorphisms, bounded powers, connections to small tripling) |
| CauchyDavenport.lean | Cauchy-Davenport theorem: lower bound \|s + t\| ≥ \|s\| + \|t\| - 1 for sumsets in groups, with generalizations using e-transform technique for arbitrary groups and direct proof for linearly ordered groups |
| Convolution.lean | Convolution operations for finsets in additive combinatorics |
| CovBySMul.lean | Covering by scalar multiples: definition of sets that can be covered by finitely many translates |
| Dissociation.lean | Dissociation and span: sets where all finite subsets have different sums (analog of linear independence with coefficients restricted to 0, ±1) |
| DoublingConst.lean | Doubling and difference constants: σ[A, B] = \|A + B\| / \|A\| and δ[A, B] = \|A - B\| / \|A\|, fundamental measures of additive structure |
| Energy.lean | Additive energy E[s, t]: counts quadruples (a₁, a₂, b₁, b₂) where a₁ + b₁ = a₂ + b₂, central quantity in additive combinatorics |
| ErdosGinzburgZiv.lean | Erdős-Ginzburg-Ziv theorem: any 2n - 1 elements of ℤ/nℤ contain n elements summing to zero, proved using Chevalley-Warning |
| ETransform.lean | E-transform technique: replaces sets to decrease sumset size while preserving sum of cardinalities, used in Cauchy-Davenport proof |
| FreimanHom.lean | Freiman homomorphisms and isomorphisms: n-Freiman homomorphism preserves n-fold sums, generalizing group homomorphisms with domain restricted to a set |
| PluenneckeRuzsa.lean | Plünnecke-Ruzsa inequality and Ruzsa triangle inequality: fundamental bounds relating sizes of sumsets and difference sets, showing small doubling implies small powers in abelian groups |
| Randomisation.lean | Randomization techniques for additive combinatorics |
| RuzsaCovering.lean | Ruzsa covering lemma: tool for bounding size of sumsets via covering arguments |
| SmallTripling.lean | Small tripling implies small powers: shows sets with \|A³\| ≤ k\|A\| have bounded higher powers even in non-abelian groups (stronger than small doubling for non-abelian case) |
| VerySmallDoubling.lean | Very small doubling: characterization of sets with minimal doubling constant, related to affine structure |

## Subdirectories

- [~] `AP/` - Arithmetic progressions (preliminary)
- [ ] `Corner/` - Corners and corner-free sets (pending)

## Search Tags

additive-combinatorics sumset doubling-constant tripling cauchy-davenport pluennecke-ruzsa erdos-ginzburg-ziv freiman-homomorphism approximate-subgroup additive-energy dissociation ruzsa-triangle-inequality e-transform corner-free arithmetic-progression roth-theorem salem-spencer 3ap-free
