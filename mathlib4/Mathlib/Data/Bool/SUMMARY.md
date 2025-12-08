---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/Bool
generated: 2025-12-08T15:40:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 4
subdirs_count: 0
---

# Bool

## Overview

This directory contains foundational lemmas and properties about the Boolean type (`Bool`) in Lean. It covers basic Boolean algebra (equality, negation, conjunction, disjunction, XOR), the relationship between Booleans and decidable propositions via `decide`, Boolean quantifiers on lists (`all` and `any`), counting occurrences of true/false values in lists, De Morgan's laws, and the linear order structure on Booleans. It also includes set-theoretic operations on Booleans such as `Set.univ` and `Set.range`, providing the mathematical foundation for Boolean reasoning in mathlib4.

## Key Files

| File | Purpose |
|------|---------|
| AllAny.lean | Boolean quantifiers for lists; proves properties of `List.all` (universal) and `List.any` (existential) relating them to `∀` and `∃` propositions |
| Basic.lean | Core Boolean lemmas including equality, negation, conjunction, disjunction, XOR, relationship with decidable propositions, De Morgan's laws, linear order instance, conversions to/from natural numbers, and Kaminski's equation |
| Count.lean | Counting lemmas for lists of Booleans; proves relationships between counts of true/false values and list length, especially for alternating chains with `IsChain (· ≠ ·)` |
| Set.lean | Set-theoretic operations on Booleans; proves `Set.univ = {false, true}`, range and complement lemmas for Boolean sets |

## Subdirectories

*(none)*

## Search Tags

bool boolean logic decidable propositions quantifiers lists counting order linear-order xor de-morgan set-theory
