---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/ClassNumber
generated: 2026-01-25T22:30:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# ClassNumber

## Overview

The `ClassNumber/` directory formalizes the finiteness of class groups for global fields (both number fields and function fields) using the theory of admissible absolute values. It provides the general machinery for showing that any integral closure with an admissible absolute value has a finite class group, along with specific instantiations for the standard absolute value on integers and the cardPowDegree absolute value on polynomials over finite fields.

## Key Files

| File | Purpose |
|------|---------|
| AdmissibleAbsoluteValue.lean | Core definition of `IsAdmissible` structure for absolute values `R → ℤ` that respect Euclidean domain structure and guarantee existence of close approximations via pigeonhole-style partition arguments |
| AdmissibleAbs.lean | Proves the standard absolute value on ℤ is admissible (`absIsAdmissible`) using partition of remainders with ceiling bound `⌈1/ε⌉₊` |
| AdmissibleCardPowDegree.lean | Proves `cardPowDegree` on polynomials over finite fields (mapping `p : 𝔽_q[X]` to `q^(degree p)`) is admissible using logarithmic partition bounds |
| Finite.lean | Main class number theorem: proves `ClassGroup.fintypeOfAdmissibleOfFinite` showing class groups are finite for integral closures with admissible absolute values, using norm bounds and approximation to reduce to finitely many ideal classes |
| FunctionField.lean | Instantiates the class number theorem for function fields, defining `classNumber Fq F` as the cardinality of the class group and proving it equals 1 iff the ring of integers is a PID |

## Subdirectories

(none)

## Search Tags

class-number class-group admissible-absolute-value finiteness number-fields function-fields integral-closure dedekind-domain ideal-class-group norm-bounds approximation pigeonhole polynomial-rings finite-fields cardPowDegree euclidean-domain algebraic-number-theory global-fields
