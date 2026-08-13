# LANG1409 Quiz Workflow (Synthetic Portfolio Version)

This project demonstrates a script-traceable workflow for preparing quiz data from library training workshops using fully synthetic data. It is designed for portfolio use and does not include confidential records.

Synthetic data modeled on a real analysis workflow - real data is confidential.

## What This Contains

- A strict notebook version of the workflow in [LANG1409_script_only_synthetic.ipynb](LANG1409_script_only_synthetic.ipynb)
- Deterministic synthetic data generation (seeded)
- Script-style CSV cleaning behavior:
  - detect/remove section marker row
  - remove first 3 columns
- Basic validation checks after cleaning

## Sanitization

All internal references are replaced with placeholders:

- [LMS_BASE_URL]
- [LOCAL_DATA_FOLDER]
- [REAL_FILENAME]
- [COURSE_IDENTIFIER]

No real student identities, internal URLs, or private file paths are included.

## Files

- [LANG1409_script_only_synthetic.ipynb](LANG1409_script_only_synthetic.ipynb): main portfolio notebook
- [LANG1409_portfolio_synthetic.ipynb](LANG1409_portfolio_synthetic.ipynb): earlier presentation-style notebook variant
- [LANG Sample.py](LANG%20Sample.py): source script provided for workflow grounding

## How To Run

1. Open [LANG1409_script_only_synthetic.ipynb](LANG1409_script_only_synthetic.ipynb) in VS Code or Jupyter.
2. Run cells from top to bottom.
3. The notebook will generate synthetic CSV outputs in the same folder.

## Suggested GitHub Upload Scope

Recommended to commit:

- [README.md](README.md)
- [LANG1409_script_only_synthetic.ipynb](LANG1409_script_only_synthetic.ipynb)

Recommended to exclude:

- Real CSV/XLSX exports from private folders
- Any non-synthetic local data artifacts

## Notes

This notebook intentionally avoids adding analysis steps that are not directly supported by the provided source script. Its goal is methodological transparency and confidentiality-safe reproducibility.
