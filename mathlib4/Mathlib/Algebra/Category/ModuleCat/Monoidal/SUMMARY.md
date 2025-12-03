---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Category/ModuleCat/Monoidal
generated: 2025-12-02T12:15:00Z
git_sha: 91b78e4d87f6d8084f92183992611f2312971592
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# Monoidal

## Overview

The `Monoidal/` directory establishes the monoidal category structure on `ModuleCat R` (and `SemimoduleCat R`) using the tensor product as the monoidal product. It proves that modules form a monoidal category with associators and unitors derived from tensor product isomorphisms, then extends this to a braided and symmetric monoidal category via the tensor product commutativity, and finally constructs the monoidal closed structure where the internal hom is given by the linear hom-functor. This provides the complete enriched categorical structure needed for working with modules in a monoidal framework.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines monoidal category structure on `SemimoduleCat R` and `ModuleCat R` with tensor product ⊗ as monoidal product; constructs associators, left/right unitors, and whiskering operations; proves pentagon and triangle coherence axioms; provides `tensorLift` for constructing morphisms from tensor products and extensionality lemmas (`tensor_ext`, `tensor_ext₃`) for reasoning about tensor morphisms |
| Symmetric.lean | Constructs symmetric monoidal structure on modules via the braiding isomorphism `M ⊗ N ≅ N ⊗ M` from tensor product commutativity; proves hexagon coherence axioms and braiding naturality; defines `tensorμ` which permutes factors in nested tensor products `(A ⊗ B) ⊗ (C ⊗ D) → (A ⊗ C) ⊗ (B ⊗ D)` |
| Closed.lean | Establishes monoidal closed structure on `ModuleCat R` where the internal hom `ihom M` is the linear coyoneda functor (linear maps into M); constructs the adjunction `M ⊗ - ⊣ ihom M` with explicit curry/uncurry operations; describes evaluation and coevaluation maps for the closed structure |

## Subdirectories

(no subdirectories)

## Search Tags

monoidal-categories symmetric-monoidal braided-categories monoidal-closed tensor-products modules internal-hom associators unitors coherence-axioms pentagon triangle hexagon whiskering curry-uncurry adjunctions linear-algebra category-theory
