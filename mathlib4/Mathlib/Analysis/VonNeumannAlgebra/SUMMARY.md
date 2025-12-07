---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/VonNeumannAlgebra
generated: 2025-12-07T09:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 1
subdirs_count: 0
---

# VonNeumannAlgebra

## Overview

This directory contains the formalization of von Neumann algebras in both their abstract and concrete forms. It defines `WStarAlgebra` (Sakai's abstract definition as a C*-algebra with Banach space predual) and `VonNeumannAlgebra` (the concrete double commutant definition as a *-closed subalgebra of bounded operators on a Hilbert space). The file establishes basic structural properties, commutants, and characterizations of idempotents and star projections in von Neumann algebras. A major future project is proving the equivalence between these two definitions and the von Neumann double commutant theorem.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `WStarAlgebra` (abstract von Neumann algebra as C*-algebra with predual) and `VonNeumannAlgebra` (concrete definition via double commutant); establishes SetLike and SubringClass instances, commutant operations, and characterization theorems for idempotents and star projections |

## Subdirectories

None.

## Search Tags

von-neumann-algebra wstar-algebra double-commutant sakai-definition cstar-algebra banach-predual hilbert-space bounded-operators star-subalgebra commutant centralizer idempotent star-projection weak-topology strong-topology functional-analysis operator-algebras
