# papers

This repository collects the papers of its owner (GitHub: `sudodo`) in one place. For each paper it holds the released versions of:

- the PDF and the TeX source,
- the scripts that mechanically check the manuscript,
- the Lean formalization, when the paper has one,
- a README stating which claims of the paper passed mechanical checking in Lean and which did not.

A paper says nothing about Lean verification beyond what its README lists.

The repository is an empty skeleton for now. Papers are added when their preprints are released.

## Layout

| Path | Contents |
|---|---|
| `preprints/<paper>/` | PDF, TeX source and manuscript checking scripts of each released version |
| `lean/<paper>/` | A self-contained Lake package with the paper's Lean formalization |
| `lean/formalization.yaml` | One catalogue of all formalizations in this repository |
| `CONTENTS.md` | Map of the papers |
| `history.md` | Log of updates to this repository |

The layout follows [`openai/math`](https://github.com/openai/math).

## Licenses

- `preprints/` (PDFs and TeX sources) is licensed under [Creative Commons Attribution 4.0 International](LICENSE-CC-BY-4.0) (CC BY 4.0).
- `lean/` and all scripts are licensed under the [Apache License 2.0](LICENSE-APACHE).
