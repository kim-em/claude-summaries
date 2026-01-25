---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/LocalField
generated: 2026-01-25T22:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 1
subdirs_count: 0
---

# LocalField

## Overview

The `LocalField/` directory defines the foundational theory of non-archimedean local fields in Lean. It introduces the `IsNonarchimedeanLocalField` typeclass for topological fields equipped with a valuation that is locally compact and non-discrete. The module proves that such fields automatically satisfy numerous key properties: the value group is isomorphic to ℤᵐ⁰, the valuation ring is a discrete valuation ring, the residue field is finite, and (with a compatible uniform structure) the field and its valuation ring are complete spaces.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `IsNonarchimedeanLocalField` typeclass and establishes core properties: compactness of closed balls, DVR structure of valuation ring, value group isomorphism to ℤᵐ⁰, finiteness of residue field, and completeness theorems |

## Subdirectories

(none)

## Search Tags

local-fields non-archimedean valuation discrete-valuation-ring DVR value-group residue-field complete-space locally-compact topological-field p-adic
