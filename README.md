# Beamer Presentation Template

A clean, minimal LaTeX Beamer template for academic seminar and conference presentations, styled in a navy-blue serif theme.

## Features

- 16:9 aspect ratio with Palatino-style typography (`mathpazo`)
- Custom navy/light-blue color scheme applied to frame titles, structure elements, and buttons
- Minimal footline showing only the frame counter; navigation symbols removed
- Appendix slides excluded from the frame count via `appendixnumberbeamer`
- Pre-built skeleton frames: title page, Motivation, Research Question, Literature & Contribution, Conclusion, and References
- Custom commands:
  - `\gapbox{...}` — highlighted `tcolorbox` for research questions or key takeaways
  - `\SolidImplies` — bold TikZ implication arrow for inline use in math mode
  - `\src{...}` — small gray source note for figures and tables
  - `\tight` — compact itemize spacing
- Numbered figure captions and custom itemize markers

## Requirements

- A LaTeX distribution (e.g., TeX Live or MiKTeX)
- BibTeX for the bibliography (`natbib` with the `apalike` style)
- Packages: `beamer`, `mathpazo`, `booktabs`, `graphicx`, `amsmath`, `amssymb`, `mathtools`, `natbib`, `tcolorbox`, `tabularx`, `array`, `multirow`, `appendixnumberbeamer`, `tikz`, `soul`, `xcolor`

## Compilation

```bash
pdflatex slides_template.tex
bibtex   slides_template
pdflatex slides_template.tex
pdflatex slides_template.tex
```

## Project Structure

```
.
├── slides_template.tex   # Main Beamer source
├── ref.bib               # Bibliography database (expected by \bibliography{ref})
└── figures/              # Figures directory (set via \graphicspath)
```

## Usage

Replace the placeholder title, author, and frame content with your own material, add references to `ref.bib`, and place figures in `figures/`.
