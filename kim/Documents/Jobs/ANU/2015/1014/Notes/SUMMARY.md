---
source_path: /Users/kim/Documents/Jobs/ANU/2015/1014/Notes
generated: 2025-12-04T07:30:00Z
git_sha: 48a99ef1be36fc0c3cca2af4518f1aebb71ec697
git_branch: master
status: complete
files_count: 7
subdirs_count: 25
---

# Notes

## Overview

Complete lecture materials for MATH1014 (Mathematics and Applications 2) semester 2 2015, comprising 25 lectures that form a comprehensive first-year linear algebra course at ANU. The course progresses systematically from concrete geometric concepts (vectors, lines, and planes in ℝ³) through abstract vector space theory (subspaces, linear independence, bases, dimension) to advanced topics (eigenvalues, diagonalization, orthogonality, least squares). Special applications include Markov chains, dynamical systems, and SVD image compression. Each lecture contains professionally crafted LaTeX source with beamer presentations, worked examples, and supporting geometric diagrams (over 200 diagrams total across lectures). A sophisticated build infrastructure with custom LaTeX document classes, shared notation macros, and automated make/latexmk compilation generates both presentation slides and 3-up handouts, with automated posting to the tqft.net teaching website.

## Key Files

| File | Purpose |
|------|---------|
| `makefile` | Complex build script that compiles all 25 lectures into slides and handouts, creates combined handout PDF, and posts to tqft.net website (2.7KB with automatic symbolic link creation and latexmk integration) |
| `beamer-preamble.tex` | Shared LaTeX preamble for beamer presentations (2.2KB with package imports for babel, graphics, AMS math, multicol) |
| `lecture.cls` | Custom LaTeX document class for lecture slides with automatic type detection (beamer/handout/slides) based on filename (2.4KB) |
| `local-defs.tex` | Mathematical notation macro definitions including vector commands (\vecx, \vecy), boldface shortcuts (\bi, \bj, \bk), and blackboard bold (\bR, \bZ, \bC) (3.3KB) |
| `course.tex` | Course metadata file defining MATH1014 title, instructor (Dr Scott Morrison), timing (Second Semester 2015), and institution (ANU MSI) (652 bytes) |
| `readme.txt` | Build instructions: 'make files' to recompile PDFs, 'make post' to upload to tqft.net (200 bytes) |
| `ignore` | Bash script for SVN version control that sets svn:ignore properties on LaTeX auxiliary files (aux, log, out, PDF, etc.) in all lecture directories (873 bytes) |

## Subdirectories

- [x] `Lecture01/` - First lecture: Administrative overview and introduction to vectors, coordinates, and geometry in ℝ³, with 42 supporting diagrams (complete)
- [x] `Lecture02/` - Second lecture: Vector multiplication operations (dot product and cross product in ℝ³), including scalar/vector projections and applications (complete)
- [x] `Lecture03/` - Third lecture: Lines and planes in Euclidean space (vector/parametric/symmetric equations for lines, vector/scalar equations for planes using normal vectors) with professionally crafted 3D geometric diagrams
- [x] `Lecture04/` - Fourth lecture on distances in ℝ³ (point-to-plane, point-to-line, line-to-line) with comprehensive 25KB examples file containing 12 worked problems and 16 exercises, supported by 25 vector diagrams in multiple formats (complete)
- [x] `Lecture05/` - Fifth lecture introducing abstract vector spaces and subspaces in MATH1014, with supporting diagrams illustrating geometric concepts (complete)
- [x] `Lecture06/` - Sixth lecture on null spaces, column spaces, and linear transformations (kernel and range) in abstract vector spaces, with 5 detailed worked examples (complete)
- [x] `Lecture07/` - Seventh lecture on linear independence and bases for abstract vector spaces (linear independence definitions, spanning set theorem, algorithms for bases of Nul A and Col A, unique representation theorem, coordinates) (complete)
- [x] `Lecture08/` - Eighth lecture on coordinate systems and change of basis (isomorphisms, coordinate mappings, change-of-coordinate matrices P_{C←B}, worked examples in ℝ², P₂, and M_{2×2}) (complete)
- [x] `Lecture09/` - Ninth lecture on dimension theory for vector spaces (dimension definitions, Basis Theorem, Rank Theorem rank(A) + dim(Nul A) = n, row spaces with dim(Row A) = rank(A), Invertible Matrix Theorem extensions) with Hermite polynomial quantum mechanics example (complete)
- [x] `Lecture10/` - Tenth lecture on applications of linear algebra to Markov chains: stochastic matrices, probability vectors, steady-state vectors, transition matrices, regular stochastic matrices, and convergence theorem with bird aviary, Land of Oz weather, and rat cage examples (complete)
- [x] `Lecture11/` - Eleventh lecture introducing eigenvectors and eigenvalues: definitions, eigenspaces as null spaces, triangular matrix eigenvalue theorem, linear independence of eigenvectors with distinct eigenvalues, with worked examples finding eigenspace bases (complete)
- [x] `Lecture12/` - Mid-semester examination review lecture covering worked solutions to 2013 exam questions (lines/planes, bases/coordinates, vector spaces, linear transformations, matrix subspaces) plus thematic revision questions, with Markov chains computational examples (complete)
- [x] `Lecture13/` - Thirteenth lecture on eigenvalues and eigenvectors: characteristic equation (det(A - λI) = 0), similarity transformations, and dynamical systems applications with Maple computational examples (complete)
- [x] `Lecture14/` - Fourteenth lecture on matrix diagonalization: definition of diagonalizable matrices, diagonalization theorem A = PDP⁻¹, computing matrix powers using diagonalization, connection between eigenvectors and change of basis (complete)
- [x] `Lecture15/` - Fifteenth lecture on advanced diagonalization theory with worked examples including non-diagonalizable matrices, eigenspace dimension theorem, and change of basis interpretation (complete)
- [x] `Lecture16/` - Sixteenth lecture on matrix representations of linear transformations relative to arbitrary bases, connecting diagonalization to diagonal B-matrix representations (complete)
- [x] `Lecture17/` - Seventeenth lecture on complex eigenvalues and eigenvectors for real matrices, rotation-scaling decomposition A = PCP⁻¹, with complex numbers addendum and 8 geometric diagrams (complete)
- [x] `Lecture18/` - Eighteenth lecture on discrete linear dynamical systems with eigenvalue-based trajectory analysis (attractors, repellors, saddle points, spirals) and predator-prey/population modeling examples, supported by 16 mathematical and ecological diagrams (complete)
- [x] `Lecture19/` - Nineteenth lecture on inner products and orthogonality (dot product, vector length, orthogonal complements, dimension theorem dim(W) + dim(W⊥) = n, vector decomposition into W + W⊥) (complete)
- [x] `Lecture20/` - Twentieth lecture on orthogonal and orthonormal sets (orthogonal set definitions, linear independence theorem, orthogonal basis coordinate formulas, orthonormal sets, orthogonal matrices with U^TU = I property) (complete)
- [x] `Lecture21/` - Twenty-first lecture on orthogonal projections onto subspaces (Orthogonal Decomposition Theorem, Best Approximation Theorem, projection matrix UU^T, with 4 geometric diagrams) (complete)
- [x] `Lecture22/` - Twenty-second lecture on Gram-Schmidt orthogonalization and QR matrix factorization with six worked examples and supporting geometric diagrams (complete)
- [x] `Lecture23/` - Twenty-third lecture on the Least Squares Problem (finding best approximations to inconsistent linear systems via normal equations A^TA x̂ = A^T b) (complete)
- [x] `Lecture24/` - Twenty-fourth lecture on Markov chains for text prediction/generation and SVD for image compression, with Mathematica notebook and Python implementations (complete)
- [x] `Lecture25/` - Final lecture containing comprehensive revision questions and solutions covering all major course topics: change of basis, eigenvalues/eigenvectors, diagonalization, complex eigenvalues, dynamical systems, Markov chains, orthogonal projections, linear transformations on abstract vector spaces, and differential operators (complete)

## Search Tags

math1014 linear-algebra lecture-notes anu 2015 semester-2 beamer latex slides handouts pdf-generation build-system makefile latexmk scott-morrison mathematics first-year teaching
