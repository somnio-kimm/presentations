# Presentations

LaTeX [Beamer](https://ctan.org/pkg/beamer) presentations by **Soo Min Kimm** (16:9).
Each talk lives in its own folder with `main.tex`, a shared `format.tex` (theme,
title macros, helpers), a `figure/` directory, and the compiled `main.pdf`.

## Talks

| Talk | Topic | Slides |
|------|-------|--------|
| [State-Space Models](State-Space%20Models/main.pdf) | State-space models / SSMs | [PDF](State-Space%20Models/main.pdf) · [source](State-Space%20Models/main.tex) |
| [Generative Models](Generative%20Models/main.pdf) | Survey of generative modeling families | [PDF](Generative%20Models/main.pdf) · [source](Generative%20Models/main.tex) |
| [Computer Vision](CV/main.pdf) | Object recognition | [PDF](CV/main.pdf) · [source](CV/main.tex) |
| [World Models](World%20Models/main.pdf) | Ha & Schmidhuber (2018): architecture, experiments, and recent-model comparison | [PDF](World%20Models/main.pdf) · [speaker notes](World%20Models/main-notes.pdf) · [source](World%20Models/main.tex) |

[`Template/`](Template/) is a blank starting point for new talks.

## Building

Each folder is self-contained. To compile a talk:

```bash
cd "Generative Models"
latexmk -pdf main.tex     # or: pdflatex main.tex (run twice for the ToC/refs)
```

Compiled `main.pdf` files are committed so the slides are viewable without a
LaTeX toolchain. Auxiliary build files (`.aux`, `.log`, `.nav`, …) are
git-ignored — see [.gitignore](.gitignore).
