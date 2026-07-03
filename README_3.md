# ❤️ Heart Disease Prediction — Orange Data Mining Project

This repository documents a complete, no-code machine learning workflow built in
[Orange Data Mining](https://orangedatamining.com/) to explore and predict heart
disease from clinical patient data (1,025 records, 13 features).

![Orange](https://img.shields.io/badge/tool-Orange%20Data%20Mining-orange)
![Best AUC](https://img.shields.io/badge/best%20AUC-0.986%20(Tree)-brightgreen)
![Status](https://img.shields.io/badge/status-complete-success)

---

## 📄 What's in this repo

| File | What it is |
|------|-----------|
| **`Heart_Disease_Orange_Report.pdf`** | The full **process report** — a 10-page write-up covering the project overview, what Orange is, the dataset, the complete workflow architecture with every widget connection explained, step-by-step methodology, EDA findings, model results, and key takeaways. Read this to understand the *why* behind every step. |
| **`Screenshot_Gallery.pdf`** | A **visual-only gallery** — one screenshot per page, in workflow order, from the raw canvas overview through to the final Tree Viewer. No analysis, just a clean walkthrough of what each widget looked like when run. Useful as a quick visual reference or for presentations. |
| `data/heart.csv` | The source dataset |
| `workflow/heart_disease.ows` | The actual Orange workflow file — open this in Orange to reproduce everything |
| `screenshots/` | The 12 individual PNG screenshots used in both PDFs |

## 📊 Quick Summary

Four classifiers were trained and cross-validated on the dataset:

| Model | AUC | Accuracy |
|-------|-----|----------|
| 🥇 **Tree** | **0.986** | **95.7%** |
| Logistic Regression | 0.937 | 86.6% |
| Naive Bayes | 0.919 | 84.6% |
| kNN | 0.864 | 72.6% |

The decision tree came out on top, with **`cp` (chest pain type), `thal`, and `ca`**
emerging as the strongest predictors of heart disease — consistent with their known
clinical significance.

Full details, methodology, and every chart are in `Heart_Disease_Orange_Report.pdf`.

## 🧰 Tools Used

Orange Data Mining 3.x — widgets: CSV File Import, Data Table, Edit Domain, Column
Statistics, Distributions, Box Plot, Scatter Plot, Correlations, Select Columns,
Tree, Naive Bayes, Logistic Regression, kNN, Test and Score, Confusion Matrix, ROC
Analysis, Tree Viewer.

## ▶️ How to Reproduce

1. Install [Orange Data Mining](https://orangedatamining.com/download/) (free).
2. Clone this repo:
   ```bash
   git clone https://github.com/<your-username>/heart-disease-orange.git
   ```
3. Open Orange → **File → Open** → select `workflow/heart_disease.ows`.
4. Run the canvas — all widgets re-execute on `data/heart.csv`.

## 📜 License

MIT License — feel free to reuse and adapt.

---

*Built as a hands-on exercise in visual, no-code machine learning with Orange Data Mining.*
