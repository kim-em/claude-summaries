---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/IntegralClosure/IsIntegralClosure
generated: 2026-02-01T20:15:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 2
subdirs_count: 0
---

# IsIntegralClosure

## Overview

The `IsIntegralClosure/` directory defines and develops the characteristic predicate `IsIntegralClosure A R B`, which states that `A` is the integral closure of `R` in `B`. This means an element of `B` is integral over `R` if and only if it lies in the image of the algebra map from `A` to `B`. The directory provides the core definition as a typeclass and proves extensive properties including: integral elements in division rings are units, integral subalgebras of division rings are closed under inverses, the equivalence "finite = integral + finite type" (with a reference to the Kurosh problem), transitivity of integral extensions, lifting maps between integral closures, and the fact that the integral closure of a field in a domain is itself a field.

## Key Files

| File | Purpose |
|------|---------|
| Defs.lean | Defines `IsIntegralClosure A R B` as a typeclass with two properties: injectivity of `algebraMap A B` and the characteristic predicate that `x : B` is integral over `R` iff `x` is in the image of `A` |
| Basic.lean | Main development of `IsIntegralClosure` properties: inverses of integral elements stay integral, `Algebra.IsIntegral.finite` (integral + finite type = finite module), transitivity (`IsIntegral.trans`), lifting algebra homomorphisms via `IsIntegralClosure.lift`, equivalence of integral closures via `IsIntegralClosure.equiv`, quotient compatibility, local ring structure on integral extensions, and that integral closures of fields are fields |

## Subdirectories

(none)

## Search Tags

IsIntegralClosure integral-closure characteristic-predicate inverse-integral inv-mem finite-type Kurosh-problem Algebra.IsIntegral.finite isIntegral_trans transitivity lift-integral-closure equiv-integral-closure quotient-integral isLocalHom isField-integral algebraMap-injective adjoin-integral integralClosure-idem roots-integral
