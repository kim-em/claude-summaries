---
source_path: /Users/kim/Documents/Jobs/ANU/2016/MATH1014/Worksheets
generated: 2026-01-25T09:45:00Z
git_sha: fafb26e72fe7b535873cd5b8a8f359b75df7fe29
git_branch: master
status: preliminary
files_count: 28
subdirs_count: 1
---

# Worksheets

## Overview

Weekly linear algebra tutorial worksheets for MATH1014 (Semester 2, 2016) covering weeks 3-14, plus a general matrix workshop. Each week's worksheet includes LaTeX source files and compiled PDFs with problem sets designed for in-class tutorial work. The worksheets cover foundational topics in linear algebra including geometric distance calculations, linear transformations, eigenvectors and eigenvalues, diagonalization, and matrix projections. The header.tex file provides a common formatting template with toggleable solution/hint display using `\solutions` and `\nosolutions` commands, allowing the same source to generate both student and instructor versions.

## Key Files

| File | Purpose |
|------|---------|
| MATH1014-LinearAlgebra-Week03-worksheet.tex/.pdf | Week 3 worksheet on distance from a point to a line using vector methods and cross products |
| MATH1014-LinearAlgebra-Week04-worksheet.tex/.pdf | Week 4 worksheet on linear algebra topics |
| MATH1014-LinearAlgebra-Week05-worksheet.tex/.pdf | Week 5 worksheet on linear algebra topics |
| MATH1014-LinearAlgebra-Week06-worksheet.tex/.pdf | Week 6 worksheet on linear algebra topics |
| MATH1014-LinearAlgebra-Week08-worksheet.tex/.pdf | Week 8 worksheet (note: no Week 7, likely mid-semester break) |
| MATH1014-LinearAlgebra-Week09-worksheet.tex/.pdf | Week 9 worksheet on linear algebra topics |
| MATH1014-LinearAlgebra-Week10-worksheet.tex/.pdf | Week 10 worksheet on linear transformations, diagonalizability, eigenvectors, and geometric interpretation of projections |
| MATH1014-LinearAlgebra-Week10-worksheet-solutions.pdf | Solutions for Week 10 worksheet with detailed explanations |
| MATH1014-LinearAlgebra-Week11-worksheet.tex/.pdf | Week 11 worksheet on linear algebra topics |
| MATH1014-LinearAlgebra-Week12-worksheet.tex/.pdf | Week 12 worksheet on linear algebra topics |
| MATH1014-LinearAlgebra-Week13-worksheet.tex/.pdf | Week 13 worksheet on linear algebra topics |
| MATH1014-LinearAlgebra-Week14-worksheet.tex/.pdf | Week 14 worksheet (largest file at 132KB PDF, likely review or comprehensive problems) |
| MATH1014-LinearAlgebra-matrix-worksheet.tex/.pdf | General matrix workshop covering eigenvalues, eigenvectors, diagonalization, and exploring when matrices are/aren't diagonalizable |
| header.tex | Common LaTeX header with formatting, solution/hint environments that can be toggled with `\solutions` or `\nosolutions` commands |
| makefile | Build script to compile all .tex files to PDFs using latexmk, with rsync target to upload to teaching server |
| makefile.user | User-specific makefile customizations |

## Subdirectories

- [x] `diagrams/` - Contains pointline.pdf diagram used in Week 3 worksheet for illustrating point-to-line distance problems

## Search Tags

anu math1014 2016 semester2 linear-algebra worksheets tutorial weekly latex eigenvectors eigenvalues diagonalization matrix transformations distance vector-geometry teaching-materials
