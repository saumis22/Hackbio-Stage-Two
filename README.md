# Single-Cell RNA-Seq Analysis with Scanpy

## Overview
This project reproduces a core scRNA-seq workflow using Scanpy.  
We identify immune cell populations, evaluate whether the dataset truly represents bone marrow, and assess whether the immune system reflects a healthy or inflamed state.

---

## What This Notebook Does
- Performs QC, normalization, log transform
- Runs PCA → neighbors → UMAP
- Clusters cells (Leiden)
- Identifies marker genes and annotates cell types
- Quantifies cell-type proportions
- Compares observed composition vs expected biology
- Interprets tissue origin and immune health state

---

## Key Results
**Cell types identified:**  
T cells, cytotoxic T/NK-like cells, NK cells, classical + inflammatory monocytes,  
B cells, memory B cells, plasma cells, proliferating immune cells, platelets/megakaryocytes.

**Tissue conclusion:**  
The dataset does **not** resemble true bone marrow (no progenitors, granulocyte or erythroid lineages).  
Composition aligns with **peripheral blood / PBMC**.

**Health conclusion:**  
Elevated inflammatory monocytes, cytotoxic/NK expansion, plasma cells, and proliferating cells indicate an **activated / infected immune state**, not healthy baseline.

---

## Running the Notebook
Install dependencies:
pip install scanpy anndata pandas seaborn matplotlib
