# visual-formats

Creative strategy visual-format library.

- **`formats/`** One folder per format, each holding a `classify.md` (how to identify the format) and an `execute.md` (how to build one). The definitions are shared by every season.
- **`files/evergreen/`** Year-round example ads, tagged `s=evergreen`. See its `_index.md`.
- **`files/bfcm/`** Black Friday / Cyber Monday example ads, tagged `s=bfcm`, with offer tags in the file names and tag notes in its `_index.md`. See its `_index.md`.

- **`index.html`** One browsable page of every example ad (evergreen + Black Friday) with filters and playable videos. All media loads from this repo. Rebuilt by the brain tool at tools/visual-formats-page/build.py.

Start with [index.md](formats/index.md).
