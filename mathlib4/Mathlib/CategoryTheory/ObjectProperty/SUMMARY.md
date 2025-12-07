---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/ObjectProperty
generated: 2025-12-07T10:15:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: preliminary
files_count: 23
subdirs_count: 1
---

# ObjectProperty

## Overview

The `ObjectProperty/` directory provides a comprehensive framework for working with properties of objects in categories, treating them as predicates `C → Prop` equipped with rich structure. It defines the `ObjectProperty C` type as an abbreviation for `C → Prop`, establishes that properties form a complete lattice, and develops theory for closure operations (under isomorphisms, limits, colimits), smallness conditions, and interactions with functors. This infrastructure enables formal reasoning about subcategories defined by properties (e.g., "objects that are limits of small objects" or "objects closed under finite colimits"), with applications to accessible categories, presentability, and Grothendieck's axioms in abelian categories.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions: `ObjectProperty C` as `C → Prop`, typeclass `P.Is X`, singleton/pair properties, inverse image and essential image under functors |
| ClosedUnderIsomorphisms.lean | Typeclass `P.IsClosedUnderIsomorphisms` and isomorphism closure operation `P.isoClosure` with closure properties |
| CompleteLattice.lean | Proof that `ObjectProperty C` forms a complete lattice with inf/sup/iSup operations and stability under isomorphism closure |
| LimitsOfShape.lean | `P.limitsOfShape J` and `P.strictLimitsOfShape J` for objects that are limits of diagrams satisfying `P`, typeclass `P.IsClosedUnderLimitsOfShape J` |
| ColimitsOfShape.lean | Dual to LimitsOfShape: `P.colimitsOfShape J` and `P.strictColimitsOfShape J`, typeclass `P.IsClosedUnderColimitsOfShape J`, duality with opposite category |
| LimitsClosure.lean | Closure of property under limits: `P.limitsClosure` as supremum over all limit shapes, stability properties |
| ColimitsClosure.lean | Closure of property under colimits: `P.colimitsClosure` as supremum over all colimit shapes |
| ColimitsCardinalClosure.lean | Closure under colimits indexed by categories with bounded cardinality of arrows (κ-accessible objects) |
| Small.lean | Smallness of properties: `ObjectProperty.Small.{w} P` as `Small.{w} (Subtype P)`, essential smallness via isomorphism closure, equivalence characterizations |
| HasCardinalLT.lean | Property of objects with cardinality strictly less than a cardinal κ, used for accessibility and presentability |
| Ind.lean | Ind-objects as supremum of colimits of shape `J` for filtered categories `J` |
| Equivalence.lean | Behavior of properties under category equivalences, functorial operations on properties |
| Opposite.lean | Opposite and unop operations for properties in opposite categories with preservation results |
| Retract.lean | Objects that are retracts of objects satisfying a property, closure under retracts |
| EpiMono.lean | Properties related to epimorphisms and monomorphisms (likely interaction with object properties) |
| Orthogonal.lean | Orthogonality between object properties (likely lifting property formulations) |
| InheritedFromHom.lean | Properties inherited from morphism properties (e.g., object satisfies P if identity morphism satisfies a hom-property) |
| FullSubcategory.lean | Full subcategory defined by an object property with inclusion functor and universal properties |
| ContainsZero.lean | Properties that contain the zero object (in pointed categories or categories with zero objects) |
| Extensions.lean | Extensions of properties along functors or inclusions |
| Local.lean | Local properties of objects (satisfied in neighborhoods or under certain conditions) |
| SiteLocal.lean | Properties that are local in the sense of Grothendieck topologies and sheaf conditions |
| Shift.lean | Behavior of properties under shift functors in graded/triangulated categories |

## Subdirectories

- [ ] `FunctorCategory/` - Properties of functors viewed as objects in functor categories (pending)

## Search Tags

object-properties category-theory predicates closure-operations limits colimits isomorphisms full-subcategory accessibility presentable-categories small-objects essentially-small complete-lattice functor-categories grothendieck-axioms
