---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/Additive
generated: 2025-12-08T20:30:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 17
subdirs_count: 2
---

# Additive

## Overview

The `Additive/` directory contains a comprehensive formalization of additive combinatorics, combining sumset theory, density results, and structural theorems. The core provides foundational tools including Freiman homomorphisms, doubling/tripling constants, additive energy, approximate subgroups, and dissociation. Classical results include the Cauchy-Davenport theorem (lower bounds on sumset sizes), Plünnecke-Ruzsa inequality (relating doubling to higher powers), Erdős-Ginzburg-Ziv theorem (zero-sum problems in cyclic groups), and the Ruzsa triangle inequality. The specialized subdirectories provide a complete theory of 3-term arithmetic progressions (3AP-free sets, Roth numbers, Behrend's construction) and prove Roth's theorem via the corners theorem using Szemerédi's regularity lemma, demonstrating the deep connections between different areas of additive combinatorics.

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

- [x] `AP/` - Complete theory of 3-term arithmetic progressions: definitions (3AP-free/3GP-free sets, Roth numbers), decidability instances, monotonicity and preservation theorems under Freiman homomorphisms, product constructions, and Behrend's sphere construction proving the lower bound on Roth numbers
- [x] `Corner/` - Corners theorem and its connection to Roth's theorem: defines corners and corner-free sets, proves corners theorem using triangle removal via Szemerédi's regularity lemma, derives Roth's theorem as a consequence with asymptotic density bounds

## Search Tags

additive-combinatorics sumset doubling-constant tripling cauchy-davenport pluennecke-ruzsa erdos-ginzburg-ziv freiman-homomorphism approximate-subgroup additive-energy dissociation ruzsa-triangle-inequality e-transform corner-free arithmetic-progression roth-theorem salem-spencer 3ap-free
