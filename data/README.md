## Data setup

The datasets used in this project are **not stored in the repository**.

To run the notebook locally, place the required files in this `data/` directory following the structure expected by the notebook.

The notebook automatically detects whether data files are located in the working directory (e.g. a university JupyterHub environment) or in a `data/` subdirectory (GitHub repository layout).

---

## Required files

The project expects the following files to be available locally:

- **`wiki-articles.json`**  
  Line-delimited JSON file containing Wikipedia articles. Each line includes an article ID, URL, title, and body text (text content only).

- **`tweets.json`**  
  Line-delimited JSON file containing tweets. Each entry includes a tweet ID, timestamp, and tweet text.

- **`linuxwords`**  
  Plain-text English word list used for dictionary-based matching tasks.

---

## Notes

- These files are not included in the repository due to **size and licensing considerations**.
- The notebook contains saved outputs and is intended to be readable without re-running the analysis.
