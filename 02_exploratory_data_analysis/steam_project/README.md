# Steam – Big Data Analysis

## Project Description
This project aims to support Ubisoft in understanding the current video game ecosystem by analyzing data from the Steam marketplace. The objective is to uncover key trends across publishers, genres, languages, platforms, and release timelines.

## Objectives
- Conduct macro-level, genre-based, and platform-based analysis
- Identify the most prolific publishers and best-rated games
- Study the evolution of releases over time (including Covid period)
- Analyze price distribution, discounts, and high-value categories
- Explore genre popularity and average review performance
- Compare platform availability across Windows, Mac, and Linux

## Data Processing
The dataset was processed using PySpark within a Databricks environment to handle a large number of records efficiently. The workflow included:

- loading and inspecting large datasets
- cleaning and filtering records
- aggregating data by publisher, genre, and platform
- computing metrics such as review scores and price distributions

## Tech Stack
- PySpark
- Databricks
- Python
- Spark DataFrames
- Data visualization in Databricks

## Folder Structure
```text
steam_project/
│
├── notebooks/
│   ├── steam.html     # version lisible + visualisations
│   └── steam.ipynb    # version réexécutable
│
└── README.md
```

## How to Use
- Open Steam.html to view the full analysis and all charts
- Import Steam.ipynb into Databricks to rerun or extend the analysis
