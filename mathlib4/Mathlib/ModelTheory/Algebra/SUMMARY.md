---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/ModelTheory/Algebra
generated: 2026-01-25T20:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 0
subdirs_count: 2
---

# Algebra

## Overview

The `Algebra/` directory applies first-order model theory to algebraic structures, specifically rings and fields. It provides the formal language of rings with operations (+, *, -, 0, 1), establishes compatibility between model-theoretic structures (`Language.ring.Structure`) and Mathlib's algebraic type classes (`Ring`, `Field`), and develops complete first-order theories for fields with various characteristics and algebraically closed fields. The directory solves the fundamental problem of bridging two different ways to express algebraic structures: via Mathlib's type classes versus model theory's structure semantics. It includes major results such as the completeness and categoricity of the theory of algebraically closed fields (ACF), the Lefschetz principle relating characteristic 0 to characteristic p, and the definability of polynomial zero loci.

## Key Files

This directory contains no files directly—all content is organized into subdirectories.

## Subdirectories

- [x] `Field/` - First-order theory of fields as axioms over the language of rings, theories of fields with specific characteristics (0 and prime p), complete theory of algebraically closed fields with completeness and κ-categoricity proofs, Lefschetz principle relating characteristic 0 to characteristic p
- [x] `Ring/` - Defines `Language.ring` with function symbols {+, *, -, 0, 1}, `CompatibleRing` type class for reconciling model-theoretic and algebraic structures, bidirectional conversions, definability of multivariable polynomial zero loci, and conversion of `FreeCommRing` elements to terms

## Search Tags

model-theory algebraic-structures rings fields language-of-rings compatible-ring field-theory algebraically-closed-fields characteristic-p ACF lefschetz-principle definability polynomial-zero-locus free-comm-ring
