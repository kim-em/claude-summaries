---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Data/FP
generated: 2025-12-09T06:00:00Z
git_sha: 52bf977aaf73eb6dcf02137c12d9ed22fd9687ef
git_branch: fix/improve-init-import-error-message
status: complete
files_count: 1
subdirs_count: 0
---

# FP

## Overview

The `FP/` directory contains an experimental implementation of floating-point numbers in Lean. It provides a configuration-based framework for arbitrary-precision floating-point arithmetic with formal validation constraints. The implementation includes IEEE-style rounding modes (currently only round-to-nearest-even), finite/infinite/NaN representations, and basic arithmetic operations (add, subtract, multiply, divide) that convert through rational numbers to maintain mathematical precision. Most operations are marked unsafe pending formal verification.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core floating-point implementation with type `Float` (parameterized by precision and exponent bounds), validity constraints for finite values, conversions to/from rationals, rounding modes, and arithmetic operations; includes unsafe implementations pending proof obligations |

## Subdirectories

(No subdirectories)

## Search Tags

floating-point arithmetic FP IEEE-754 rounding precision exponent rational-conversion finite infinite NaN unsafe experimental validation
