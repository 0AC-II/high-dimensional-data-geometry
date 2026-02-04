# Understanding High-Dimensional Biological Data

### A Guided Comparison of PCA and t-SNE

High-dimensional data is everywhere in modern science; from gene expression to proteomics to single-cell data and yet human intuition breaks down quickly beyond a few dimensions.

This project explores **how high-dimensional data behaves** and how common dimensionality reduction techniques can **shape (and sometimes distort)** our understanding of structure.

Rather than treating PCA or t-SNE as mere visualization tools, this notebook approaches them as **models with assumptions**, using a controlled synthetic dataset inspired by biological data.

---

## Project Motivation

When thousands of features are compressed into two dimensions, something is always lost.

The key questions guiding this project were:

* Why does distance intuition fail in high dimensions?
* What does PCA preserve — and what does it ignore?
* Why does t-SNE often produce convincing clusters?
* How do we avoid over-interpreting visually appealing plots?

The goal is not model performance, but **interpretation, reasoning, and intellectual discipline**.

---

## Dataset

* **Type:** Synthetic gene-expression-like data
* **Samples:** 600
* **Features:** 1,200 (genes)
* **Classes:** 3 biological conditions
* **Properties:**

  * Sparse informative features
  * Correlated genes (redundancy)
  * Noise and class overlap

Synthetic data is used intentionally so the *ground truth is known*, making distortions easier to reason about.

---

## Methods Covered

* High-dimensional distance analysis
* Distance concentration effects
* Principal Component Analysis (PCA)
* Explained variance and reconstruction error
* t-SNE for local neighborhood preservation
* Sensitivity to hyperparameters and random seeds

---

## Key Insights

* In high dimensions, “nearest neighbors” lose meaning
* PCA preserves variance, not class separation or biological relevance
* t-SNE excels at local structure but can create misleading global patterns
* Dimensionality reduction methods **do not reveal objective truth** — they impose perspective

---

## What This Project Is (and Is Not)

**This project is:**

* A conceptual and exploratory analysis
* Focused on understanding model assumptions
* Designed for clarity and interpretability

**This project is not:**

* A benchmarking exercise
* A clustering validation study
* A claim of biological discovery

---

## Notebook

* `notebooks/Understanding_High_Dimensional_Biological_Data.ipynb`

The notebook is fully commented and highly guided, with step-by-step explanations intended for learning and clarity.

---

## Why This Matters

Misinterpreting dimensionality reduction plots can lead to false confidence and incorrect conclusions — especially in scientific and biomedical contexts.

This project is a reminder that **beautiful plots require careful thinking**.
