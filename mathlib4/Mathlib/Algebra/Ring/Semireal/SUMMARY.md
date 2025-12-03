---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Ring/Semireal
generated: 2025-12-01T19:45:30Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 1
subdirs_count: 0
---

# Semireal

## Overview

The `Semireal/` directory contains the theory of semireal rings, which are commutative rings in which `-1` is not a sum of squares. This is a fundamental concept in real algebra, with linearly ordered rings being a primary example (since sums of squares are positive and `-1` is negative). The single file provides the core definition via the `IsSemireal` typeclass and establishes that linearly ordered semirings are semireal.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | `IsSemireal` typeclass: characterizes semireal rings where `-1` is not a sum of squares, with instance showing linearly ordered semirings satisfy this property |

## Subdirectories

None.

## Search Tags

semireal ring sum-of-squares ordered-ring real-algebra negative-one linearly-ordered commutative-ring
