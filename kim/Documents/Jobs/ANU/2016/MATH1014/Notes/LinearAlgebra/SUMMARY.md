---
source_path: /Users/kim/Documents/Jobs/ANU/2016/MATH1014/Notes/LinearAlgebra
generated: 2026-01-25T09:40:00Z
git_sha: fafb26e72fe7b535873cd5b8a8f359b75df7fe29
git_branch: master
status: preliminary
files_count: 9
subdirs_count: 25
---

# LinearAlgebra

## Overview

LaTeX-based lecture notes for the linear algebra component of MATH1014 (Mathematics and Applications 2), taught by A/Prof Scott Morrison at ANU in Semester 2 2016. The course material is organized into 25 lectures, each with source files and generated PDFs in both slides and 3-up handout formats. Includes a sophisticated build system using makefiles and latexmk to generate multiple output formats from shared source files.

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
- [ ] `Lecture12/` - Linear algebra lecture content
- [ ] `Lecture13/` - Linear algebra lecture content
- [ ] `Lecture14/` - Linear algebra lecture content
- [ ] `Lecture15/` - Linear algebra lecture content
- [ ] `Lecture16/` - Linear algebra lecture content
- [ ] `Lecture17/` - Linear algebra lecture content
- [ ] `Lecture18/` - Linear algebra lecture content
- [ ] `Lecture19/` - Linear algebra lecture content
- [ ] `Lecture20/` - Linear algebra lecture content
- [ ] `Lecture21/` - Linear algebra lecture content
- [ ] `Lecture22/` - Linear algebra lecture content
- [ ] `Lecture23/` - Linear algebra lecture content
- [ ] `Lecture24/` - Linear algebra lecture content
- [ ] `Lecture25/` - Linear algebra lecture content

## Search Tags

math1014 linear-algebra beamer latex teaching lecture-notes anu 2016 semester2 scott-morrison makefile slides handouts vector-spaces eigenvalues eigenvectors
