---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/GroupTheory/Commutator
generated: 2026-01-24T22:51:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# Commutator

## Overview

The `Commutator/` directory formalizes commutators in group theory, covering both element-level commutators `⁅g₁, g₂⁆ = g₁ * g₂ * g₁⁻¹ * g₂⁻¹` and subgroup-level commutators `⁅H₁, H₂⁆`. Basic.lean establishes foundational properties including the commutator subgroup (normal closure of all commutators), the Three Subgroups Lemma via Hall-Witt identity, relationships with centralizers and centers, and conditions for quotient commutativity. Finite.lean extends this theory to finite contexts, proving that commutator subgroups are finitely generated when the commutator set is finite, establishing bounds on center indices, and providing equality for commutators of finite direct products.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core commutator theory: element/subgroup commutators, Three Subgroups Lemma, normality, characteristic subgroups, centralizer/center relationships, quotient commutativity characterization, representatives |
| Finite.lean | Finiteness properties: finite generation of commutator subgroups when commutatorSet is finite, bounds on center index (≤ card(commutatorSet)^rank(G)), equality of commutators for finite direct products |

## Subdirectories

*(No subdirectories)*

## Search Tags

commutator subgroup bracket hall-witt three-subgroups lemma centralizer center normal-subgroup characteristic quotient-group abelianization derived-series finite-generation rank index direct-product representatives
