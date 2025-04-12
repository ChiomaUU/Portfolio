# 🌍 NPRI Emissions Prediction and Environmental Impact Analysis

This project focuses on preparing and analyzing the **National Pollutant Release Inventory (NPRI)** dataset to develop machine learning-ready data for **environmental impact prediction**. The goal was to clean, explore, merge, and transform emissions data in order to build models that can forecast future pollutant trends and support better policy decisions.

> 📊 Developed as part of **CMPT 2400 – Data Preparation & Analytics**, in collaboration with **Environment and Climate Change Canada (ECCC)**.

---

## 🎯 Project Objectives

- 🧼 Clean and preprocess NPRI data for releases, disposals, and transfers
- 🧩 Align and merge multiple datasets into one analytical base table
- 🔎 Explore trends, outliers, and reporting inconsistencies
- 🔢 Encode and normalize features to build ML-ready data
- 🏗️ Engineer new features (e.g., proportions, pollutant ratios, trends)
- 🔮 Build predictive models to forecast future emissions and reporting behavior

---

## 🛠 Technologies Used

- Python (Pandas, NumPy)
- Jupyter Notebooks
- scikit-learn
- Plotly / Matplotlib
- Git & GitHub
- Optional: Dash (for interactive dashboard)

---

## 📁 Dataset
NPRI_Releases.csv - https://drive.google.com/file/d/13DeyFXucHf_U0zfI3LLFlVJW4lIH7YpE/view?usp=sharing
NPRI_Disposals and Transfers.csv - https://drive.google.com/file/d/1WLbt5G9PneNmYTiqNys0_EbtCWe_sKrd/view?usp=sharing
NPRI_Comments.csv - https://drive.google.com/file/d/1wrogE1VGhz69uvo1aPSuCFO3K-cCHhUD/view?usp=sharing

---

## 🔍 Project Milestones

### 🔹 Phase 1: EDA and Data Cleaning
- Identified missing values, bad housekeeping issues, scale mismatches
- Removed or imputed missing values, justified decisions in code
- Explored pollutant distributions, reporting trends by industry/province

### 🔹 Phase 2: Dataset Alignment & Merging
- Merged `releases`, `disposals`, and `comments` tables using facility and year
- Conducted integrity checks for duplication and data alignment
- Matched pollutant reporting with external variables (e.g., oil prices, GDP)

### 🔹 Phase 3: Feature Engineering
- Encoded categorical features (e.g., NAICS codes, provinces)
- Engineered new columns like:
  - Ratios (releases to disposals)
  - Predicted vs. actual emissions
  - Year-on-year trend indicators
- Normalized numeric features for modeling

### 🔹 Phase 4: Predictive Modeling
- Framed multiple regression problems such as:
  - Predicting CO and NOx emissions in oil & gas sector under crude oil price scenarios
  - Forecasting emissions trends based on federal carbon pricing
  - Estimating reporting behavior and emissions volumes across provinces

---

## 💡 Key Insights

- **Carbon pricing policies** appear to correlate with reduced emissions from some sectors
- **Oil & gas** remains the highest emitter across multiple pollutant types
- Predictive models show measurable trends in NOx and CO reduction over time
- Provinces with stricter regulations (e.g., BC) showed clearer pollutant decline patterns

---

## 📈 Optional Feature: Interactive Dashboard

An interactive dashboard (Plotly Dash) was prototyped to:
- Display emissions trends across provinces and sectors
- Allow filtering by pollutant type and timeframe
- Visually compare landfill vs. treatment methods

---

## 📄 Acknowledgments

This project was developed in collaboration with **Environment and Climate Change Canada (ECCC)** as part of the CMPT 2400 curriculum at NorQuest College.

We would like to thank our instructors and the ECCC team for providing datasets, real-world feedback, and ongoing support during demo and feedback sessions.

---

## 📜 License

This project is for academic and demonstration purposes only.
