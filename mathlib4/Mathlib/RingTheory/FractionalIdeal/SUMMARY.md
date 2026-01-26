---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/FractionalIdeal
generated: 2026-01-26T19:45:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: complete
files_count: 5
subdirs_count: 0
---

# FractionalIdeal

## Overview

The `FractionalIdeal/` directory provides a comprehensive formalization of fractional ideals in commutative algebra. Fractional ideals generalize ordinary ideals by allowing denominators: they are R-submodules I of a localization P such that aI ⊆ R for some a. The directory defines the basic type `FractionalIdeal S P`, proves it forms a commutative semiring and lattice under ideal operations, and provides specialized operations including ideal quotients (division), inverses, extension along ring homomorphisms, and absolute norms for fractional ideals over Dedekind domains.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: `IsFractional` predicate, `FractionalIdeal S P` type as subtype, coercion to submodules, lattice and commutative semiring instances, ideal operations (multiplication, addition as sup, containment), monotonicity of multiplication |
| Operations.lean | Additional operations: `map` for pushforward along algebra morphisms, `Div` instance for ideal quotient (I / J), Noetherian property (fractional ideals over Noetherian domains are Noetherian) |
| Inverse.lean | Inverse operator `I⁻¹` defined as `1 / I`, properties of inverses for nonzero fractional ideals; note that invertibility theorem (all nonzero fractional ideals are invertible in Dedekind domains) is in DedekindDomain/Ideal/Basic.lean |
| Extended.lean | Extension of fractional ideals along ring homomorphisms: `extended` function and `extendedHom` ring homomorphism for extending fractional ideals from IsLocalization M K to IsLocalization N L, injectivity results for extensions over Dedekind domains |
| Norm.lean | Absolute norm for fractional ideals: `absNorm : FractionalIdeal R⁰ K →*₀ ℚ` defined as `absNorm(I.num) / |norm(I.den)|` where I = (I.num)/(I.den), determinant interpretation via basis change matrices, norm of principal fractional ideals |

## Subdirectories

None - this is a leaf directory.

## Search Tags

fractional-ideal fractional-ideals commutative-algebra localization field-of-fractions ideal-theory invertible-ideal Dedekind-domain ideal-quotient division inverse norm absolute-norm extension principal-ideal Noetherian submodule lattice semiring Marcus Cassels Froehlich Neukirch
