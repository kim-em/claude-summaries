---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/ModelTheory/Algebra/Field
generated: 2026-01-25T19:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 3
subdirs_count: 0
---

# Field

## Overview

The `Field/` directory contains the first-order model-theoretic treatment of fields and their theories. It defines the theory of fields as a collection of first-order sentences in the language of rings, establishes the theory of fields with specific characteristics (including characteristic 0 and prime characteristics), and develops the complete theory of algebraically closed fields (ACF). The directory includes the proof of completeness for ACF and the Lefschetz principle, which relates properties of algebraically closed fields in characteristic 0 to those in characteristic p for almost all primes p.

## Key Files

| File | Purpose |
|------|---------|
| `Basic.lean` | Defines the first-order theory of fields as axioms over the language of rings, proves that models of the field theory correspond to Mathlib field structures via `fieldOfModelField` and `compatibleRingOfModelField` |
| `CharP.lean` | Extends the field theory to fields of characteristic p, defining `Theory.fieldOfChar p` and proving equivalence between being a model and having `CharP K p` |
| `IsAlgClosed.lean` | Defines the theory of algebraically closed fields `Theory.ACF p`, proves it is complete and κ-categorical for uncountable κ, establishes the Lefschetz principle relating characteristic 0 to characteristic p properties |

## Subdirectories

This directory contains no subdirectories.

## Search Tags

model-theory fields first-order-logic field-axioms characteristic algebraically-closed-fields ACF completeness lefschetz-principle categorical charP field-theory ring-language sentences axiomatization compatibility
