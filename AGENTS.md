# AGENTS.md

## Project goal

This repository supports a **research-proposal writing project whose objective is to discover one research gap in Text-to-SQL**. The selected literature, citation graph, bibliography, and manuscript materials are organized so the gap can be identified, justified with references, and developed into a proposal.

## Directory layout

```text
txt2sql/
├── map.csv                # Paper index: front, BibTeX ID, PDF location
├── papers/                # Downloaded paper PDFs (git-ignored)
├── src/
│   ├── main.tex           # Text-to-SQL reference graph and grouped bibliography table
│   ├── ref.bib            # BibTeX source of truth for all references
│   ├── proposal.md        # Research-proposal slide deck (Marp markdown)
│   ├── proposal.tex       # Research-proposal LaTeX file
│   └── *.{aux,log,out,pdf}  # LaTeX build artifacts (git-ignored)
├── scripts/
│   ├── build_tex.sh       # Compile a .tex file with XeLaTeX in Docker
│   ├── download_arxiv.py  # Download arXiv PDFs listed in a BibTeX file
│   └── lint_bib_lib.py    # Lint src/ref.bib against reference rules
└── venv/                  # Local Python environment (has bibtexparser, PyPDF2, matplotlib, etc.)
```

`_extract/` is a temporary working directory and is git-ignored.

## `map.csv`: fast index for locating papers

`map.csv` is the paper index used to avoid re-reading `src/main.tex` and
`src/ref.bib` during later tasks. Each row represents exactly one selected paper.

| Column | Meaning |
| --- | --- |
| `research front` | One of the seven research-front labels used in `src/main.tex`. |
| `bibtex entry ID` | Entry key in `src/ref.bib` (for example `ren_purple_2024`). |
| `paper location` | Path to the paper PDF under `papers/`. |

The current index contains the 33 papers selected in `src/main.tex`. Keep it in
sync when papers are added or removed.

## Naming conventions

### Paper PDFs

Store every paper under `papers/` using:

```text
<lastname-of-first-author><YY><first-word-of-title>.pdf
```

- Lowercase the whole filename.
- Keep only alphanumeric characters; strip spaces and punctuation.
- `YY` is the two-digit publication year.
- Examples: `yu18spider.pdf`, `ren24purple.pdf`, `cao26apex.pdf`.
- `scripts/download_arxiv.py` generates this name automatically; reuse the
  existing filename when adding a row to `map.csv`.

### Research fronts

Use the exact labels from `src/main.tex`:

- `Benchmarks & evaluation`
- `Schema linking & neural parsing`
- `LLM prompting / decomposition`
- `Agentic LLM (multi-agent)`
- `Generate-then-rank & self-correction`
- `SLM-LLM collaboration & open-source`
- `Industrial NLIDB systems`

### Bibliography

- Add all references to `src/ref.bib`; do not cite papers that are absent there.
- Every entry should have `title`, `author`, `year`, and `url`.
- `scripts/lint_bib_lib.py` requires at least 50% of entries to be published
  since 2024.
- Preserve existing BibTeX keys; `map.csv` refers to them directly.

## Notes for agents

- Treat `src/ref.bib` as the bibliography source of truth.
- Do not commit PDFs, build artifacts, `venv/`, or `_extract/`.
- When editing `src/main.tex`, keep the 33-paper graph, research-front labels,
  and `map.csv` consistent with each other.
