---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Smooth
generated: 2026-02-01T23:15:00Z
git_sha: 5cb27be88dd78e9476463c255b7852485b175fb7
git_branch: master
status: complete
files_count: 13
subdirs_count: 0
---

# Smooth

## Overview

The `Smooth/` directory contains the formalization of smooth algebras and morphisms in commutative algebra. This includes formally smooth algebras (characterized by projective Kähler differentials and vanishing first cotangent cohomology), the standard lifting property for nilpotent ideals, standard smooth algebras (those admitting submersive presentations), and specialized results for smooth algebras over fields, local rings, and in relation to integral closure. The theory establishes smooth as the combination of formally smooth and finite presentation, and proves stability under composition, base change, and localization. Key results include the equivalence of standard smoothness with free Kähler differentials on {d sᵢ}, the relationship between smooth and étale (smooth of dimension 0), Noetherian descent (smooth algebras have finitely generated models), and the fundamental theorem that smooth algebras are flat.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of formally smooth and smooth algebras; proves equivalence with lifting property for square-zero ideals; establishes stability under isomorphisms, composition, base change, and localization |
| Kaehler.lean | Establishes correspondence between retractions of cotangent maps and algebra sections; proves formal smoothness is equivalent to split injectivity of I/I² → S ⊗[P] Ω[P⁄R] |
| StandardSmooth.lean | Standard smooth algebras (those with submersive presentations); relative dimension; stability under composition and base change |
| StandardSmoothCotangent.lean | Cotangent complex of submersive presentations; proves I/I² is S-free on classes of relations, H¹(L_{S/R}) = 0, Ω[S⁄R] is S-free with rank equal to dimension, section construction for cotangent complex; extends to standard smooth algebras and localization away |
| StandardSmoothOfFree.lean | Presentation-independent characterization: S is standard smooth iff H¹(S/R) = 0 and Ω[S⁄R] is free on {d sᵢ} for some sᵢ ∈ S; proves equivalence between étale and standard smooth of dimension 0; establishes that smoothness is local (smooth at prime iff standard smooth on some basic open) |
| IntegralClosure.lean | Proves smooth base change commutes with integral closure; establishes bijectivity of S ⊗[R] integralClosure R B → integralClosure S (S ⊗[R] B) for flat/smooth S |
| Local.lean | Jacobian criterion for smoothness of local algebras; formal smoothness equivalent to injectivity of cotangent complex base change to residue field |
| Field.lean | Smooth algebras over fields; separably generated extensions are formally smooth; finitely generated extensions over perfect fields are smooth |
| AdicCompletion.lean | Formally smooth algebras lift through adic completions; any map A →ₐ[R] S/I lifts to A →ₐ[R] S when S is I-adically complete; constructs sections of quotient projections using formal smoothness |
| Flat.lean | Proves smooth algebras are flat; uses adic completion and formal smoothness to construct retracts for Noetherian case, then applies Noetherian descent for general case |
| Locus.lean | Smooth locus of an algebra (primes where localization is formally smooth); proves locus is open, characterized by vanishing H¹ cotangent and free Kähler differentials; equivalence between basic open in smooth locus and smooth localization |
| NoetherianDescent.lean | Noetherian descent for smooth algebras; proves any smooth A-algebra B admits a model over a finitely generated ℤ-subalgebra A₀ of A with B ≃ₐ A ⊗[A₀] B₀ for smooth A₀-algebra B₀; extends to standard smooth of relative dimension and étale algebras |
| Pi.lean | Smooth algebras over product rings (finite products); establishes component-wise characterization |

## Subdirectories

(None)

## Search Tags

smooth formally-smooth finite-presentation Kaehler-differential cotangent-complex lifting-property square-zero nilpotent standard-smooth submersive-presentation relative-dimension Jacobian-criterion local-ring residue-field field-extension separably-generated perfect-field integral-closure base-change composition localization
