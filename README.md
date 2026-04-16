# Thesis skeleton

Skeleton of the Master's thesis. Preamble mirrors `../example/main.tex`:
`report` class, `biblatex` + `biber`, 12 pt, 1.5 line spacing.

## Layout

```
thesis/
├── main.tex                       # preamble + \input glue
├── ref.bib                        # bibliography (placeholder entry)
├── frontmatter/
│   ├── titlepage.tex
│   ├── abstract.tex
│   ├── declaration.tex
│   ├── acknowledgments.tex
│   └── abbreviations.tex
├── chapters/
│   ├── 01_introduction.tex
│   ├── 02_background.tex
│   ├── 03_methods.tex
│   ├── 04_results.tex
│   ├── 05_discussion.tex
│   ├── 06_conclusion.tex
│   ├── 07_future_work.tex
│   └── appendix.tex
└── fig/                           # place PDF figures here
```

All section/subsection headings are in place; bodies are `% TODO` placeholders
only — this commit establishes the outline, not the prose.

## Build

```bash
cd dissertarion/thesis
pdflatex main
biber    main
pdflatex main
pdflatex main
```
