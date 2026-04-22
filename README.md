# team138

## 1. Install Dependencies
```bash
pip install pandas numpy matplotlib scipy scikit-learn
```

---

## Clean Data
This generates `clean_data.csv` for the gap score calculation.

### Required Files
Ensure the following files are in the same folder:
- `state_recency.csv`
- `zip_dma.csv`
- `laws_and_incentives.csv`
- `data_clean.ipynb`

---

## EV Gap Score Generation
This generates state-level EV **Gap Scores**, which measure the difference between EV policy strength and charging infrastructure.

### Required Files
Ensure the following files are in the same folder:
- `gap_score.ipynb`
- `clean_data.csv`
- `state_recency.csv`
- `zip_dma.csv`
- `vehicle_registration_data.csv`

---

## Calculate Gap Scores
Open the notebook `calculate_gap_scores.ipynb` and run all cells.

You can verify the correlation coefficient between gap score and EV adoption rate.  
This will generate `gap_scores.csv` for clustering code.


## Run Clusetering Algorithm
This generates state-level EV **Clustering**, which creates a hierarchical clustering of each state depending on their gap score. 

## Open Clustering.ipynb

## Input
- `gap_scores.csv` (ensure you ran the previous python file so you have this file in the same folder)

## Output
- `gap_score_only_dendrogram.png`
- `gap_only_clustered.csv`
---
### Open Dendrogram Locally

## Requirements
- Visual Studio or any IDE
- For Visual Studio install 'Live Server' by Ritwick Dey

## Required Files
- `cluster_gap_score.html`
- data >> `gap_only_clustered.csv`
- lib >> `d3.v5.min.js` and `topojson.v2.min.js`

Open the folder Code on Visual Studio and then right click on `cluster_gap_score.html` file and click 'Open with Live Server`
This should open a browser tab with the dengrogram.

---
### Dashboard Information

==================================================
IDENTIFYING ELECTRIC VEHICLE INFRASTRUCTURE GAPS
==================================================


PROJECT DESCRIPTION
-------------------

This project aims to examine the alignment between state-level electric vehicle policies and the availability of charging infrastructure across the U.S. The objective is to find out which states are passing lots of EV laws but still do not have enough chargers to back it up and delivers insights through interactive visual analytics.

The project utilized multiple national datasets, including state-level EV policy data, charging infrastructure data, vehicle registration data, and ZIP level population data. From these datasets, several metrics are constructed, including policy score,infrastructure score, EV adoption rate. The gap score is calculated as the difference between normalized policy score and normalized infrastructure score, and normalized EV adoption rate. Finally, hierarchical clustering analysis is performed to group the states into four cluster based on the gap score.

The project provides four interactive dashboards for users to explore how different states compare in terms of charging infrastructure distribution, gap scores and policy effects, identify states with over or balanced EV ecosystems as well as those where policy and infrastructure mismatched, these dashboards also highlight similarities among states, and provide a "what if" simulation tool for user to explore when there is policy/infrastructure/EV adaptation change, how it will affect a state's gap score.


INSTALLATION 
-------------------

No installation is required to view the visualization.
Users can access the interactive dashboards directly through the Tableau link provided in the Execution section.


EXECUTION
-------------------

To view the visualization dashboards:

1) Open the Tableau dashboard using the link below in your web browser:
<https://public.tableau.com/app/profile/anuradha.nugawela/viz/CSEProject_v4/IdentifyEVInfrastuctureGaps>

2)The dashboards will be loaded directly in the browser, for a better view, see it in full screen.

3) Use the interactive features(filters, tooltips, and map navigation) in the dashboards, users can explore:
a.EV charging infrastructure distribution across states (1st dashboard)
b.Gap scores by states dynamically (2nd dashboard)
c.Policy score vs Infrastructure (2nd dashboard) 
d.EV adoption patterns (2nd dashboard)
e.Gap score ranking and State details (2nd dashboard)
f.States cluster by gap score (3nd dashboard)
g.Click the arrow in the 3nd dashboard, users can explore the interactive hierarchical clustering dendrogram.
h.what if analysis (4th dashboard)
