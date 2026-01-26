---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/Prod
generated: 2026-01-26T10:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 0
subdirs_count: 1
---

# Prod

## Overview

The `Prod/` directory provides theory for order structures on Cartesian products of ordered types. While product orders typically use the pointwise order where `(a₁, b₁) ≤ (a₂, b₂)` iff `a₁ ≤ a₂` and `b₁ ≤ b₂`, this directory focuses on lexicographic product orders. The `Lex/` subdirectory contains infrastructure for order homomorphisms that convert between standard products and lexicographic products, where pairs are ordered first by their first component, and the second component only matters when first components are equal.

## Key Files

*(No files directly in this directory)*

## Subdirectories

- [x] `Lex/` - Lexicographic product orders

## Search Tags

product-order Cartesian-product pointwise-order lexicographic-order binary-product order-product
