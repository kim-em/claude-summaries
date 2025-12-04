---
source_path: /Users/kim/Documents/Jobs/ANU/2014/Analysis3
generated: 2025-12-04T00:00:00Z
git_sha: 48a99ef1be36fc0c3cca2af4518f1aebb71ec697
git_branch: master
status: preliminary
files_count: 9
subdirs_count: 6
---

# Analysis3

## Overview

MATH3325 Analysis 3 Honours course materials from Semester 2, 2014 at ANU. An honours-level mathematics course covering Hilbert spaces, operators on Hilbert space, abstract measure theory, spectral theory for bounded self-adjoint operators, and Banach spaces. Based on Stein & Shakarchi's Real Analysis (Vol. III) chapters 4-6 and Functional Analysis (Vol. IV) chapter 1. The course had 14 enrollments and received strong student evaluations (4.3/5 overall satisfaction). Includes complete lecture notes, four problem sets with hints, four assignments with sample solutions, essay assignments, reference materials, a build script for publishing to the course website, and a TODO list of proof corrections needed.

## Key Files

| File | Purpose |
|------|---------|
| `Sem_2_2014-MATH3325_Analysis_3_Honours.pdf` | Official course outline from ANU showing topics (Hilbert spaces, operators, measure theory, spectral theory, Banach spaces), assessment structure (4 assignments 40%, final exam 60%), and textbook requirements (Stein & Shakarchi Vols. III-IV) |
| `Sem_2_2014-Scott_Morrison.pdf` | Course evaluation results showing 14 enrollments, 5 responses, 4.3/5 average satisfaction, with positive feedback on lecture notes accessibility, clear explanations of concepts, and good applications of theory; suggestions for more frequent assignments and clearer exam scope |
| `EXAMINATION INFORMATION GATHERING AID END OF SEM.doc` | Exam preparation aid (119KB Word document, too large to read in detail) |
| `TODO.txt` | Course development TODO list including needed proof corrections (countable additivity in Carathéodory extension theorem, Stone-Weierstrass theorem proof, continuity for Borel calculus, equivalence between Baire category formulations); includes Halmos quote about mathematics pedagogy |
| `make` | Build and deployment script: compiles all LaTeX lecture notes and problem sets using XeLaTeX, copies PDFs to ~/Sites/tqft.net/web/teaching/2014/Analysis3/, generates 4-up reduced versions of lecture notes for printing, commits to SVN repository |
| `preamble.tex` | Shared LaTeX preamble defining theorem environments (proposition, theorem, lemma, corollary, definition), custom math operators (norm, span, kernel, Fourier transform), note formatting system with color-coded instructor notes (green), and macros for Hilbert space notation (\HH, \ang, \norm) |
| `operators.tex` | Draft chapter outline on operators on Hilbert space covering linear functionals, Riesz representation theorem, adjoints, self-adjoint operators, projections, isometries, unitaries, compact operators, Calkin algebra, and spectral theory for self-adjoint compact operators; also includes abstract measure theory and Banach spaces sections |
| `references.tex` | LaTeX source for course bibliography listing required text (Stein & Shakarchi Real Analysis Vol. III) and recommended references including Tao's measure theory notes, Bressan, Conway, Halmos problem book, Kowalski's spectral theory notes |
| `references.pdf` | Compiled bibliography PDF (1 page) |
| `web` | Symbolic link to /Users/scott/Sites/tqft.net/web/teaching/2014/Analysis3/ for local website preview |

## Subdirectories

- [~] `Assignments/` - Four assignments with TeX source, compiled PDFs, sample solutions (Assignments 1, 2, 4), student submission folders, essay components (EssayTopics, EssayDrafts, EssayExamples, FinalEssays) (preliminary)
- [ ] `LectureNotes/` - 12+ lecture note files covering the course progression from Hilbert spaces through Banach spaces, including topics on compact operators, functional calculus, Fourier transform, fundamental solutions, Radon-Nikodym derivatives, Stone-Weierstrass theorem, and spectral theory (pending)
- [ ] `ProblemSets/` - Four problem sets with TeX source, compiled PDFs, and hints files for problem sets 1, 2, and 4; includes flags.tex for conditional compilation (pending)
- [ ] `books/` - Reference textbook collection (10 files) including Stein & Shakarchi volumes 1-4 (Fourier, Complex, Real, Functional analysis) with solutions manual for Vol. 3, and additional references by Bressan, Conway, Halmos, Helmberg, and Pedersen (pending)
- [ ] `evaluations/` - Course and instructor evaluation PDFs showing student feedback on MATH3325 and Scott Morrison's teaching (pending)
- [ ] `grades/` - Grade spreadsheets (2460-MATH-3325-7322.xlsx, 2460-MATH-6214-7325.xlsx) and Mathematica notebook for grade calculations (pending)

## Search Tags

math3325 analysis-3 honours anu 2014 semester-2 hilbert-spaces operators measure-theory spectral-theory banach-spaces functional-analysis stein-shakarchi scott-morrison real-analysis lecture-notes problem-sets assignments course-evaluation xelatex latex tqft-net teaching mathematics advanced-analysis radon-nikodym stone-weierstrass borel-calculus compact-operators self-adjoint fourier-transform
