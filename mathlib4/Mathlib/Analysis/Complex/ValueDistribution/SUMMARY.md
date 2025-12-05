---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Complex/ValueDistribution
generated: 2025-12-05T00:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 4
subdirs_count: 0
---

# ValueDistribution

## Overview

This directory implements Nevanlinna Value Distribution Theory for meromorphic functions on the complex plane. It defines the three main functions of value distribution theory: the characteristic function (Nevanlinna height), the counting function, and the proximity function. These functions measure the "complexity" of meromorphic functions, with the characteristic function playing a role analogous to height functions in number theory. The directory includes proofs of the First Main Theorem of Value Distribution Theory, which establishes invariance properties of the characteristic function under function transformations.

## Key Files

| File | Purpose |
|------|---------|
| CharacteristicFunction.lean | Defines the characteristic function (Nevanlinna height) as the sum of proximity and counting functions; proves behavior under arithmetic operations (multiplication, powers); establishes subadditivity properties |
| CountingFunction.lean | Defines the logarithmic counting function that measures how often a meromorphic function takes a given value within a disk, weighted by multiplicity; proves Jensen's formula relating counting functions to circle averages of log ‖f‖ |
| ProximityFunction.lean | Defines the proximity function quantifying how well a meromorphic function approximates a constant on a circle; proves arithmetic properties and relationships between proximity functions of f and f⁻¹ |
| FirstMainTheorem.lean | Proves the First Main Theorem of Value Distribution Theory in two parts: (1) characteristic functions of f and f⁻¹ agree up to a bounded function, (2) characteristic functions of f and f - const agree up to a bounded function |

## Subdirectories

(No subdirectories)

## Search Tags

nevanlinna-theory value-distribution characteristic-function counting-function proximity-function meromorphic-functions jensen-formula first-main-theorem nevanlinna-height complex-analysis divisor-theory poles-zeros multiplicity circle-average logarithmic-counting lang-hyperbolic noguchi-winkelmann diophantine-approximation
