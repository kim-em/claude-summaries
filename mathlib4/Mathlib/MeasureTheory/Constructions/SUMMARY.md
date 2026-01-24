---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/MeasureTheory/Constructions
generated: 2026-01-25T22:15:00Z
git_sha: 542a7d7979ad5f45d2a89008412e565c8fa001d2
git_branch: heads/nightly-testing
status: preliminary
files_count: 9
subdirs_count: 2
---

# Constructions

## Overview

The `Constructions/` directory provides foundational constructions for building measures on complex spaces from simpler components. It includes product measures for finite and countable families of spaces, projective limits of measure families, generalized polar coordinate changes for normed spaces, and cylinder-based measure theory. The folder also contains specialized measurable space instances for quotient modules, additive characters, and the unit interval with its canonical probability measure.

## Key Files

| File | Purpose |
|------|---------|
| Pi.lean | Product measures on indexed families: defines `Measure.pi` for finitely many σ-finite measures on `(i : ι) → α i`, constructs iterated products via `tprod`, proves product measures satisfy `μ (pi univ s) = ∏ i, μ i (s i)`, supports Fubini/Tonelli theorems via marginal construction |
| HaarToSphere.lean | Generalized polar coordinate changes: for Haar measure `μ` on normed space `E`, constructs `μ.toSphere` on the unit sphere such that `μ` factors as product of sphere measure and radial measure with density `r^n`, provides integral rewriting for norm-only functions, estimates sphere measures |
| Projective.lean | Projective measure families and limits: defines `IsProjectiveMeasureFamily` for families `P : ∀ J : Finset ι, Measure (∀ j : J, α j)` where projections preserve measures, defines `IsProjectiveLimit μ P` for limits, proves uniqueness of projective limits for finite measure families |
| Cylinders.lean | π-systems of cylinders and square cylinders: defines `cylinder s S` as product of set on finite indices with `univ` elsewhere, defines `squareCylinders` and `measurableCylinders`, proves these generate the product σ-algebra, establishes π-system properties for measure construction |
| ClosedCompactCylinders.lean | Cylinders with closed compact bases: defines `closedCompactCylinders X` for Kolmogorov extension theorem, proves closed compact cylinders are measurable in second-countable spaces with measurable opens |
| ProjectiveFamilyContent.lean | Additive content from projective families: constructs `projectiveFamilyContent` on measurable cylinders from projective measure family `P`, proves measurable cylinders form a set algebra, provides foundation for projective limit construction via Ionescu-Tulcea and Kolmogorov extension theorems (not yet in mathlib) |
| UnitInterval.lean | Canonical measure on unit interval: provides `MeasureSpace` instance on `unitInterval` as probability measure with no atoms, proves volume formulas for intervals `Icc`, `Ico`, `Ioc`, `Ioo` and variants, establishes measure-preserving properties of symmetry map |
| AddChar.lean | Measurable space for additive characters: endows `AddChar A M` with discrete measurable space structure for finite discrete `A` |
| SubmoduleQuotient.lean | Measurability on quotient modules: provides `MeasurableSpace` instance for `M ⧸ p` (quotient of module by submodule), inherits discrete measurability |

## Subdirectories

- [x] `BorelSpace/` - Borel space constructions and properties
- [x] `Polish/` - Polish space measure theory

## Search Tags

product-measure pi-measure projective-limit projective-family haar-measure sphere-measure polar-coordinates cylinder measure-construction unit-interval probability-measure additive-character quotient-module borel-space polish-space kolmogorov-extension ionescu-tulcea fubini tonelli marginal
