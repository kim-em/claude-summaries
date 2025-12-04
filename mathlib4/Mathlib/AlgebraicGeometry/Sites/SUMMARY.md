---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/AlgebraicGeometry/Sites
generated: 2025-12-04T12:45:00Z
git_sha: 453cce856d41bd2715d9055ecdc877015033095f
git_branch: heads/nightly-testing
status: complete
files_count: 7
subdirs_count: 0
---

# Sites

## Overview

The `Sites/` directory formalizes Grothendieck topologies and sites for algebraic geometry, providing the categorical framework for sheaf theory on schemes. It defines the big Zariski and étale sites as Grothendieck topologies on the category of all schemes, small sites on categories of schemes over a fixed base, and the small affine Zariski site using only affine open sets. The directory establishes the fundamental machinery for defining coverings via morphism properties, proving subcanonicity of the Zariski topology, and constructing equivalences between different sheaf categories.

## Key Files

| File | Purpose |
|------|---------|
| MorphismProperty.lean | Defines precoverages and joint surjectivity conditions for morphism properties, establishing the framework for constructing sites from properties like open immersions and étale morphisms |
| Pretopology.lean | Constructs pretopologies and Grothendieck topologies from morphism properties, showing that the topology agrees with jointly surjective P-covers and providing monotonicity lemmas |
| BigZariski.lean | Defines the big Zariski site (Grothendieck topology on all schemes) where coverings are jointly surjective families of open immersions, proves subcanonicity via gluing morphisms |
| Etale.lean | Defines the big and small étale sites using étale morphisms as covering families, establishes that Zariski topology refines étale topology |
| Small.lean | Constructs small sites on Over S and P.Over ⊤ S categories, defining overPretopology and smallPretopology where coverings are P-covers of S-schemes, with induced topologies from the big site |
| SmallAffineZariski.lean | Defines the small affine Zariski site X.AffineZariskiSite with affine opens and basic open morphisms, characterizes coverings via ideal generators (Ideal.span s = ⊤), proves equivalence with sheaves on X.Opens |
| Representability.lean | Proves that locally representable sheaves are representable: if F is a sheaf with locally surjective family of relatively representable open immersions, then F is representable via gluing construction (Stacks 01JJ) |

## Subdirectories

(none)

## Search Tags

grothendieck-topology sites zariski-topology etale-topology pretopology morphism-property coverings sheaves big-site small-site affine-zariski open-immersion jointly-surjective subcanonical representability gluing descent categorical-topology
