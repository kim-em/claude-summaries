---
source_path: /Users/kim/Documents/Jobs/ANU/2015/1014/OldMaterial/JELLecturesSem1_2015
generated: 2025-12-05T13:45:00Z
git_sha: 48a99ef1be36fc0c3cca2af4518f1aebb71ec697
git_branch: master
status: complete
files_count: 5
subdirs_count: 29
---

# JELLecturesSem1_2015

## Overview

Complete archival collection of Joan Licata's (JEL) Semester 1 2013/2015 MATH1014 (Mathematics and Applications 2 - Algebra) lecture materials, later adapted by Scott Morrison for Semester 2 2015. This is a comprehensive, professionally-developed linear algebra course featuring 23 main lectures plus a capstone applications lecture, structured around Lay's Linear Algebra textbook. The materials showcase a modern pedagogical approach combining theoretical rigor with extensive computational exploration (28 Maple worksheets using the custom `laylinalg` package) and real-world applications (cryptography, network flow, economic modeling, error-correcting codes).

The course progression follows a carefully scaffolded curriculum: geometric foundations in R³ (dot products, cross products, lines, planes, distances) → abstract vector spaces and subspaces → linear independence and bases → eigenvalue theory and diagonalization → applications to Markov chains and dynamical systems → inner products and orthogonality → least squares and Gram-Schmidt. Each lecture directory contains LaTeX source, Beamer presentations (both screen and print-friendly 4-per-page versions), Graffle diagrams, and compiled PDFs. The collection includes robust assessment support with practice problems from Lay's textbook (organized in LayExams/), comprehensive revision materials covering the full syllabus, and detailed case studies linking theory to applications. The materials demonstrate some organizational artifacts (lecture numbering inconsistencies, multiple file versions marked "redo") reflecting iterative course development.

## Key Files

| File | Purpose |
|------|---------|
| `Notes.tex` | Main LaTeX document that compiles all lecture notes into a single PDF booklet for "Math1014 Linear Algebra Notes 2012 Semester 1" |
| `RobertsInfo.tex` | Course information Beamer presentation including syllabus, textbook requirements (Lay's Linear Algebra), WebAssign quiz system, and resource links |
| `course.tex` | Course metadata defining instructor (Dr Scott Morrison), institution (ANU), and timing (Second Semester 2015) - updated from original JEL version |
| `beamer-preamble.tex` | Common Beamer presentation configuration using Boadilla theme, shared across all lecture slides |
| `local-defs.tex` | LaTeX macro definitions for mathematical notation (vectors, spaces, operators) used throughout all lecture materials |

## Subdirectories

- [x] `CaseStudies/` - 17 application-oriented case study files focusing on practical uses of linear algebra: detailed exercises on Hill cipher cryptography (mod 26 arithmetic), Hamming (7,4) error-correcting codes over Z₂, Fibonacci/Lucas sequences via eigenvalues, SVD applications, plus PDFs from Lay textbook sections and supplementary materials
- [x] `David/` - Lecture materials for Lectures 13-14 covering Markov chains and eigenvectors/eigenvalues, possibly contributed by a different instructor or TA named David
- [x] `LayExams/` - Practice exam problems extracted from Lay's Linear Algebra textbook with detailed step-by-step solutions: Second Exam, Third Exam, and Final Exam versions providing comprehensive problem sets aligned with course content
- [x] `Lecture01/` - Course introduction and preliminaries: syllabus overview, LaTeX source, Beamer presentations (screen and print versions), OmniGraffle diagrams establishing course structure and expectations
- [x] `Lecture02/` - Geometric foundations in R³: dot product properties and applications, cross product definition and geometric interpretation, with worked examples and visual diagrams
- [x] `Lecture03/` - Vector equations for lines and planes in R³: parametric and symmetric forms, plane equations via normal vectors, cross product applications, distance formulas, with LaTeX source and presentation materials
- [x] `Lecture04/` - Advanced geometric distances in R³: point-to-plane (projection formula), point-to-line (cross product method), line-to-line distances (skew and parallel cases), with physics/engineering application examples
- [x] `Lecture05/` - Transition to abstract vector spaces: formal ten axioms defining vector spaces, diverse examples (matrix spaces, polynomial spaces, function spaces), subspace definition via closure properties, span construction, introduction to column spaces
- [x] `Lecture06/` - Fundamental matrix subspaces: null space as kernel, column space as range, linear transformations between abstract vector spaces, one-to-one and onto properties, connecting concrete matrices to abstract theory
- [x] `Lecture07/` - Linear independence and bases: formal definitions, Spanning Set Theorem, computational algorithms for finding bases of null spaces and column spaces via row reduction, Unique Representation Theorem, coordinate systems in general vector spaces
- [x] `Lecture08/` - Change of basis machinery: vector space isomorphisms, change-of-coordinate matrices P[C←B], two algorithmic approaches (direct computation and factoring through standard basis), applications to simplifying computations
- [x] `Lecture09*(redo)/` - Dimension theory: dimension as cardinality of basis, Rank Theorem relating column space and null space dimensions, marked "(redo)" indicating this lecture was revised or corrected after initial version
- [x] `Lecture10/` - Introduction to eigenvalue theory (Lay §5.1): eigenvectors and eigenvalues defined, comprehensive revision of vector spaces/bases/geometry from earlier lectures, three Maple worksheets (map1301-map1303) demonstrating matrix iteration T^7, T^15, T^20 converging to steady states, exhibits lecture numbering confusion (files labeled "Lecture11" and "LA13" within "Lecture10" directory)
- [x] `Lecture11/` - Markov chains application (Lay §5.2): steady-state vectors, probability interpretation, regular stochastic matrices, rat cage population example with OmniGraffle diagram, contains duplicate source files reflecting organizational inconsistencies
- [x] `Lecture12/` - Eigenvalue theory fundamentals: formal definitions, eigenspaces characterized as null spaces Nul(A - λI), Triangular Matrix Theorem (diagonal entries are eigenvalues), Linear Independence Theorem for eigenvectors with distinct eigenvalues
- [x] `Lecture13/` - Characteristic equation and computational methods: det(A - λI) = 0 for finding eigenvalues, similarity transformations preserving eigenvalues, applications to dynamical systems, includes Maple computational examples
- [x] `Lecture14/` - Matrix diagonalization theory and criteria: Diagonalization Theorem (A = PDP⁻¹ with eigenvector columns), necessary and sufficient conditions (n linearly independent eigenvectors), worked examples demonstrating when matrices are/aren't diagonalizable based on eigenspace dimensions
- [x] `Lecture15/` - Coordinate-free linear algebra: matrix representations of linear transformations T: V → W relative to bases B and C, showing [T(x)]C = [T]C←B[x]B, demonstrating how basis choice affects matrix form and connecting to diagonalization as optimal basis choice (Lay §5.4)
- [x] `Lecture16/` - Complex eigenvalues (Lay §5.5): computing eigenvalues with complex roots a±bi, geometric interpretation as rotation (angle θ = arctan(b/a)) combined with scaling (factor r = √(a²+b²)), real matrix factorization A = PCP⁻¹ with rotation matrix C, normal forms for 2×2 matrices
- [x] `Lecture17/` - Discrete dynamical systems (Lay §5.6): difference equations xₖ₊₁ = Axₖ solved via eigenvalue decomposition, trajectory analysis based on eigenvalue magnitudes, predator-prey ecological models, equilibrium point classification (attractors |λ|<1, repellors |λ|>1, saddle points, spirals from complex eigenvalues)
- [x] `Lecture18/` - Inner products and orthogonality foundations (Lay §6.1): dot product review and properties, vector length ‖v‖ = √(v·v), normalization to unit vectors, orthogonal vectors and orthogonal complements, Fundamental Theorem relating row space and null space as orthogonal complements
- [x] `Lecture19/` - Orthogonal bases (Lay §6.2): orthogonal sets definition, Orthogonal Set Theorem (automatic linear independence), orthonormal bases, coordinate computation via dot products ([x]B has entries x·uᵢ), orthogonal matrices Q (columns form orthonormal basis, Q⁻¹ = Qᵀ, length/angle preservation)
- [x] `Lecture20/` - Orthogonal projections (Lay §6.3): projection onto subspace W as closest point, Orthogonal Decomposition Theorem (y = ŷ + z with ŷ ∈ W, z ∈ W⊥), Best Approximation Theorem, projection matrix formula P = UUᵀ when U has orthonormal columns spanning W
- [x] `Lecture21/` - Gram-Schmidt process and QR factorization (Lay §6.4): algorithm for converting basis {x₁,...,xₙ} to orthonormal basis {u₁,...,uₙ}, worked computational examples, geometric visualizations, QR factorization A = QR as byproduct with applications to solving least squares
- [x] `Lecture22-REDO!/` - Least squares problems (Lay §6.5): overdetermined systems Ax = b (m > n), normal equations AᵀAx̂ = Aᵀb giving best approximation, connection to orthogonal projection onto Col(A), marked "REDO!" indicating this lecture required revision (likely to fix errors in original version)
- [x] `Lecture23Applications/` - Capstone lecture showcasing advanced applications: Fourier analysis (representing functions as infinite series of sines/cosines using orthogonality), algebraic topology and homology groups (counting holes in spaces), Google PageRank algorithm (eigenvector of web graph transition matrix), personality test dimensionality reduction, includes topology diagrams illustrating homological concepts
- [x] `LectureRevision/` - Exam preparation materials built around 2013 Mid-Semester Exam: worked solutions with step-by-step problem-solving techniques for lines/planes in R³, bases and coordinate systems, vector spaces and subspaces, matrix subspaces (null/column spaces), includes LaTeX source, Beamer presentations (screen and print versions), multiple exam PDF variants (la1301/a/b, la1302/a), Maple worksheets demonstrating Markov chain iteration, Italian exam paper (prova.pdf) possibly for comparison
- [x] `Revision/` - Comprehensive end-of-course revision: 13 practice problems spanning entire syllabus (change of basis, eigenvalue computation, diagonalization, dynamical systems, complex eigenvalues, orthogonal projections, orthogonal matrices, Markov chains, linear transformations on matrix/polynomial spaces), parallel question sheet (RevisionQ) and detailed solution manual (RevisionSols) with complete worked solutions, plus single worked example on complex eigenvalue factorization
- [x] `maple_cs Folder/` - Rich collection of 28 Maple computational case studies (.mws format) using custom `laylinalg` package: network flow and traffic analysis (Section 1.10), Hill cipher cryptography with modular arithmetic (Section 4.1), Leontief input-output economic models (Section 2.6), Fibonacci sequences via eigenvalues (Section 5.3), error-correcting codes, polynomial interpolation, cubic splines, numerical methods (LU/QR factorizations, condition numbers, QR eigenvalue algorithm), Jacobian matrices, optimization, graph theory (adjacency matrices), electrical circuit analysis (currents.mws, 4.4MB largest file), ranges from focused 12KB examples to extensive 1.5MB demonstrations

## Search Tags

math1014 joan-licata jel lecture-materials linear-algebra beamer-slides latex-source semester1-2013 semester1-2015 anu vectors eigenvalues vector-spaces orthogonality case-studies maple-worksheets lay-textbook webassign archived-lectures
