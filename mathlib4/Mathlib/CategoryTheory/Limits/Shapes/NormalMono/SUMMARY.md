---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Limits/Shapes/NormalMono
generated: 2025-12-07T12:30:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 2
subdirs_count: 0
---

# NormalMono

## Overview

The `NormalMono/` directory formalizes normal monomorphisms and normal epimorphisms in category theory. A normal monomorphism is a morphism that is the kernel of some other morphism (dually, a normal epimorphism is the cokernel of some morphism). The directory establishes that normal monos/epis are special cases of regular monos/epis, proves that equivalences reflect normality, shows that pullbacks of normal monos are normal, and defines categories where all monos/epis are normal. The second file proves that normal mono categories with finite products and kernels have all equalizers (and dually for normal epi categories).

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of NormalMono and NormalEpi classes, universal lifting properties, proofs that normal implies regular, pullback/pushout preservation, and IsNormalMonoCategory/IsNormalEpiCategory typeclasses |
| Equalizers.lean | Proves that normal mono categories with finite products and kernels have all equalizers (and dually normal epi categories with coproducts and cokernels have coequalizers), by constructing equalizers from kernels of product morphisms |

## Subdirectories

(none)

## Search Tags

normal-monomorphism normal-epimorphism kernel cokernel regular-monomorphism regular-epimorphism equalizers coequalizers finite-products finite-coproducts pullback-preservation pushout-preservation normal-mono-category normal-epi-category abelian-categories
