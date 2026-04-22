# team138

### 1. Install Dependencies
pip install pandas numpy matplotlib scipy scikit-learn

### Clean Data
This generates clean_data.csv for the gap score calculation
Ensure the following files are in the **same folder**:
### Required files
- `state_recency.csv`
- `zip_dma.csv`
- `laws_and_incentives.csv`
- `data_clean.ipynb`


### EV Gap Score Generation

This generates state-level EV **Gap Scores**, which measure the difference between EV policy strength and charging infrastructure.

---

## Required Files

Ensure the following files are in the **same folder**:

- `gap_score.ipynb`
- `clean_data.csv`
- `state_recency.csv`
- `zip_dma.csv`
- `vehicle_registration_data.csv`

---

### Calculate Gap Scores
Open the notebook calculate_gap_scores.ipynb and run all cells.
You can verify the correlation coefficient between gap score and EV adoption rate
This will generate gap_scores.csv for clustering code. 
--- 
## Run Clusetering Algorithm
This generates state-level EV **Clustering**, which creates a hierarchical clustering of each state depending on their gap score. 

## Open Clustering.ipynb

## Input
- gap_scores.csv (ensure you ran the previous python file so you have this file in the same folder)

## Output
- gap_score_only_dendrogram.png  
- gap_only_clustered.csv
---
### Open Dendrogram Locally
