# team138

EV Gap Score Generation

This project generates state-level EV **Gap Scores**, which measure the difference between EV policy strength and charging infrastructure.

---

## Required Files

Ensure the following files are in the **same folder**:

- `gap_score.ipynb`
- `clean_data.csv`
- `state_recency.csv`
- `zip_dma.csv`

---

## How to Run

### 1. Install Dependencies
```bash
pip install pandas numpy matplotlib scipy scikit-learn

### 2. Calculate Gap Scores
Open the notebook calculate_gap_scores.ipynb and run all cells.

### 3. Run Clustering

Run the clustering script after generating the gap scores.

### Requirements


### Run
Clustering.ipynb

### Input
- gap_scores.csv (ensure you ran the previous python file so you have this file in the same folder)

### Output
- gap_score_only_dendrogram.png  
- gap_only_clustered.csv
