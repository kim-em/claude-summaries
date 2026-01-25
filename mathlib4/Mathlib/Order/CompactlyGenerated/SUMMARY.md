---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/CompactlyGenerated
generated: 2026-01-25T20:00:00Z
git_sha: ffb766c85c7ad82861131c2f10a0669884e4fd5f
git_branch: HEAD
status: complete
files_count: 2
subdirs_count: 0
---

# CompactlyGenerated

## Overview

This directory contains the theory of compactly generated complete lattices, compact elements, and related compactness properties. The main results establish four equivalent characterizations of well-foundedness in complete lattices: well-founded `>` relation, sup-closed compactness, sup-finite compactness, and every element being compact. The directory also provides fundamental results about compact elements, including their interaction with directed sets and intervals, and proves that compactly generated modular lattices are complemented if and only if they are atomistic.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core theory: defines `IsCompactElement`, `IsSupClosedCompact`, `IsSupFiniteCompact`, `IsCompactlyGenerated` class; proves equivalence of four well-foundedness characterizations; establishes that well-founded lattices are compactly generated; proves compact elements make `[⊥, k]` coatomic; shows compactly generated modular atomistic lattices are complemented (Theorem 6.6, Călugăreanu) |
| Intervals.lean | Compactness for intervals in complete lattices: proves compact elements in α remain compact when viewed in Iic a; shows Iic a is compactly generated when α is; proves complemented lattice structure can be lifted from intervals to the whole lattice |

## Subdirectories

(No subdirectories)

## Search Tags

compactly-generated compact-element well-founded complete-lattice directed-set sup-closed sup-finite IsCompactElement IsCompactlyGenerated complemented-lattice modular-lattice atomistic coatomic interval upper-continuous Zorn Călugăreanu
