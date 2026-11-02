# Dataset Browser

A static, self-contained copy of the local dataset browser. It works on GitHub Pages without a Python server or API.

## Publish with GitHub Pages

1. Create a new GitHub repository for this site.
2. Copy the contents of this folder to the repository root.
3. In the repository, open **Settings → Pages**.
4. Select **Deploy from a branch**, choose the `main` branch and `/ (root)`, then save.

The dataset comparison table opens a dataset when its name is selected. **HaluEval** and **Legal Hallucinations** are omitted from the navigation and comparison table, matching the local viewer. Their sample JSON files are included in `data/datasets/` as part of the complete local copy. Because GitHub Pages serves these files publicly, anyone who knows their file paths can access them.

## Data and sources

The site includes the local JSONL samples converted to JSON, the browser metadata, and the dataset source links shown in the viewer. Dataset records are static assets under `data/datasets/`; all contents of a public repository and GitHub Pages site can be downloaded. Check each source dataset's redistribution terms before publishing.

To rebuild this folder from the thesis project, run `python scripts/build_public_dataset_viewer.py` from the project root.
