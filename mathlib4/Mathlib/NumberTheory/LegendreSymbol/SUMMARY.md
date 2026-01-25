---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/NumberTheory/LegendreSymbol
generated: 2026-01-25T22:50:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 6
subdirs_count: 1
---

# LegendreSymbol

## Overview

The `LegendreSymbol/` directory provides a comprehensive formalization of the Legendre and Jacobi symbols, fundamental tools in number theory for determining quadratic residuosity. The directory includes the definition and basic properties of the Legendre symbol for primes (via Euler's criterion), its generalization to the Jacobi symbol for composite moduli, the celebrated Law of Quadratic Reciprocity and its supplementary laws for -1, 2, and -2, and Gauss's and Eisenstein's lemmas used in reciprocity proofs. The underlying theory is built on additive characters, quadratic characters on finite fields (which compute via Euler's criterion and connect to special values via Gauss sums), and specialized characters χ₄, χ₈, χ₈' on ZMod rings. The `QuadraticChar/` subdirectory extends these ideas to finite fields generally, proving when elements like -1, 2, and odd primes are squares based on field cardinality modulo 4 and 8. Applications include binary quadratic forms, counting square roots, and efficient computation via fast recursive algorithms with csimp rules.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core Legendre symbol definition, Euler's criterion, multiplicativity, values at 0/1/-1, connection to squares mod p, applications to binary quadratic forms |
| AddCharacter.lean | Additive characters on finite rings/fields, primitive characters, existence results for ZMod and finite fields, character sums, complex-valued characters |
| GaussEisensteinLemmas.lean | Gauss's lemma (computing Legendre symbol via counting) and Eisenstein's lemma for quadratic reciprocity proofs |
| JacobiSymbol.lean | Jacobi symbol definition extending Legendre to composite moduli, multiplicativity, quadratic reciprocity, supplementary laws for -1/2/-2, fast computation via csimp rules |
| QuadraticReciprocity.lean | Law of Quadratic Reciprocity for Legendre symbol, supplementary laws for 2 and -2, interpretation via congruences mod 4 and 8 |
| ZModChar.lean | Quadratic characters χ₄, χ₈, χ₈' on ZMod 4 and ZMod 8, explicit formulas in terms of residues, connection to powers of -1 |

## Subdirectories

- [x] `QuadraticChar/` - Quadratic characters on finite fields determining quadratic residuosity via Euler's criterion, Gauss sum theory for special values at 2/-2, criteria for when elements are squares based on card F mod 8, reciprocity theorem relating characters across different fields

## Search Tags

legendre-symbol jacobi-symbol quadratic-reciprocity quadratic-residue quadratic-character gauss-lemma eisenstein-lemma euler-criterion additive-character primitive-character finite-field zmod multiplicative-character binary-quadratic-form
