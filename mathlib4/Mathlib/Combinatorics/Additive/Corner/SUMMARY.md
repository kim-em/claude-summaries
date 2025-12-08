---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/Additive/Corner
generated: 2025-12-08T15:42:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 2
subdirs_count: 0
---

# Corner

## Overview

The `Corner/` directory formalizes the corners theorem and its connection to Roth's theorem on arithmetic progressions. A corner in an abelian group is a triple of points `(x, y), (x + d, y), (x, y + d)`, and the corners theorem proves that dense subsets of `G × G` must contain nontrivial corners. The proof uses triangle removal via Szemerédi's regularity lemma to establish that corner-free sets have density tending to zero as the group grows. The directory proves both the corners theorem and derives Roth's theorem as a consequence.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Defines corners (`IsCorner`), corner-free sets (`IsCornerFree`), basic properties (monotonicity, preservation under 2-Freiman homomorphisms/isomorphisms), and characterizations for subsingleton sets |
| Roth.lean | Proves the corners theorem for finite abelian groups and ℕ using triangle removal, derives Roth's theorem on 3-term arithmetic progressions from the corners theorem, provides asymptotic version showing `rothNumberNat` is little-o of the identity |

## Subdirectories

*(none)*

## Search Tags

corners corner-free corners-theorem roth-theorem arithmetic-progression 3ap-free szemeredi-regularity triangle-removal additive-combinatorics freiman-homomorphism density-result
