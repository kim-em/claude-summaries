---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Order/Extension
generated: 2026-01-26T22:51:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 2
subdirs_count: 0
---

# Extension

## Overview

The `Extension/` directory contains constructions for extending partial orders and well-founded orders to linear orders and well-orders, respectively. It implements two fundamental extension theorems using Zorn's lemma and ordinal rank functions. The linear extension uses the Szpilrajn extension theorem to extend any partial order to a linear order, while the well-order extension maps well-founded relations into the lexicographic product of ordinal ranks and cardinal embeddings.

## Key Files

| File | Purpose |
|------|---------|
| Linear.lean | Szpilrajn extension theorem proving any partial order can be extended to a linear order using Zorn's lemma; provides `LinearExtension` type alias and `toLinearExtension` order homomorphism |
| Well.lean | Extends well-founded orders to well-orders via lexicographic product of ordinal rank and cardinal embedding; provides `WellOrderExtension` type alias and proves `exists_well_order_ge` theorem |

## Subdirectories

None.

## Search Tags

order-extension Szpilrajn linear-extension well-order-extension partial-order well-founded-order Zorns-lemma ordinal-rank lexicographic-order
