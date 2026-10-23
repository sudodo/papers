# lean

One self-contained Lake package per paper: `lean/<paper>/` (with its `lakefile`, `lean-toolchain`, `lake-manifest.json`, specification modules and proof modules).

`lean/<paper>/README.md` states the scope of the formalization: which claims of the paper passed mechanical checking in Lean (with declaration names), which did not, the Lean and Mathlib versions, and the axioms used. The paper refers to Lean verification only through a footnote pointing to this README.

- The published Lean source is the revision that was mechanically checked.
- A paper that builds on another paper's formalization depends on that paper's package at a fixed released version through `require`; it does not keep a copy.
- `formalization.yaml` is the single catalogue of all formalizations in this repository.

Licensed under the Apache License 2.0. See the repository README.
