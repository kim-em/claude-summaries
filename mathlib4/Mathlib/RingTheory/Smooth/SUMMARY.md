---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/Smooth
generated: 2026-02-01T22:45:00Z
git_sha: 5cb27be88dd78e9476463c255b7852485b175fb7
git_branch: master
status: preliminary
files_count: 13
subdirs_count: 0
---

# Smooth

## Overview

The `Smooth/` directory contains the formalization of smooth algebras and morphisms in commutative algebra. This includes formally smooth algebras (characterized by projective Kähler differentials and vanishing first cotangent cohomology), the standard lifting property for nilpotent ideals, standard smooth algebras (those admitting submersive presentations), and specialized results for smooth algebras over fields, local rings, and in relation to integral closure. The theory establishes smooth as the combination of formally smooth and finite presentation, and proves stability under composition, base change, and localization.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definition of formally smooth and smooth algebras; proves equivalence with lifting property for square-zero ideals; establishes stability under isomorphisms, composition, base change, and localization |
| Kaehler.lean | Establishes correspondence between retractions of cotangent maps and algebra sections; proves formal smoothness is equivalent to split injectivity of I/I² → S ⊗[P] Ω[P⁄R] |
| StandardSmooth.lean | Standard smooth algebras (those with submersive presentations); relative dimension; stability under composition and base change |
| StandardSmoothCotangent.lean | (Content not examined in detail) |
| StandardSmoothOfFree.lean | (Content not examined in detail) |
| IntegralClosure.lean | Proves smooth base change commutes with integral closure; establishes bijectivity of S ⊗[R] integralClosure R B → integralClosure S (S ⊗[R] B) for flat/smooth S |
| Local.lean | Jacobian criterion for smoothness of local algebras; formal smoothness equivalent to injectivity of cotangent complex base change to residue field |
| Field.lean | Smooth algebras over fields; separably generated extensions are formally smooth; finitely generated extensions over perfect fields are smooth |
| AdicCompletion.lean | (Content not examined in detail) |
| Flat.lean | (Content not examined in detail) |
| Locus.lean | (Content not examined in detail) |
| NoetherianDescent.lean | (Content not examined in detail) |
| Pi.lean | (Content not examined in detail) |

## Subdirectories

(None)

## Search Tags

smooth formally-smooth finite-presentation Kaehler-differential cotangent-complex lifting-property square-zero nilpotent standard-smooth submersive-presentation relative-dimension Jacobian-criterion local-ring residue-field field-extension separably-generated perfect-field integral-closure base-change composition localization
