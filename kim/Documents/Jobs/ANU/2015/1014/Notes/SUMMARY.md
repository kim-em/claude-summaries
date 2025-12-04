---
source_path: /Users/kim/Documents/Jobs/ANU/2015/1014/Notes
generated: 2025-12-04T06:00:00Z
git_sha: 48a99ef1be36fc0c3cca2af4518f1aebb71ec697
git_branch: master
status: preliminary
files_count: 7
subdirs_count: 25
---

# Notes

## Overview

Lecture notes for MATH1014 (Mathematics and Applications 2) semester 2 2015, containing 25 individual lecture directories with LaTeX source files for linear algebra topics. The folder includes a sophisticated build system using make and latexmk that automatically generates both presentation slides and 3-up handouts from each lecture's source. Key infrastructure files provide shared LaTeX formatting (beamer preamble, custom lecture document class, mathematical notation shortcuts) and build automation (makefile with targets for compilation and web posting).

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
- [ ] `Lecture12/` - Twelfth lecture material (pending)
- [ ] `Lecture13/` - Thirteenth lecture material (pending)
- [ ] `Lecture14/` - Fourteenth lecture material (pending)
- [ ] `Lecture15/` - Fifteenth lecture material (pending)
- [ ] `Lecture16/` - Sixteenth lecture material (pending)
- [ ] `Lecture17/` - Seventeenth lecture material (pending)
- [ ] `Lecture18/` - Eighteenth lecture material (pending)
- [ ] `Lecture19/` - Nineteenth lecture material (pending)
- [ ] `Lecture20/` - Twentieth lecture material (pending)
- [ ] `Lecture21/` - Twenty-first lecture material (pending)
- [ ] `Lecture22/` - Twenty-second lecture material (pending)
- [ ] `Lecture23/` - Twenty-third lecture material (pending)
- [ ] `Lecture24/` - Twenty-fourth lecture with supplementary materials (SVD compression Mathematica notebook, Markov chain Python scripts, Harry Potter text, GIF/PNG images) (pending)
- [ ] `Lecture25/` - Final lecture material (pending)

## Search Tags

math1014 linear-algebra lecture-notes anu 2015 semester-2 beamer latex slides handouts pdf-generation build-system makefile latexmk scott-morrison mathematics first-year teaching
