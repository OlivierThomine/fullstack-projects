# Getaround – Model Deployment

## Project Description
Getaround is a peer-to-peer car rental platform where late vehicle returns can create conflicts between consecutive bookings.
This project analyzes rental delays to quantify their operational impact and support product decisions such as introducing buffer times between rentals.
The project also includes a machine learning model designed to support pricing optimization, deployed through an API and connected to a web dashboard for interactive exploration.

## Objectives
- Analyze the impact of rental overlaps and late checkouts.
- Help define a buffer time policy between rentals.
- Build and deploy a machine learning model to suggest optimal prices.
- Provide a functional API and documentation for external use.

## Project Components
The project includes several components:
- **Exploratory Data Analysis** to understand rental delay patterns.
- **Machine Learning model** to estimate optimal rental prices.
- **FastAPI service** exposing the trained model.
- **Streamlit dashboard** to visualize insights and predictions.
- **MLflow tracking** for experiment management.

## Tech Stack
- Python  
- Pandas  
- Scikit-learn  
- Streamlit  
- FastAPI  
- MLflow  
- AWS S3  
- Hugging Face Spaces  

## Folder Structure
```text
.
├── data/           # datasets (ignored in git)
├── notebooks/
├── scripts/
└── README.md
```
