---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Algebra/Spectrum
generated: 2025-12-01T20:15:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# Spectrum

## Overview

The `Spectrum/` directory develops the theory of spectra and quasispectra for elements in algebras, providing the algebraic foundation for spectral theory. The spectrum of an element `a` in an `R`-algebra `A` is the set of scalars `r : R` where `r•1 - a` is not a unit, capturing when the element fails to be invertible after a scalar shift. The quasispectrum extends this notion to non-unital algebras using quasiregularity (invertibility in the monoid structure `x ∘ y := y + x + x*y`), and serves as the domain for the non-unital continuous functional calculus.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of `resolventSet`, `spectrum`, and `resolvent` function, with fundamental properties including scalar multiplication/addition commutation, spectrum of products `σ(ab)` vs `σ(ba)`, star operations, and field-specific results |
| Quasispectrum.lean | Theory of quasiregularity and quasispectrum for non-unital algebras, defining `PreQuasiregular` type synonym with alternative monoid structure, relating quasiregularity to unitization via `IsQuasiregular x ↔ IsUnit (1 + x)`, and proving `quasispectrum R a = spectrum R a ∪ {0}` in unital algebras |
| Pi.lean | Spectrum and quasispectrum of indexed products and binary products, proving `spectrum R a = ⋃ i, spectrum R (a i)` for pi types and `spectrum R ⟨a,b⟩ = spectrum R a ∪ spectrum R b` for products, with analogous results for quasispectra |

## Subdirectories

None.

## Search Tags

spectrum quasispectrum resolvent resolvent-set quasiregular quasiregularity spectral-theory non-unital-algebra unitization functional-calculus banach-algebra pi-product spectrum-union
