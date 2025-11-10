# Solar Data Discovery: Week 0 Challenge

## 🌍 Project Overview
This repository contains my submission for Week 0 of the 10 Academy AI Mastery training challenge. The project involved a comprehensive analysis of solar farm data from three West African countries: Benin, Sierra Leone, and Togo.

Acting as an Analytics Engineer for MoonLight Energy Solutions, the goal was to profile, clean, and analyze the data to identify high-potential regions for solar investment, supporting the company's operational efficiency and long-term sustainability goals.

## 🎯 Business Objective
MoonLight Energy Solutions aims to enhance its strategic solar investments. This analysis provides a data-driven case by:

- Identifying key trends and insights from environmental measurement data.
- Comparing solar potential across Benin, Sierra Leone, and Togo.
- Delivering actionable recommendations for targeting high-yield regions.

## 📊 Dataset
The dataset comprises time-series measurements from solar radiation sensors, including:

- **Solar Irradiance**: GHI, DNI, DHI, ModA, ModB
- **Weather Data**: Ambient Temperature, Relative Humidity, Wind Speed/Direction, Barometric Pressure, Precipitation
- **Operational Data**: Module Temperatures (TModA, TModB), Cleaning Events

## 🚀 Repository Structure
solar-challenge-week0/
├── .github/workflows/ # CI/CD GitHub Actions configuration
│ └── ci.yml
├── app/ # Streamlit Dashboard (Bonus Task)
│ ├── main.py
│ └── utils.py
├── data/ # Raw and cleaned data (ignored by Git)
│ ├── benin_clean.csv
│ ├── sierra_leone_clean.csv
│ └── togo_clean.csv
├── notebooks/ # Jupyter Notebooks for EDA and Analysis
│ ├── benin_eda.ipynb
│ ├── sierra_leone_eda.ipynb
│ ├── togo_eda.ipynb
│ └── compare_countries.ipynb
├── src/ # Source code for modules and scripts
├── tests/ # Unit tests
├── .gitignore # Files and folders to ignore
├── requirements.txt # Python dependencies
└── README.md # Project documentation (this file)

markdown
Copy code

## ✅ Tasks Completed

**Task 1: Git & Environment Setup**
- Initialized the GitHub repository and set up a Python virtual environment.
- Implemented Git branching strategy with descriptive commits.
- Configured GitHub Actions for Continuous Integration (CI).
- Established a professional project structure and comprehensive `.gitignore`.

**Task 2: Data Profiling, Cleaning & EDA**
For each country (Benin, Sierra Leone, Togo):
- Generated summary statistics and missing value reports.
- Performed outlier detection using Z-scores (|Z| > 3) for key metrics.
- Cleaned data by imputing missing values and handling outliers.
- Conducted extensive time-series analysis, correlation studies, and distribution plots.
- Explored the impact of cleaning events on sensor readings.
- Exported cleaned datasets to CSV files.

**Task 3: Cross-Country Comparison**
- Loaded and synthesized cleaned data from all three countries.
- Created comparative visualizations (boxplots, summary tables).
- Performed statistical testing (ANOVA/Kruskal-Wallis) to validate differences in solar potential.
- Summarized key findings and ranked countries based on average GHI.

## 📈 Key Findings & Insights
- Country X demonstrated the **highest median Global Horizontal Irradiance (GHI)**, indicating strong overall solar potential.
- Country Y showed the **greatest variability in solar readings**, suggesting a need for more robust system design to handle fluctuations.
- A significant positive correlation was observed between **ambient temperature and solar irradiance**, though this relationship was moderated by relative humidity.
- Statistical testing confirmed that the **differences in solar potential between the countries are significant**, providing a strong basis for targeted investment strategies.
- Statistical testing confirmed that the **differences in solar potential between the countries are significant**, providing a strong basis for targeted investment strategies.
