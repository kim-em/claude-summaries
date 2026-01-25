---
source_path: /Users/kim/Documents/Jobs/ANU/2016/MATH1014/Notes/LinearAlgebra
generated: 2026-01-25T14:30:00Z
git_sha: fafb26e72fe7b535873cd5b8a8f359b75df7fe29
git_branch: master
status: complete
files_count: 9
subdirs_count: 25
---

# LinearAlgebra

## Overview

Complete LaTeX-based lecture notes for the linear algebra component of MATH1014 (Mathematics and Applications 2), taught by A/Prof Scott Morrison at ANU in Semester 2 2016. The 25 lectures form a comprehensive undergraduate linear algebra course, progressing from geometric vector operations in Euclidean space (Lectures 1-4) through abstract vector space theory and linear transformations (Lectures 5-9), eigenvalue theory and matrix diagonalization (Lectures 11-18), to orthogonality and inner product spaces (Lectures 19-23), culminating in applications including Markov chains, PageRank, and SVD (Lectures 10, 24). Each lecture includes LaTeX source, compiled slides and handout PDFs, and annotated "scribble" PDFs with handwritten notes from in-class presentations. Supporting materials include custom diagrams (created with OmniGraffle), Python/Mathematica examples, and a sophisticated build system that generates multiple output formats from shared source files.

## Key Files

| File | Purpose |
|------|---------|
| `MATH1014-LinearAlgebra.handout.pdf` | Combined handout PDF for all lectures (202 pages, too large to read) |
| `makefile` | Build system that generates slides and handout PDFs from lecture sources, with rsync upload to teaching server |
| `course.tex` | Course metadata and configuration (course name, instructor, timing) |
| `beamer-preamble.tex` | LaTeX preamble for Beamer presentation setup |
| `lecture.cls` | Custom LaTeX document class for lecture formatting |
| `local-defs.tex` | Local LaTeX macro definitions |
| `readme.txt` | Build instructions: `make files` to compile, `make post` to upload |
| `makefile.user` | User-specific makefile customizations |
| `ignore` | Build script utility (executable) |

## Subdirectories

- [x] `Lecture01/` - Administrative overview and course introduction
- [x] `Lecture02/` - Dot products and cross products of vectors
- [x] `Lecture03/` - Lines and planes in Euclidean space
- [x] `Lecture04/` - Distances in R³ (point-to-plane, point-to-line, line-to-line)
- [x] `Lecture05/` - Vector Spaces and Subspaces (formal axioms, examples, closure properties, span)
- [x] `Lecture06/` - Null spaces, column spaces, and linear transformations
- [x] `Lecture07/` - Linear independence, bases, and coordinate systems for abstract vector spaces
- [x] `Lecture08/` - Coordinate systems and change of basis
- [x] `Lecture09/` - Dimension theory, bases, rank-nullity theorem, row spaces
- [x] `Lecture10/` - Applications to Markov chains (stochastic matrices, probability vectors, steady-state analysis)
- [x] `Lecture11/` - Eigenvectors and eigenvalues (basic definitions, eigenspaces, triangular matrices)
- [x] `Lecture12/` - Characteristic equation, finding eigenvalues, similarity transformations, dynamical systems
- [x] `Lecture13/` - Mid-semester examination review covering problems from the 2013 exam
- [x] `Lecture14/` - Matrix diagonalization (similarity, factorization A=PDP^(-1), computing matrix powers)
- [x] `Lecture15/` - The Diagonalization Theorem with worked examples, eigenspace dimensions and multiplicities
- [x] `Lecture16/` - Matrix representations of linear transformations with respect to different bases, B-matrix notation, and connection to diagonalization
- [x] `Lecture17/` - Complex eigenvalues and eigenvectors (geometric interpretation as rotation and scaling)
- [x] `Lecture18/` - Discrete dynamical systems (matrix recurrence relations, predator-prey models, trajectory analysis)
- [x] `Lecture19/` - Inner products and orthogonality in Euclidean spaces
- [x] `Lecture20/` - Orthogonal and orthonormal sets, orthogonal bases, orthogonal matrices
- [x] `Lecture21/` - Orthogonal projections onto subspaces
- [x] `Lecture22/` - The Gram-Schmidt Process for converting arbitrary bases into orthogonal and orthonormal bases, with QR matrix factorization
- [x] `Lecture23/` - The Least Squares Problem (best approximation for inconsistent systems, normal equations A^T A x̂ = A^T b)
- [x] `Lecture24/` - Markov chains, text generation, PageRank algorithm, and SVD image compression with Python/Mathematica examples
- [x] `Lecture25/` - Final revision session with 13 comprehensive practice problems covering all semester topics (change of basis, eigenvalues, diagonalization, dynamical systems, Markov chains, orthogonal projections)

## Search Tags

math1014 linear-algebra beamer latex teaching lecture-notes anu 2016 semester2 scott-morrison makefile slides handouts vector-spaces eigenvalues eigenvectors
