# Patient Segmentation Using K‑Means Clustering
## Overview
This project applies K‑Means clustering to identify meaningful patient segments based on Age and Initial Days spent in the hospital. The goal is to uncover actionable patterns that support personalized care strategies, operational planning, and resource optimization.
## Business Question
Can K‑Means clustering identify actionable patient clusters using Age and Initial Days?
## Goal of Analysis
The analysis aims to segment patients into distinct groups based on age and initial hospital stay length. These clusters help the hospital understand patient patterns, anticipate care needs, and design targeted interventions that improve efficiency and patient outcomes.
## Clustering Technique
### Method: 
K‑Means clustering
### Features used: 
- Age
- Initial_days

### Process:
- Standardized features
- Removed outliers using Z‑score thresholds
- Evaluated cluster quality using elbow plot and silhouette score
- Outcome: Four well‑defined clusters representing different patient profiles
## Data Preparation
- Loaded and explored the dataset
- Checked for duplicates and missing values
- Removed outliers using Z‑score capping
- Scaled features to ensure equal contribution to distance calculations
- Exported cleaned and scaled data for modeling

## Optimal Number of Clusters
### Determined using:
- Elbow plot (WCSS)
- Silhouette score

Both methods indicated k = 4 as the optimal number of clusters
- Silhouette score: 0.54, indicating moderately strong cluster separation
## Results
The K‑Means model produced four distinct patient clusters:
- Cluster 0: Younger patients with longer hospital stays
- Cluster 1: Younger patients with shorter stays
- Cluster 2: Older patients with extended stays
- Cluster 3: Older patients with short stays
These clusters reveal meaningful patterns in care utilization and help identify opportunities for targeted interventions.
## Implications
- Younger patients with long stays may require closer monitoring or follow‑up
- Routine cases among younger patients highlight opportunities for workflow optimization
- Older patients with long stays may benefit from enhanced discharge planning and chronic‑care coordination
- Older patients with short stays may represent efficient care pathways worth replicating
## Limitations
- Unsupervised learning lacks ground‑truth labels, making validation challenging
- Only two variables were used, which may oversimplify patient complexity
- Additional features could reveal deeper or more nuanced patterns
## Recommendations
- Cluster 0: Increase monitoring and review care delays
- Cluster 1: Continue optimizing workflows and use as a benchmark
- Cluster 2: Implement targeted senior‑care strategies and early discharge planning
- Cluster 3: Analyze successful care pathways and replicate across other groups
