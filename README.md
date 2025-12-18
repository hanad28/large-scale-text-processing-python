# Large-scale Text Processing in Core Python

This project demonstrates efficient processing and analysis of large text datasets using **core Python only** (no Pandas, NumPy, or NLP libraries).  
The focus is on streaming I/O, memory-aware data structures, and algorithmic text analysis that scales to large corpora.

The work is based on large Wikipedia article data and Twitter text data and is presented as a portfolio-style technical project.

---

## Project contents

### Notebook
The main analysis is contained in a single Jupyter notebook:

**[Large-scale Text Processing in Core Python](notebooks/large_scale_text_processing_core_python.ipynb)**  
- A step-by-step technical walkthrough covering:
  
  - Streaming and parsing line-delimited JSON datasets
  - Text normalisation and token handling
  - Frequency analysis and case-variant tracking
  - Similarity matching using the Jaccard index (with pruning)
  - Building a positional inverted index and supporting wildcard-style search

The notebook includes saved outputs and is intended to be readable without re-running the analysis.

---

### Technical report
A concise technical report accompanies the notebook:

**[Technical report (PDF)](reports/large_scale_text_processing_core_python_report.pdf)**  
- A consice explanation of the approach taken for each task, focusing on:
  
  - algorithmic logic and design decisions
  - choice of data structures and control flow
  - efficiency, scalability, and maintainability considerations

---

## Data

The datasets used in this project are **not included in the repository** due to size and licensing considerations.

Details about the expected data files and directory structure can be found in [`data/README.md`](data/README.md).

The notebook automatically detects whether data files are located in the working directory (e.g. a university JupyterHub environment) or in a `data/` subdirectory (GitHub layout).

---

## Key techniques demonstrated

- Streaming processing of large text corpora
- Efficient use of Python sets, dictionaries, and Counters
- Case-sensitive and case-insensitive text analysis
- Similarity matching with pruning
- Positional inverted index construction
- Wildcard-style phrase search

---

## Notes

This repository is intended as a **readable portfolio artefact** rather than a fully reproducible pipeline.  
The emphasis is on code clarity, algorithmic reasoning, and scalable design.

