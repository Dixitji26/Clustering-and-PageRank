# Assignment 4 — Clustering, Web Search, and PageRank

This repository contains a Python notebook implementation for three classic data mining / information retrieval tasks:

1. **Clustering**
2. **Web Search using an Inverted Index**
3. **PageRank**

The main implementation is in:

- `Assignment4_MLBD.ipynb`

---

## Project Overview

### Part 1 — Clustering
Implements clustering routines for the UCI Spam dataset:

- `readVectorsSeq(filename)`
- `kcenter(P, k)`
- `kmeansPP(P, k)`
- `kmeansObj(P, C)`

It also runs the required experiments using:
- `k = 10`
- `k1 = 20`

### Part 2 — Web Search
Implements a simple search engine based on an inverted index.  
It supports:

- adding webpages from a folder
- finding pages that contain a given word
- finding positions of a word inside a webpage
- verifying the output against `answers.txt`

### Part 3 — PageRank
Implements PageRank for graph datasets.

- uses Spark if available
- falls back to a pure Python implementation if Spark is not installed
- reports the top-5 and bottom-5 ranked nodes

---
Requirements
Python 3.9+
NumPy
PySpark (optional, only for Spark-based PageRank)

Suggested installation:
pip install numpy pyspark
If PySpark is not installed, the notebook automatically uses the pure Python PageRank implementation.
