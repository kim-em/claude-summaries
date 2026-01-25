---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/Real
generated: 2026-01-25T23:57:00Z
git_sha: ffb766c85c7ad82861131c2f10a0669884e4fd5f
git_branch: HEAD
status: complete
files_count: 2
subdirs_count: 0
---

# Real

## Overview

The `Real/` directory contains number-theoretic results about specific real numbers, focusing on irrationality proofs and properties of algebraic constants. It provides the foundational `Irrational` predicate along with comprehensive closure properties under arithmetic operations, and applies this machinery to prove irrationality of square roots and the golden ratio.

## Key Files

| File | Purpose |
|------|---------|
| Irrational.lean | Defines the `Irrational` predicate for real numbers, proves square roots of non-square integers are irrational (including the famous √2), provides Decidable instances for automated irrationality checking, and establishes closure properties (addition, multiplication, negation, inverse) with dot-style API |
| GoldenRatio.lean | Defines the golden ratio φ = (1+√5)/2 and its conjugate ψ = (1-√5)/2, proves their irrationality, establishes algebraic identities (φ² = φ+1, φψ = -1), proves Binet's formula expressing Fibonacci numbers as (φⁿ - ψⁿ)/√5, and connects them to the Fibonacci recurrence relation |

## Subdirectories

_(none)_

## Search Tags

irrational real-numbers golden-ratio fibonacci binet-formula square-root transcendental algebraic-numbers sqrt-2 phi decidable closure-properties dot-notation
