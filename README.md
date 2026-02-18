# VigiMed Pharmacovigilance Pipeline

This repository provides a reproducible data processing pipeline used to
construct and analyze pharmacovigilance data from the Brazilian VigiMed
system.

The workflow allows researchers to reconstruct the analytical database and
calculate disproportionality metrics for drug–adverse event signal detection.

---

## 📊 Data Source

The standardized dataset used in this project is publicly available in the
Harvard Dataverse repository.

Users must download the Parquet files before running the notebooks.

Dataset DOI: *(insert DOI here)*

---

## 🔄 Workflow Overview

The pipeline is divided into two notebooks.

### 1️⃣ Database Construction

Notebook:01_construcao_banco.ipynb



This notebook: [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/carolinajacoby/vigimed/blob/main/01_construcao_banco.ipynb)


- loads standardized datasets
- builds the analytical database
- exports the file `fat_analitica.parquet`

---

### 2️⃣ Disproportionality Analysis

Notebook: 02_analises_desproporcionalidade.ipynb


This notebook: [![Open Notebook 02 in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/carolinajacoby/vigimed/blob/main/02_analises_desproporcionalidade.ipynb)


- builds contingency tables
- calculates disproportionality metrics
- exports final analytical results

Metrics calculated:

- Reporting Odds Ratio (ROR)
- Proportional Reporting Ratio (PRR)
- Chi-square test
- Information Component (BCPNN)
- Empirical Bayes Geometric Mean (EBGM)

---

## ▶️ How to Run

Recommended environment: Google Colab.

Steps:

1. Download data tables from Dataverse.
2. Open notebooks in Google Colab.
3. Upload required files when requested.
4. Execute all notebook cells.

Results will be generated automatically.

---

## 📚 Citation

If you use this pipeline or dataset, please cite:

Jacoby AC et al. Adverse drug reaction records from the Brazilian pharmacovigilance system (VigiMed), 2018–2025. 2026.

---

## 📧 Contact

Ana Carolina Jacoby  
Email: anacarolinajacoby0@gmail.com


