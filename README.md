# Large-Scale Text Processing in Core Python

## Overview

This project demonstrates how **large text datasets can be processed efficiently using core Python only**, without relying on high-level data or NLP libraries such as Pandas, NumPy, or spaCy.

The emphasis is on **algorithmic reasoning, memory-aware design, and scalable processing patterns** that transfer directly to real-world data analytics, data science, and information retrieval problems.

The work is based on **large Wikipedia article data and Twitter text data** and is presented as a **portfolio-style technical project**, focusing on clarity, efficiency, and maintainability rather than producing a fully packaged pipeline.

---

## Why this project

Many text analytics projects rely heavily on high-level libraries that abstract away performance and design considerations. This project deliberately takes the opposite approach.

It focuses on:
- Streaming large datasets without loading them into memory
- Choosing appropriate core data structures for efficiency
- Designing algorithms that scale to large corpora
- Writing readable, modular code that could be handed over to another analyst or engineer

These are the same constraints faced in real production and analytics environments.

---

## Key techniques demonstrated

- Streaming processing of large, line-delimited JSON datasets
- Memory-efficient use of Python sets, dictionaries, Counters, and default dictionaries
- Text normalisation and token handling for noisy real-world data
- Frequency analysis and case-variant tracking
- Similarity matching using the **Jaccard index**, with pruning to reduce unnecessary computation
- Construction of a **positional inverted index**
- Support for wildcard-style phrase search across large text corpora

---

## What the analysis covers

The notebook walks through a series of progressively more complex tasks, including:

### Wikipedia corpus analysis
- Identifying the most frequently occurring words across articles while avoiding bias from repeated terms within the same document
- Finding the longest contiguous sequence of capitalised words in article text
- Identifying the largest anagram sets across the corpus using canonical signatures

### Twitter corpus analysis
- Extracting and aggregating user mentions efficiently
- Tracking words with the highest number of case variations
- Identifying long dictionary-word sequences that appear across multiple distinct tweets

### Cross-corpus similarity
- Matching tweets to Wikipedia articles using **Jaccard similarity**
- Applying simple but effective pruning strategies to reduce computational cost

### Search and retrieval
- Building a shared **positional inverted index** across both corpora
- Supporting wildcard-style phrase queries without scanning entire documents
- Using candidate filtering followed by positional verification for efficiency

---

## Project structure

```
.
├── README.md
├── data/
│   └── README.md
├── notebooks/
│   └── large_scale_text_processing_core_python.ipynb
└── reports/
    └── large_scale_text_processing_core_python_report.pdf
```

---

## Notebook

The main analysis is contained in a single Jupyter notebook:

**[Large-scale Text Processing in Core Python](notebooks/large_scale_text_processing_core_python.ipynb)**

- Step-by-step technical walkthrough
- Clear explanations of algorithmic choices
- Saved outputs included for readability
- Designed to be understood without re-running the analysis

---

## Technical report

A concise technical report accompanies the notebook:

**[Technical Report](reports/large_scale_text_processing_core_python_report.pdf)**

The report explains:
- Algorithmic logic and design decisions
- Choice of data structures and control flow
- Efficiency, scalability, and maintainability considerations

It is written as if the work were being handed over to another data scientist or engineer.

---



## Data

The datasets used in this project are **not included in the repository** due to size and licensing constraints.

Expected files:
- `wiki-articles.json`
- `tweets.json`
- `linuxwords`

Details about the required data files and directory structure are provided in `data/README.md`.

The notebook automatically detects whether data files are located:
- In the working directory (e.g. university JupyterHub), or
- In a local `data/` subdirectory (GitHub layout)

---

## Design principles

Across all tasks, the guiding principles were:

- **Streaming I/O** to minimise memory usage
- **Single-pass algorithms** where possible
- **Appropriate core data structures** for fast lookup and aggregation
- **Readable, modular code** that is easy to audit and extend
- Avoiding unnecessary passes over the data

The goal was not linguistic sophistication, but **robust, scalable text processing**.

---

## Notes

This repository is intended as a **readable portfolio artefact**, not a fully reproducible production pipeline.

The focus is on:
- Core Python fundamentals
- Algorithmic thinking
- Scalable design patterns

The existing structure is deliberately simple so that more advanced techniques (e.g. TF–IDF, cosine similarity, improved tokenisation, persistence to disk) could be layered on without major refactoring.

---

## Future extensions

Possible extensions include:
- More robust tokenisation for social media text
- Alternative similarity measures (e.g. TF–IDF with cosine similarity)
- Persisting the inverted index to disk for larger-than-memory datasets
- Parallelising parts of the pipeline where appropriate

These enhancements were intentionally left out to keep the core logic clear and focused.

---

## Skills demonstrated

- Python (core language and standard library)
- Data analysis on large datasets
- Algorithmic problem solving
- Information retrieval
- Text processing and corpus analysis
- Memory-aware and scalable system design

---

### Final note

If you are reviewing this project as part of a data, analytics, or data science application, the emphasis here is **how problems are approached and solved**, not just the final outputs.

