---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/Additive/AP/Three
generated: 2025-12-08T15:42:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 2
subdirs_count: 0
---

# Three

## Overview

This directory contains the core formalization of 3-term arithmetic progressions (3AP) in additive combinatorics. It includes the definition of 3AP-free sets (Salem-Spencer sets), Roth numbers, fundamental preservation theorems under Freiman homomorphisms, and Behrend's construction which provides an explicit lower bound showing that Roth numbers grow as `N * exp(-O(√(log N)))`. This is a leaf folder with no subdirectories, containing complete theory and constructions.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Defines 3AP-free and 3GP-free sets, Roth numbers (addRothNumber, mulRothNumber, rothNumberNat), decidability instances, monotonicity lemmas, preservation under Freiman homomorphisms and isomorphisms, product constructions, and special cases for natural numbers |
| Behrend.lean | Proves Behrend's lower bound on Roth numbers using the sphere construction - maps integer points on spheres to natural numbers preserving 3AP-freeness, includes optimization of parameters (nValue, dValue), numerical bounds, and the main theorem showing rothNumberNat N ≥ N * exp(-4 * √(log N)) |

## Subdirectories

No subdirectories.

## Search Tags

3ap-free 3gp-free salem-spencer roth-number additive-combinatorics arithmetic-progression behrend-construction sphere strictly-convex freiman-homomorphism lower-bound combinatorics
