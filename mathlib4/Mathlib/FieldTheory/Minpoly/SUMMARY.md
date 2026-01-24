---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/FieldTheory/Minpoly
generated: 2026-01-24T22:45:00Z
git_sha: 073b1c781e4870a435fcc3a04440176ab0c8af88
git_branch: heads/nightly-testing
status: complete
files_count: 6
subdirs_count: 0
---

# Minpoly

## Overview

The `Minpoly/` directory contains the complete theory of minimal polynomials in field theory and algebra. It defines the minimal polynomial of an element as the monic polynomial of smallest degree having that element as a root, and develops this theory across different contexts: general rings, fields, and integrally closed domains. The directory covers fundamental properties (irreducibility, uniqueness, divisibility), specialized results for fields and integrally closed domains, conjugate roots and their equivalence classes, and the quotient polynomial `minpoly R x / (X - C x)` used in trace form duality.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of minimal polynomials: defines `minpoly A x` as the monic polynomial of smallest degree with `x` as root (or 0 if non-integral); proves basic properties like monic, nonzero, element is a root, not equal to 1 |
| Field.lean | Minimal polynomials over fields: proves irreducibility, uniqueness characterization, divisibility of any polynomial with the element as root, radical property for reduced rings, scalar tower results |
| IsIntegrallyClosed.lean | Minimal polynomials over integrally closed domains: proves minimal polynomial over ring equals minimal polynomial over fraction field (when mapped), divisibility for primitive polynomials, kernel characterization |
| IsConjRoot.lean | Conjugate roots theory: defines `IsConjRoot K x y` (same minimal polynomial), proves it's an equivalence relation, provides operations preserving conjugacy (addition/multiplication by scalars), connects to Galois automorphisms in normal extensions |
| ConjRootClass.lean | Conjugacy classes: defines `ConjRootClass K L` as quotient of `L` by `IsConjRoot` relation, provides quotient map `mk`, proves properties of conjugacy classes including carrier sets and arithmetic operations |
| MinpolyDiv.lean | Quotient polynomial theory: defines `minpolyDiv R x = minpoly R x / (X - C x)`, proves evaluation properties (equals derivative at x, zero at other roots), spans adjoin of x, used for trace form dual basis |

## Subdirectories

*None*

## Search Tags

minimal-polynomial minpoly field-theory monic-polynomial irreducible-polynomial polynomial-roots integrally-closed fraction-field conjugate-roots equivalence-relation galois-automorphisms conjugacy-classes quotient-polynomial derivative trace-form dual-basis algebraic-elements integral-elements polynomial-division aeval
