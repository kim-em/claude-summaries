---
source_path: /Users/kim/projects/lean/mathlib4
generated: 2025-12-01T03:29:28Z
git_sha: dc19f2a67ff55a2078ba23a4c1740a5eb0d50e41
git_branch: master
status: preliminary
files_count: 15
subdirs_count: 10
---

# mathlib4

## Overview

Mathlib4 is the main mathematical library for the Lean 4 theorem prover, maintained by the Lean community. It contains a comprehensive collection of formalized mathematics spanning algebra, analysis, topology, number theory, category theory, and more, along with supporting tactics and automation. The library serves as both programming infrastructure and a foundation for formal mathematical development in Lean 4.

## Key Files

| File | Purpose |
|------|---------|
| README.md | Project documentation covering installation, usage, contributing guidelines, and maintainer information |
| lakefile.lean | Lake build configuration defining package structure, dependencies (batteries, Qq, aesop, proofwidgets), linter options, and build targets |
| lean-toolchain | Specifies Lean version (v4.26.0-rc2) used by this project |
| Mathlib.lean | Root import file containing all 7331 public imports from the Mathlib library |
| Archive.lean | Root import file for archived/historical mathematical content |
| Counterexamples.lean | Root import file for mathematical counterexamples |
| MathlibTest.lean | Root import for test suite |
| docs.lean | Root import for additional documentation modules |
| CODE_OF_CONDUCT.md | Contributor Covenant Code of Conduct for the community |
| LICENSE | Apache 2.0 license for the project |
| bors.toml | Configuration for Bors merge bot |
| lake-manifest.json | Lock file tracking exact versions of dependencies |

## Subdirectories

- [?] `Mathlib/` - Core mathematical library containing formalized mathematics
- [?] `Archive/` - Historical and archived mathematical content
- [?] `Counterexamples/` - Collection of mathematical counterexamples
- [?] `MathlibTest/` - Test suite for verifying library functionality
- [?] `Cache/` - Cache management utilities for downloading precompiled .olean files
- [ ] `LongestPole/` - Tools for analyzing build time longest poles and unused imports
- [ ] `DownstreamTest/` - Tests for downstream package compatibility
- [ ] `docs/` - Additional documentation in the form of module docstrings
- [ ] `scripts/` - Utility scripts for linting, code generation, and project maintenance
- [ ] `widget/` - ProofWidgets integration and UI components

## Search Tags

lean4 theorem-prover formal-mathematics mathlib formalization algebra analysis topology category-theory number-theory tactics automation proof-assistant lake build-system
