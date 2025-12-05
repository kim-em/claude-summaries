---
source_path: /Users/kim/Documents/Jobs/ANU/2015/1014/Worksheets
generated: 2025-12-05T08:40:00Z
git_sha: 48a99ef1be36fc0c3cca2af4518f1aebb71ec697
git_branch: master
status: complete
files_count: 27
subdirs_count: 1
---

# Worksheets

## Overview

Complete set of tutorial worksheets for MATH1014 linear algebra component (Semester 2 2015). Contains 11 weekly problem sets covering weeks 2-4, 6, 8-14, plus a supplementary matrix workshop on eigenvalues and diagonalization. Each worksheet consists of LaTeX source and compiled PDF, with support for toggling solutions/hints via the header.tex infrastructure. Topics progress from geometric vector problems (distances, cross products, illustrated by supporting diagrams) through matrix operations, linear systems, vector spaces, and eigenvalue theory to advanced applications including dynamical systems and diagonalization. The makefile provides automated PDF compilation and deployment to web directory for student access. Includes single supporting diagram for Week 02's point-to-line distance problem.

## Key Files

| File | Purpose |
|------|---------|
| `MATH1014-LinearAlgebra-Week02-worksheet.tex/pdf` | Distance workshop: finding distance from point to line using vectors, trigonometry, and cross products |
| `MATH1014-LinearAlgebra-Week03-worksheet.tex/pdf` | Worksheet for week 3 (content TBD from PDF) |
| `MATH1014-LinearAlgebra-Week04-worksheet.tex/pdf` | Worksheet for week 4 (content TBD from PDF) |
| `MATH1014-LinearAlgebra-Week06-worksheet.tex/pdf` | Worksheet for week 6 (content TBD from PDF) |
| `MATH1014-LinearAlgebra-Week08-worksheet.tex/pdf` | Worksheet for week 8 (content TBD from PDF) |
| `MATH1014-LinearAlgebra-Week09-worksheet.tex/pdf` | Worksheet for week 9 (content TBD from PDF) |
| `MATH1014-LinearAlgebra-Week10-worksheet.tex/pdf` | Worksheet for week 10 (content TBD from PDF) |
| `MATH1014-LinearAlgebra-Week11-worksheet.tex/pdf` | Worksheet for week 11 (content TBD from PDF) |
| `MATH1014-LinearAlgebra-Week12-worksheet.tex/pdf` | Worksheet for week 12 (content TBD from PDF) |
| `MATH1014-LinearAlgebra-Week13-worksheet.tex/pdf` | Worksheet for week 13 (content TBD from PDF) |
| `MATH1014-LinearAlgebra-Week14-worksheet.tex/pdf` | Worksheet for week 14 (largest file at 132KB PDF, 9.6KB TeX - likely cumulative or exam prep) |
| `MATH1014-LinearAlgebra-matrix-worksheet.tex/pdf` | Advanced workshop on eigenvalues, eigenvectors, and diagonalization with hints/solutions; covers warm-up problems, projection transformations, and non-diagonalizable matrices |
| `header.tex` | LaTeX header defining solution/hint environments with toggle commands (\solutions and \nosolutions) for showing/hiding answers; uses green formatting for instructor notes |
| `makefile` | Build script that compiles all MATH1014*.tex files to PDF using latexmk, with post-build target to deploy to ~/Sites/tqft.net/web/teaching/2015/1014/ and commit to SVN |

## Subdirectories

- [x] `diagrams/` - Supporting diagrams and figures for worksheets

## Search Tags

math1014 linear-algebra worksheets tutorial-problems anu 2015 semester-2 problem-sets eigenvalues eigenvectors diagonalization vector-geometry matrices latex teaching-materials weekly-worksheets
