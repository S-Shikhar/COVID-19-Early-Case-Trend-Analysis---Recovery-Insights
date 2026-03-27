# COVID-19 Early Case Analysis & Recovery Insights

## Project Overview

This project analyzes early-stage COVID-19 patient data to understand infection patterns, demographic trends, and recovery behavior. The goal is to extract meaningful insights that can support public health decision-making.

---

## Objectives

* Identify **who is getting infected** (age, gender, region)
* Understand **how infections are spreading**
* Analyze **recovery trends and timelines**
* Determine **factors affecting recovery time**
* Build predictive models for recovery duration

---

## Dataset Description

The dataset contains patient-level records with the following features:

### 🔹 Demographics

* `sex`
* `birth_year`
* `country`
* `region`

### 🔹 Infection Details

* `infection_reason`
* `infection_order`
* `infected_by`

### 🔹 Exposure Metrics

* `contact_number`

### 🔹 Timeline Data

* `confirmed_date`
* `released_date`
* `deceased_date`

### 🔹 Outcome

* `state` (released, isolated, deceased)

---

## Tech Stack

* **Language:** Python
* **Libraries:**
  * Pandas
  * NumPy
  * Matplotlib
  * Seaborn
  * Scikit-learn

---

## Project Workflow

### 1. Data Cleaning

* Converted date columns to datetime
* Created `age` from birth year
* Handled missing values intelligently
* Created cleaned datasets for analysis

### 2. Feature Engineering

* Created `recovery_days`
* Generated age groups
* Built separate datasets for EDA and ML

### 3. Exploratory Data Analysis (EDA)

* Gender distribution
* Age and age group analysis
* Regional case concentration
* Infection source analysis

### 4. Recovery Analysis

* Distribution of recovery time
* Recovery vs age, gender
* Correlation analysis

### 5. Machine Learning Models

* **Linear Regression**
* **Random Forest Regressor**

### 6. Model Evaluation

* R² Score
* Mean Absolute Error (MAE)
* Model comparison

---

## Key Insights

* Most affected age group: **36–60 years**
* Major hotspots: **Gyeongsangbuk-do and Capital Area**
* Common infection sources:
  * Contact with infected individuals
  * Travel-related exposure
* Average recovery time: **~15 days**

---

## Model Findings

* Random Forest performed better than Linear Regression
* Age had higher influence on recovery compared to gender
* Dataset size limited model performance

---

## Limitations

* High number of missing values in infection-related fields
* Limited recovery data (~28 samples)
* Results are **exploratory, not definitive**

---

## 📁 Project Structure

```
├── patient.csv
├── cleaned_eda_data.csv
├── recovery_data.csv
├── eda_analysis.ipynb
├── model_and_insights.ipynb
├── README.md
```

---

## Future Improvements

* Use larger dataset for better modeling
* Apply advanced models (XGBoost, Neural Networks)
* Build interactive dashboard (Streamlit / Power BI)

---

## Conclusion

This project demonstrates how data analytics and machine learning can be applied to understand disease spread and recovery patterns. Despite data limitations, meaningful insights were extracted to support healthcare strategies.

---

## Author

**Souharda Shikhar Biswas**
B.Tech Computer Science
Adamas University
