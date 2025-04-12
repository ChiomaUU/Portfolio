# 🏡 Kijiji & RentFaster Rental + Restaurant Analysis

This project explores the relationship between **rental listings** in Alberta (from Kijiji and RentFaster) and the **quality and proximity of nearby restaurants** using the **Yelp API**. Built using **Apache Spark**, the project showcases how large-scale, real-world datasets can be integrated and analyzed in a distributed environment to extract useful insights for community housing access and urban planning.

> 📍 In partnership with the **Community Data Program**, the project supports making rental data more accessible to communities with limited data access.

---

## 🧰 Tools & Technologies

- 🐍 Python
- ⚡ Apache Spark & Spark SQL
- 🌐 Yelp API
- 📄 CSV data from Kijiji and RentFaster (web scraping)
- 🗃️ Jupyter Notebook
- 📊 Data visualization tools (Matplotlib, Seaborn, etc.)

---

## 📂 Project Structure

- `data/` – Contains cleaned and raw CSV files from Kijiji and RentFaster  
- `presentation/` – Project slide deck showcasing findings  
- `notebooks/` – Main analysis notebook with Spark SQL integration  
- `screenshots/` – Optional visuals from Spark UI or analysis results

---

## 🔍 Project Objectives

### Part 1: Data Collection  
- Web scraped rental data from RentFaster and Kijiji  
- Collected both **overview** and **detailed** data in CSV format  
- Retrieved restaurant data using the Yelp API (location, price, ratings)

### Part 2: Data Management  
- Initialized and ran Spark in local mode  
- Created Spark DataFrames and temporary SQL tables  
- Joined rental listings with nearby restaurant information

### Part 3: Data Exploration  
- Explored correlations between **rental price** and **restaurant quality/price**  
- Identified areas with high concentration of highly rated restaurants and higher rent  
- Discussed limitations in Yelp data and proposed improvements

---

## 💡 Key Insights

- There is evidence of a positive correlation between **rental prices** and the **presence of highly rated, mid-to-high priced restaurants** nearby.
- Data quality from Yelp was decent but limited in some regions, affecting the completeness of the analysis.
- Spark enabled scalable data processing and made it easier to handle large joined datasets from different sources.

---

## 📈 Future Improvements

- Expand geographic coverage beyond Alberta  
- Enhance data quality by cross-referencing with additional APIs  
- Deploy interactive dashboards for public or municipal use  
- Automate pipeline using scheduled scraping and streaming tools

---

## 🙋‍♀️ Team & Acknowledgment

This project was completed as part of the **CMPT Data Management Systems Final Project** with the support of the **Community Data Program**.

---

## 📄 License

This project is for educational and non-commercial use only.


