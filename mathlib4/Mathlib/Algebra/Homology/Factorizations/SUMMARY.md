---
source_path: /Users/kim/projects/lean/mathlib4/Mathlib/Algebra/Homology/Factorizations
generated: 2025-12-02T09:15:00Z
git_sha: addb2cace4e59e6d4b7b62f2e4e1503626f0e30d
git_branch: master
status: complete
files_count: 2
subdirs_count: 0
---

# Factorizations

## Overview

The `Factorizations/` directory develops factorization lemmas for morphisms in the category of bounded below cochain complexes, which are essential components of a model category structure. It defines the class of fibrations (`degreewiseEpiWithInjectiveKernel`) and proves the CM5b factorization axiom: any morphism between bounded below cochain complexes in an abelian category with enough injectives can be factored through a monomorphism followed by a trivial fibration (quasi-isomorphism that is also an epimorphism with degreewise injective kernel). This work supports the identification of the bounded below derived category with the homotopy category of injective complexes, crucial for total derived functor construction.

## Key Files

| File | Purpose |
|------|---------|
| Basic.lean | Defines `degreewiseEpiWithInjectiveKernel` morphism property for cochain complexes: requires each degree-wise morphism to be an epimorphism with injective kernel; proves this class is multiplicative (closed under composition and contains identities); intended as fibration class for model structure |
| CM5b.lean | Proves the CM5b factorization lemma: any morphism `f : K ⟶ L` of bounded below cochain complexes factors as `i ≫ p` where `i` is a monomorphism and `p` is a quasi-isomorphism with `degreewiseEpiWithInjectiveKernel`; constructs factorization via auxiliary complex `I K` with zero differentials and injective objects, using mapping cone and biproduct constructions |

## Subdirectories

None - this is a leaf directory.

## Search Tags

factorization model-category fibration cofibration CM5b quasi-isomorphism bounded-below cochain-complex injective-kernel degreewise-epi mapping-cone homotopy-equivalence derived-functor abelian-category enough-injectives trivial-fibration
