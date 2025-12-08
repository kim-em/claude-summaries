---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Combinatorics/Optimization
generated: 2025-12-08T16:00:00Z
git_sha: 8427e48fbc3922ef6f581162121a110b53390490
git_branch: fix-deprecated-module-linter-public-import
status: complete
files_count: 1
subdirs_count: 0
---

# Optimization

## Overview

The `Optimization/` directory formalizes general-valued constraint satisfaction problems (VCSP), a broad class of discrete optimization problems that subsume Min-Cost-Hom (including 3-SAT) and Finite-Valued CSP. The directory provides a template-based framework where optimization instances are built from allowed cost functions over a domain, with solutions evaluated as sums of term costs. The formalization includes fractional polymorphisms as a central algebraic tool for characterizing problem complexity, and proves that Max-Cut (shown via the max-cut property for binary cost functions) cannot admit symmetric fractional polymorphisms.

## Key Files

| File | Purpose |
|------|---------|
| ValuedCSP.lean | General-valued constraint satisfaction problem framework: defines VCSP templates (sets of cost functions D^n → C), terms (instantiated cost functions with variable assignments), instances (multisets of terms), solution evaluation (sum of term costs), optimality criterion (minimum over all solutions), max-cut property characterization (binary functions with argmin exactly at two complementary labelings), fractional operations (multisets of operations D^m → D), and fractional polymorphism theory proving max-cut functions forbid symmetric fractional polymorphisms |

## Subdirectories

(none)

## Search Tags

optimization discrete-optimization constraint-satisfaction valued-csp vcsp max-cut fractional-polymorphism cost-function polymorphism complexity-theory 3-sat min-cost-hom algebraic-complexity
