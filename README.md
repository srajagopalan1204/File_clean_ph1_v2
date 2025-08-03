# Phase 1 – File Reorganization Recommendation Script

This repository contains **Phase 1** of the file reorganization tool. Phase 1 analyzes the source folder, applies the configured rules (e.g., date range, file types), and generates a **recommendation report** (mapping of files to new folders) without making any changes.

## Purpose
- Scan a large directory (e.g., `C:\Users\scottuser\Documents`)
- Generate a structured mapping of files to their new locations
- Provide a preview for verification before executing moves in Phase 2

## Files
- `phase1_recommendation.py` – Core script for parsing and mapping
- `config.json` – Configuration file (input/output file, date range, destination root)
- `requirements.txt` – Python dependencies
- `.gitignore` – Excludes unnecessary files (logs, caches)

## Usage
1. Upload or place your input file (e.g., `filelist_docs_details_5540_080325.txt`) into the repo.
2. Update `config.json` with correct file name and paths.
3. Run:
```bash
python phase1_recommendation.py
```

Output Excel mapping file will be saved as `Phase1_FileMapping.xlsx`.

---
