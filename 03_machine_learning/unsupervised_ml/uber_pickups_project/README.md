# Uber Pickups – Unsupervised Learning

## Project Description
Uber aims to improve its customer experience by reducing pickup delays, which often occur when there is a mismatch between user location and driver availability. This project focuses on identifying "hot zones" in New York City—areas and times where demand is highest—so drivers can be proactively positioned in advance.

## Objectives
- Detect spatial and temporal hotspots of ride requests in NYC.
- Compare clustering techniques (e.g., KMeans vs DBSCAN) to identify the most accurate method.
- Help Uber drivers optimize their location strategy to reduce user wait time.

## Methodology
The analysis focuses on identifying geographic hotspots of ride demand using unsupervised learning techniques.

Main steps:
1. Data cleaning and preprocessing of Uber trip records.
2. Aggregation of pickup locations.
3. Application of clustering algorithms (KMeans and DBSCAN).
4. Comparison of clustering results to identify the most relevant hotspots.
5. Visualization of pickup density and clusters on NYC maps.

## Tech Stack
- Python  
- Pandas  
- Scikit-learn  
- Plotly  

## Folder Structure
```text
.
├── data/           # datasets (ignored in git)
├── notebooks/
└── README.md
```