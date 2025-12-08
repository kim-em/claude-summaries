---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Analysis/Normed/Order
generated: 2025-12-05T15:00:00Z
git_sha: 488d631b358e81211d82bcf1c4422dd1e2b08702
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 3
subdirs_count: 1
---

# Order

## Overview

The `Order/` directory provides a comprehensive bridge between normed structures and ordered structures in mathlib4. At its core, it defines classes for ordered normed spaces that avoid type class diamonds, and introduces the theory of normed lattice ordered groups with solid norms—a framework motivated by Banach lattice theory where the norm respects the lattice order. The directory studies the topological properties of upper, lower, and order-connected sets in normed groups, proving continuity and closure results for lattice operations and providing specialized lemmas for ℝⁿ to support measurability proofs. Additionally, the `Hom/` subdirectory provides constructions that upgrade algebraic group structures to (semi)normed groups using group norm homomorphisms, including specialized support for nonarchimedean (ultrametric) normed groups that satisfy the stronger ultrametric triangle inequality.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Minimal module defining ordered normed spaces as structures that are both normed and ordered, primarily to avoid type class inference diamonds |
| Lattice.lean | Defines normed lattice ordered groups with solid norms (HasSolidNorm class where \|a\| ≤ \|b\| implies ‖a‖ ≤ ‖b‖); proves that normed lattice ordered groups are topological lattices; shows continuity of inf/sup operations and Lipschitz continuity of posPart/negPart; provides OrderClosedTopology instance |
| UpperLower.lean | Studies upper/lower/order-connected sets in normed groups; proves that topological closure and interior preserve upper/lower set properties; provides specialized lemmas for ℝⁿ (product spaces) including distance monotonicity and ball approximations for upper/lower sets; proves closure of upper/lower closures when bounded |

## Subdirectories

- [x] `Hom/` - Constructs (semi)normed groups from (semi)normed homomorphisms; upgrades Group to SeminormedGroup/NormedGroup using GroupSeminormClass/GroupNormClass when codomain is ℝ; includes nonarchimedean (ultrametric) normed group constructions

## Search Tags

ordered-normed-spaces normed-lattices solid-norm banach-lattices topological-lattices upper-sets lower-sets order-connected-sets closure-interior lipschitz-continuity positive-part negative-part real-product-spaces group-seminorms group-norms ultrametric nonarchimedean ordered-structures
