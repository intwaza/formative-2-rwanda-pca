# Formative 2 PCA on Rwanda's Seasonal Agricultural Survey (2024 Season B)

PCA implemented from scratch (numpy + matplotlib only) on plot-level agricultural practice data
from the National Institute of Statistics of Rwanda (NISR).

| Path | Contents |
|---|---|
| `data/raw/` | Original dataset exactly as downloaded (with missing values), plus NISR metadata and README |
| `data/processed/sas_2024B_pca_ready.csv` | Cleaned, encoded, no missing values (unscaled) – 17,260 rows × 20 features |
| `01_data_preparation_and_pca.ipynb` | Data preparation + Task 1 (PCA from scratch) + before/after plots |
| `02_component_selection_and_benchmarking.ipynb` | Task 2 (choosing the number of components from explained variance, information lost) + Task 3 (faster, chunked PCA, benchmark, 50M-row streaming test) |
| `figures/` | Plots exported from the notebooks |
| `BSE Group Assignments _ Task Sheet_[Advanced Linear Algebra_Principle Component Analysis_Cohort 2_Team 17] - 1.pdf` | Team task sheet: who did each task, and the meeting log |

`01_data_preparation_and_pca.ipynb` writes `data/processed/sas_2024B_pca_ready.csv`, which
`02_component_selection_and_benchmarking.ipynb` reads (the file is already in the repo, so either notebook can be run on its own).
Both notebooks use paths relative to the repo root.
