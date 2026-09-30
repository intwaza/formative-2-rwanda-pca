# Formative 2 PCA on Rwanda's Seasonal Agricultural Survey (2024 Season B)

PCA implemented from scratch (numpy + matplotlib only) on plot-level agricultural practice data
from the National Institute of Statistics of Rwanda (NISR).

| Path | Contents |
|---|---|
| `data/raw/` | Original dataset exactly as downloaded (with missing values), plus NISR metadata and README |
| `data/processed/sas_2024B_pca_ready.csv` | Cleaned, encoded, no missing values (unscaled) – 17,260 rows × 20 features |
| `PCA_Formative2_Person1.ipynb` | Data preparation + Task 1 (PCA from scratch) + before/after plots |
| `PCA_Formative2_Person2.ipynb` | Task 2 (choosing the number of components from explained variance, information lost) + Task 3 (faster, chunked PCA, benchmark, 50M-row streaming test) |
| `figures/` | Plots exported from the notebooks |
| `contribution_sheet.pdf` | Team task sheet: who did each task, and the meeting log |

`PCA_Formative2_Person1.ipynb` writes `data/processed/sas_2024B_pca_ready.csv`, which
`PCA_Formative2_Person2.ipynb` reads (the file is already in the repo, so either notebook can be run on its own).
Both notebooks use paths relative to the repo root.
