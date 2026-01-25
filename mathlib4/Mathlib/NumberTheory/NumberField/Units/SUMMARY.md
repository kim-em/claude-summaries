---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/NumberField/Units
generated: 2026-01-25T20:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# Units

## Overview

The `Units/` directory contains the formalization of the unit group `(𝓞 K)ˣ` of the ring of integers of a number field `K`, including Dirichlet's Unit Theorem and the regulator. This encompasses the fundamental theorem that the unit group modulo torsion is a free ℤ-module of rank `r₁ + r₂ - 1` (where `r₁` is the number of real embeddings and `r₂` is the number of complex conjugate pairs), along with the definition and properties of the regulator as a measure of the lattice formed by the logarithmic embedding of units.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core unit theory: characterization of units by norm (`isUnit_iff_norm`), torsion subgroup structure, coercion to field, complex embeddings, and fundamental results that torsion is finite and cyclic |
| DirichletTheorem.lean | Complete proof of Dirichlet Unit Theorem: defines logarithmic embedding, unit rank, fundamental system of units, proves unit lattice is a full ℤ-lattice, and establishes unique decomposition of units as root of unity times powers of fundamental units |
| Regulator.lean | Regulator theory: defines regulator of a family of units and of the number field, proves regulator equals absolute value of determinant of logarithmic matrix, and establishes index formulas relating regulators of different unit systems |

## Subdirectories

(No subdirectories)

## Search Tags

units number-field ring-of-integers unit-group torsion dirichlet-unit-theorem regulator fundamental-units logarithmic-embedding unit-lattice unit-rank roots-of-unity norm isUnit free-module lattice-covolume determinant index
