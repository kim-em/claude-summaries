---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/CategoryTheory/Preadditive/Injective
generated: 2025-12-07T23:17:00Z
git_sha: 8806fb490620c3ccc60e504c32aefda32944948b
git_branch: flexible-linter-simp-suggestions
status: complete
files_count: 4
subdirs_count: 0
---

# Injective

## Overview

The `Injective/` directory formalizes injective objects in category theory and their applications. An object `J` is injective if every morphism into `J` can be extended along any monomorphism. This includes the core definition of injective objects, categories with enough injectives (every object embeds into an injective object), injective resolutions (cochain complexes of injective objects quasi-isomorphic to a given object), preservation of injectivity by functors, and the dual relationship between injective objects in `C` and projective objects in `Cᵒᵖ`. The directory also establishes lifting property characterizations and shows how injective objects behave under products, biproducts, and adjunctions.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Core definitions of injective objects (extension property for monomorphisms), injective presentations (`X ⟶ J` with `J` injective), and categories with enough injectives; proves injectives are closed under products/biproducts, establishes duality with projective objects via opposite categories, and provides construction helpers like `Injective.under` for choosing canonical injective presentations |
| LiftingProperties.lean | Characterization of injective objects using lifting properties: proves `Injective I` iff the morphism `I ⟶ 0` has the right lifting property with respect to all monomorphisms (`injective_iff_rlp_monomorphisms_zero`) |
| Preserves.lean | Typeclass `Functor.PreservesInjectiveObjects` for functors mapping injective objects to injective objects; shows right adjoints of monomorphism-preserving functors preserve injectivity, with converse when codomain has enough injectives |
| Resolution.lean | Injective resolutions: ℕ-indexed cochain complexes `Z ⟶ I⁰ ⟶ I¹ ⟶ ...` of injective objects with a quasi-isomorphism from the single complex concentrated at `Z`; proves exactness properties and that the kernel of `I⁰ ⟶ I¹` is isomorphic to `Z` |

## Subdirectories

*(No subdirectories)*

## Search Tags

injective-objects injective-presentations enough-injectives injective-resolutions lifting-properties quasi-isomorphisms cochain-complexes homological-algebra monomorphisms extension-property preserves-injectives adjunctions opposite-category-duality kernels exactness
