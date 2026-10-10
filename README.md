# visual-formats

Creative strategy visual-format library.

- **`formats/`** One folder per format, each holding a `classify.md` (how to identify the format) and an `execute.md` (how to build one). The definitions are shared by every season.
- **`files/`** Every example ad in one folder, year-round (`s=evergreen`) and Black Friday / Cyber Monday (`s=bfcm`), all named the same way. Naming rules, offer types, favorites and tag notes are in its `_index.md`.

- **`index.html`** One browsable page of every example ad (evergreen + Black Friday) with filters and playable videos. All media loads from this repo. Rebuilt by the brain tool at tools/visual-formats-page/build.py.

Start with [index.md](formats/index.md).
