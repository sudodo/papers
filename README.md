# papers

This repository collects the papers of its owner (GitHub: `sudodo`) in one place. For each paper it holds the released versions of:

- the PDF and the TeX source,
- the scripts that mechanically check the manuscript,
- the Lean formalization, when the paper has one,
- a README stating which claims of the paper passed mechanical checking in Lean and which did not (`lean/<paper>/README.md`).

A paper says nothing about Lean verification beyond what that README lists.

The repository is an empty skeleton for now. Papers are added when their preprints are released.

## Layout

| Path | Contents |
|---|---|
| `preprints/<Title-Month-Day-Year>/` | One released version: `README.md` (citation), the PDF, and `build/` (TeX source and manuscript checking scripts) |
| `lean/<paper>/` | A self-contained Lake package with the paper's Lean formalization, and `README.md` stating the scope of what was verified |
| `lean/formalization.yaml` | One catalogue of all formalizations in this repository |
| `CONTENTS.md` | Map of the papers |
| `history.md` | Log of updates to this repository |

The layout follows [`openai/math`](https://github.com/openai/math). The one difference is that `lean/` holds one self-contained Lake package per paper instead of a single library; the per-paper `README.md` plays the role of the scope notes in `openai/math`'s `lean/docs/`.

## Licenses

- `preprints/` (PDFs and TeX sources) is licensed under [Creative Commons Attribution 4.0 International](LICENSE-CC-BY-4.0) (CC BY 4.0).
- `lean/` and all scripts are licensed under the [Apache License 2.0](LICENSE-APACHE).
