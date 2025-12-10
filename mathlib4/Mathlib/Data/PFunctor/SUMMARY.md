---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/PFunctor
generated: 2025-12-11T12:00:00Z
git_sha: d3b1fce8074ef80dac7bb8dc86bbe26d1db89f2b
git_branch: linarith_to_grind_regressions
status: preliminary
files_count: 0
subdirs_count: 2
---

# PFunctor

## Overview

The `PFunctor/` directory defines polynomial functors and their applications to constructing inductive and coinductive data types. Polynomial functors are a fundamental tool for defining W-types (well-founded trees, least fixpoints) and M-types (potentially infinite trees, greatest fixpoints). The directory is split into univariate polynomial functors (single type parameter) and multivariate polynomial functors (type vectors), with both providing the theoretical foundation for quotients of polynomial functors (QPFs) used elsewhere in mathlib.

## Key Files

This directory contains no files directly; all content is in subdirectories.

## Subdirectories

- [x] `Multivariate/` - Multivariate polynomial functors mapping type vectors to types; defines `MvPFunctor`, M-types, and W-types for n-ary functors
- [ ] `Univariate/` - Univariate polynomial functors `PFunctor` with structure `(A : Type, B : A → Type)`; defines W-types and M-types as fixed points

## Search Tags

polynomial-functors pfunctor mvpfunctor w-types m-types inductive-types coinductive-types fixpoints corecursion well-founded-trees infinite-trees functor-composition
