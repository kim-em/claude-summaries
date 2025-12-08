---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/Additive/AP
generated: 2025-12-08T20:15:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 0
subdirs_count: 1
---

# AP

## Overview

The `AP/` directory contains formalized results about arithmetic progressions in additive combinatorics. Currently it focuses exclusively on 3-term arithmetic progressions (3APs), providing a complete theory including: the definition of 3AP-free and 3GP-free sets (Salem-Spencer sets), Roth numbers (addRothNumber, mulRothNumber, rothNumberNat), preservation theorems under Freiman homomorphisms and isomorphisms, product constructions, and Behrend's explicit construction. Behrend's result, which maps integer points on spheres to natural numbers while preserving 3AP-freeness, establishes the key lower bound `rothNumberNat N ≥ N * exp(-4 * √(log N))`, showing that arbitrarily large 3AP-free sets exist with near-linear size.

## Key Files

No files directly in this directory.

## Subdirectories

- [x] `Three/` - Complete theory of 3-term arithmetic progressions: definitions (3AP-free/3GP-free sets, Roth numbers), decidability instances, monotonicity and preservation theorems under Freiman homomorphisms, product constructions, and Behrend's sphere construction proving the lower bound on Roth numbers (complete)

## Search Tags

arithmetic-progression 3ap 3ap-free salem-spencer roth-number behrend-construction additive-combinatorics
