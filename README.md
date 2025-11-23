# Covid-19 Global Vaccination Analysis

This project analyzes global COVID-19 vaccination data to uncover regional disparities, manufacturer distribution patterns, and rollout trends across countries.

> Course: DSC450, Applied Data Science  
> Authors: Ryan Weeks, Sarah Yawn, Lisa Hansen

---

## 📊 Project Overview

The project focuses on:

- Tracking how vaccination coverage changed globally over time  
- Comparing vaccination progress across countries and regions  
- Exploring which manufacturers and vaccines dominated different markets  
- Preparing clean, validated data for downstream modeling and forecasting

My primary responsibility in this project was the **Wrangler role**, which focused on cleaning, joining, and structuring the data so the rest of the team could model and visualize it reliably.

Phase 1 centers on data wrangling, validation, and exploratory analysis.  
Phase 2 uses the cleaned data for modeling in a separate notebook.

---

## 📁 Repository Structure

- `notebooks/COVID19_Wrangler.ipynb`  
  Data wrangling and exploratory analysis. Handles loading the Kaggle data, cleaning, joining country and manufacturer files, working with missing values, and creating summary tables and plots.

- `notebooks/COVID19_Models.ipynb`  
  Modeling and additional analysis built on top of the cleaned dataset.

- `docs/COVID19_Analysis_Project_Proposal.docx`  
  Initial project proposal outlining goals, scope, and planned methods.

- `docs/COVID19_Report.docx`  
  Formal project report describing methods, results, and conclusions.

- `data/`  
  Folder intended for raw CSVs from Kaggle (not committed to the repo).

> Note: Large raw CSV files are not stored in this repository.  
> Download them directly from Kaggle (see below) and place them in `data/`.

---

## 📚 Data Source

Dataset:

- COVID World Vaccination Progress, Gpreda (2021)  
  https://www.kaggle.com/datasets/gpreda/covid-world-vaccination-progress

Place the following files in the `data/` directory if you want to reproduce the analysis locally:

- `country_vaccinations.csv`  
- `country_vaccinations_by_manufacturer.csv`

---

## 🔍 Wrangler Phase Highlights (My Role)

Wrangling and EDA work in `COVID19_Wrangler.ipynb` includes:

- Loading and joining country level and manufacturer level vaccination datasets  
- Cleaning column names and standardizing country labels  
- Handling missing values and inconsistent entries  
- Creating derived features such as:  
  - Daily vaccination counts and rolling averages  
  - Cumulative vaccinations by country  
  - Vaccinations per hundred  
  - Manufacturer shares by country or region  
- Building initial visualizations, for example:  
  - Global vaccination progress over time  
  - Top countries by total vaccinations and per hundred metrics  
  - Manufacturer usage across different regions

This creates a stable, well structured dataset that the team can then use for modeling and more advanced analysis in the `COVID19_Models.ipynb` notebook.

---

## 🧰 Tech Stack

- Python  
- pandas, NumPy  
- Matplotlib, seaborn  
- Jupyter Notebook

---

## 🚀 Next Steps (Beyond the Wrangler Phase)

Later project phases, supported by the cleaned data, extend this work by:

- Applying time series models for vaccination forecasting  
- Exploring clustering of countries by rollout patterns  
- Evaluating relationships between vaccine manufacturers and rollout efficiency

These steps are documented in the modeling notebook and the written report.

---

## 👥 Collaborators

- **Ryan Weeks** – Data Wrangler  
- **Sarah Yawn** – Data Scientist and modeling  
- **Lisa Hansen** – Presenter and visualization lead

---

## 📄 License

This project is licensed under the MIT License.  
See the `LICENSE` file for details.
