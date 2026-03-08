# Kayak – Data Collection & Infrastructure

## Project Description
Kayak is a travel search engine that helps users plan their trips by comparing prices for flights, hotels, and car rentals. To enrich the user experience, the marketing team wants to launch a destination recommendation feature based on real data (weather, hotels, etc.).

This project aims to build a robust data infrastructure capable of collecting, storing, and preparing travel-related data, weather forecasts and hotel listings, for France’s top 35 destinations.

## Objectives
- Automate the collection of weather and hotel data for major tourist cities in France.
- Store the raw and processed data in a cloud-based data lake (S3) and warehouse (NeonDB).
- Provide clean, structured datasets ready for analytics and recommendations.

## Data Pipeline
The project follows a simple data pipeline:

1. Collect weather data from external APIs.
2. Scrape hotel information for selected cities.
3. Store raw data locally and in AWS S3.
4. Clean and aggregate the data.
5. Store structured datasets in a PostgreSQL database (NeonDB).
6. Generate visualizations to support travel recommendations.

## Tech Stack
- Python
- APIs
- Web Scraping
- AWS S3
- NeonDB – PostgreSQL
- Plotly

## Folder Structure
```text
.
├── .env                 
├── .env.example         # Copy .env.example to .env and fill in your own keys before running the notebook         
│
├── data/
│   ├── raw/             # Raw data (API, scraping, ignored in git)
│   │   ├── all_hotels.csv
│   │   ├── cities_coords.csv
│   │   └── weather_daily_7d.csv
│   │
│   └── processed/       # Cleaned & aggregated datasets
│       ├── best_hotels.csv
│       ├── top5.csv
│       └── weather_avg_score.csv
│
├── charts/              # Plotly interactive visualizations
│   ├── best_hotels.html
│   ├── cities_weather_score.html
│   └── top_5_cities_weather_score.html
│
├── notebooks/           # Main development notebook
│   └── kayak.ipynb
│
├── screenshots/         
│   ├── s3_bucket/       # S3 structure (raw + processed)
│   │   ├── kayak_bucket.png
│   │   ├── raw_data.png
│   │   └── processed_data.png
│   │
│   └── neon_db/         # Database tables in NeonDB
│       ├── city_table.png
│       ├── weather_table_01.png
│       ├── weather_table_02.png
│       ├── hotel_table_01.png
│       └── hotel_table_02.png
│
└── README.md             
```