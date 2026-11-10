# SDN Proposal – Express Overleaf version

This is the same Master's research proposal with its six vector diagrams and 24 references.

## Why this edition compiles faster
- Biber/biblatex was replaced by standard LaTeX `\bibitem` references in `references.tex`.
- No external bibliography program is required; `references.bib` remains as an archival editable BibTeX source.
- The six diagrams are already pre-rendered to PDF and included from `figures/`.
- A nonessential microtype warning source was removed.
- The lighter Latin Modern font package retains 12pt academic typography while reducing compiler overhead.

## Upload and compile
1. In Overleaf choose New Project -> Upload Project and choose this ZIP.
2. Ensure `main.tex` is the main document and Compiler = **pdfLaTeX**.
3. Click Recompile; if needed use Recompile from scratch.
4. If the free-plan timeout persists, choose Fast [draft] to diagnose image overhead, or use the included compiled PDF (if delivered separately).

## Editing
- Main research text: `main.tex`.
- Editable numbered bibliography: `references.tex` (must be edited to change citations in the PDF).
- Original structured reference data: `references.bib` (backup, **not actively processed** in this fast edition).
- Original diagram TikZ code is available in the earlier Fast project; this edition uses the PDF figures for quick compilation.
- Existing `\cite{...}` commands continue to function; bibliography keys are preserved.

Note: Because the bibliography is embedded as `\bibitem`s, this version does **not** use Biber. It is a performance workaround for Overleaf compile timeout, not a change to scientific content.
