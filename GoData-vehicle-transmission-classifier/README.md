# 🚗 GoData Vehicle Transmission Classifier

This project focuses on building a **machine learning model** to automatically classify whether a vehicle has an **automatic or manual transmission** using structured vehicle listing data. The solution is intended to help streamline data labeling and improve vehicle inventory accuracy for Go Auto.

> 🧠 This project was completed as part of the **CMPT 2400 - Data Preparation & Analytics** course in collaboration with Go Auto.

---

## 🎯 Project Goal

Develop a supervised learning model that classifies transmission type (`Automatic` or `Manual`) based on vehicle attributes such as:

- Make & Model
- Year
- Price
- Odometer (Mileage)
- VIN-decoded fields (e.g., body style, drivetrain)

---

## 🧰 Tools & Technologies

- Python (Pandas, NumPy, scikit-learn)
- MLflow (model tracking and experiment logging)
- SHAP (model explainability)
- Streamlit (interactive web app for predictions)
- Jupyter Notebooks
- Git & GitHub

---

## 📂 Dataset
CBB_Listings.csv - https://drive.google.com/file/d/1_t5gnYeDzfnW_PXP4h_1oH0vdoOkhP_J/view?usp=sharing

## 🔍 Workflow Overview

### 1. 🧹 Data Cleaning & Feature Engineering
- VIN-decoded features cleaned and encoded
- Manual corrections for inconsistent or missing values
- Target encoded as binary (0 = Manual, 1 = Automatic)

### 2. 🧠 Model Development
- Used `RandomForestClassifier`
- Performed hyperparameter tuning using `GridSearchCV`
- Tracked experiments using MLflow

### 3. 📊 Model Evaluation
- Evaluated using accuracy, precision, recall, and F1-score
- Visualized feature importance using SHAP

### 4. 🚀 Deployment
- Deployed the model as a Streamlit app for live predictions
- Input: user-provided vehicle specs
- Output: predicted transmission type with SHAP explanation

---

## 💡 Key Outcomes

- Achieved high accuracy (~90%+) on unseen test data
- SHAP analysis highlighted that **Price**, **Odometer**, and **Year** are key predictors
- Final model correctly classified 4,000+ vehicles in testing
- Streamlit app demoed live predictions with visual feedback

---

## 📈 Lessons Learned

- Applied practical data cleaning and imputation techniques
- Understood the importance of stakeholder feedback during model iteration
- Integrated explainability and UI for stakeholder transparency
- Improved experience in deploying ML models and versioning experiments

---

## 👥 Team & Acknowledgment

Project developed in collaboration with **Go Auto** and evaluated in the **CMPT 2400** course at NorQuest College.  
Thanks to Go Auto stakeholders and course instructors for continuous feedback and support.

---

## 📄 License


This project is for educational and demonstration purposes only.

# Phase 2 - Vehicle Transmission Classifier Makefile Guide

This project provides a Makefile to manage the environment setup and tasks for training and prediction of a vehicle transmission classification model.

## Makefile Commands

### Environment Setup
- **Setup Virtual Environment**

```bash
make init
```
This command sets up a Python virtual environment and installs dependencies from `requirements.txt`.

### Running Tasks
- **Preprocess Data**
```bash
make preprocess
```
Executes the `preprocess.py` script in the `src` directory to prepare the dataset.

- **Train the Model**
```bash
make train
```
Executes the `train.py` script located in the `src` directory to train the vehicle transmission classification model.

- **Run Predictions**
```bash
make predict
```
Executes the `predict.py` script located in the `src` directory to make predictions with the trained model.

- **Evaluate the Model**
```bash
make evaluate
```
Executes the `evaluate.py` script located in the `src` directory to evaluate model performance.

### Cleaning Up
- **Clean Cache and Logs**
```bash
make clean
```
Removes `__pycache__` directories, the virtual environment, and cache files.

### Help
- **Display Available Commands**
```bash
make help
```
Lists all available Makefile commands with a brief description.

---

## Instructions for Environment Setup

1. Use `make init` to set up the environment.
2. Activate the virtual environment:
```bash
source .venv/bin/activate
```
3. Install additional dependencies by updating `requirements.txt`.

---

## Notes
- Ensure you have Python 3.8+ installed.
- The `clean` command will remove the virtual environment, so use it with caution.


