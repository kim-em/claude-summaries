---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/RingTheory/LocalProperties
generated: 2026-02-01T10:15:00Z
git_sha: 6d1f75c8fd1461c972d4681f9cd70ab711a346b3
git_branch: feat-affine-convex-space
status: complete
files_count: 7
subdirs_count: 0
---

# LocalProperties

## Overview

This directory formalizes the theory of local properties of commutative rings and modules - properties that can be verified by checking them at localizations (at maximal ideals or on covering spans). It provides a systematic framework for defining when a property is "local" and proves that several important algebraic properties (reducedness, integral closure, projectivity, exactness) satisfy this locality criterion. The key insight is that many global properties of rings, modules, and ring homomorphisms can be detected by checking them on stalks at maximal ideals or on standard open covers.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of local properties for rings and ring homomorphisms: `LocalizationPreserves`, `OfLocalizationMaximal`, `RingHom.PropertyIsLocal`, `RingHom.OfLocalizationSpan`; includes theorems about when ideal properties can be checked locally |
| Submodule.lean | Local properties for modules and submodules: membership, equality, triviality, and module equality can be checked on stalks at maximal ideals or on spanning sets |
| Exactness.lean | Proves that injectivity, surjectivity, bijectivity, and exactness of linear maps are local properties; can be verified at maximal ideal localizations or on standard covers |
| Projective.lean | Shows that projectivity is a local property for finitely presented modules; includes results on free modules, rank preservation under localization, and split surjectivity checking on stalks |
| IntegrallyClosed.lean | Proves that `IsIntegrallyClosed` is a local property; an integral domain is integrally closed if its localization at each maximal ideal is integrally closed |
| Reduced.lean | Proves that `IsReduced` (no nonzero nilpotent elements) is preserved by localization and can be checked at maximal ideals |
| Semilocal.lean | Local properties specific to semilocal rings (rings with finitely many maximal ideals): finite modules, Noetherian rings, and PIDs can be detected locally |

## Subdirectories

(none)

## Search Tags

local-property localization maximal-ideal prime-ideal stalk covering-span RingHom PropertyIsLocal LocalizationPreserves OfLocalizationMaximal OfLocalizationSpan reduced integrally-closed projective exactness injectivity surjectivity bijective semilocal Noetherian PID finitely-presented module submodule
