---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Order/Archimedean
generated: 2025-12-01T10:55:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 5
subdirs_count: 0
---

# Archimedean

## Overview

The `Archimedean/` directory contains the theory of archimedean ordered structures, which formalize the idea that for any two elements `x` and `y > 0` (or `y > 1` in the multiplicative case), there exists a natural number `n` such that `x ≤ n • y` (or `x ≤ y ^ n`). This folder defines the core `Archimedean` and `MulArchimedean` typeclasses, proves that ℕ, ℤ, and ℚ are archimedean, establishes uniqueness results for ordered ring homomorphisms between archimedean fields, develops the theory of archimedean classes for measuring how groups fail to be archimedean, and proves results relating indicator functions to cardinality in archimedean contexts. The folder also shows that submonoids inherit the archimedean property from their ambient structures.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core archimedean definitions: `Archimedean` and `MulArchimedean` typeclasses, floor function construction on archimedean linearly ordered rings, existence of powers/multiples exceeding any element, instances for ℕ, ℤ, ℚ |
| Class.lean | Archimedean classes for linearly ordered groups: partitions groups by "infinitesimal order" where elements in the same class satisfy `\|a\| ≤ m • \|b\|` and `\|b\| ≤ n • \|a\|` for some m,n, with order homomorphisms and ball subgroups, characterizes archimedean groups as those with all elements in one class |
| Hom.lean | Uniqueness of ordered ring homomorphisms to archimedean fields: at most one `α →+*o β` from a linear ordered field to an archimedean linear ordered field, with corresponding uniqueness for isomorphisms |
| IndicatorCard.lean | Cardinality and limits of indicator sums: characterizes infinite sets via `Tendsto (∑ k < n, s.indicator r k) atTop`, relates limsup to indicator sum convergence in archimedean ordered additive monoids |
| Submonoid.lean | Inheritance of archimedean property: `SubmonoidClass.instMulArchimedean` and `AddSubmonoidClass.instArchimedean` show that submonoids of archimedean structures are themselves archimedean |

## Subdirectories

(none)

## Search Tags

archimedean mul-archimedean ordered-structures ordered-groups ordered-fields archimedean-property archimedean-classes infinitesimal-order floor-ring floor-function uniqueness-homomorphisms ordered-ring-homomorphism indicator-functions cardinality limsup tendsto submonoid inheritance
