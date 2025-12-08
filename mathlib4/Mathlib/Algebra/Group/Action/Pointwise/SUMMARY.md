---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Group/Action/Pointwise
generated: 2025-12-01T23:55:00Z
git_sha: dc19f2a67ff55a2078ba23a4c1740a5eb0d50e41
git_branch: master
status: complete
files_count: 1
subdirs_count: 1
---

# Pointwise

## Overview

The `Pointwise/` directory implements pointwise group actions on sets and finsets, extending the basic group action theory to collective operations on finite and infinite collections. It provides the infrastructure for lifting scalar multiplication from individual elements to sets and finsets, establishing that multiplicative actions `M → α → α` naturally induce actions `Set M → Set α → Set α` and `Finset M → Finset α → Finset α`, along with comprehensive theory for translating, scaling, and manipulating collections under group actions. The `Set/` subdirectory provides the theoretical foundation with complete treatment of how set operations interact with actions, while the `Finset.lean` file provides the computationally-decidable finite counterpart with cardinality-preserving operations and coset theory for finsets.

## Key Files

| File | Purpose |
|------|---------|
| Finset.lean | Pointwise actions on finsets; defines `Finset.mulAction` and `Finset.mulActionFinset` lifting monoid actions to finsets, provides typeclass instances for `SMulCommClass`, `IsScalarTower`, and `IsCentralScalar` on finsets, includes lemmas for set operations under actions (intersection, difference, symmetric difference), cardinality preservation, and coset theory for finsets |

## Subdirectories

- [x] `Set/` - Pointwise actions on sets

## Search Tags

pointwise group-action finset-action set-action scalar-multiplication smul pointwise-operations coset translation scaling smul-comm-class scalar-tower finset-algebra typeclass-instances cardinality-preservation product-operations image-operations
