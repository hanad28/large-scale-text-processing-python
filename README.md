# Large-scale Text Processing in Core Python

This project demonstrates efficient processing and analysis of large text datasets using core Python only (no Pandas, NumPy, or NLP libraries). It focuses on algorithmic thinking, memory-aware file streaming, and data structure choices (sets, dictionaries, Counters).

## What this project covers
- Streaming and parsing large line-delimited JSON datasets
- Text normalisation and token handling
- Frequency analysis and case-variant tracking
- Similarity analysis (Jaccard similarity with pruning)
- Building an inverted index and supporting keyword and wildcard-style search

## Tech stack
- Python (core libraries only)

## Repository structure
- `src/` reusable modules (normalisation, indexing, analysis)
- `notebooks/` cleaned notebook version of the work
- `reports/` coursework report (context and explanations)
- `data/` instructions for obtaining datasets (not stored in the repo)

## Data
This project uses large datasets (tweets and wiki-style articles) which are not committed to GitHub.
See `data/README.md` for instructions on how to place data locally.

## How to run
1. Create a virtual environment
2. Install dependencies (if any):
   - `pip install -r requirements.txt`
3. Run the notebook in `notebooks/`

## Notes
This work was developed during MSc Data Science & Artificial Intelligence study and refactored for portfolio presentation.
