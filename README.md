# Smart Food Waste Prediction and Optimization System

[![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=flat&logo=python&logoColor=white)](https://www.python.org/)
[![Apache Spark](https://img.shields.io/badge/Apache_Spark-3.x-E25A1C?style=flat&logo=apachespark&logoColor=white)](https://spark.apache.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Latest-F7931E?style=flat&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Machine Learning](https://img.shields.io/badge/Focus-Machine_Learning-blue.svg)]()

An intelligent data-driven system designed to predict food consumption, reduce food wastage, and optimise operational efficiency in large-scale cafeteria environments using **Machine Learning** and **Big Data technologies**.

The system analyses historical food preparation and consumption data, learns behavioural patterns, recommends optimal food preparation quantities, and identifies abnormal waste behaviour to support informed decision-making.

---

## Project Overview

Food wastage in institutional food services often occurs due to manual estimation, static planning, and lack of data-driven insights. This project addresses the problem by integrating scalable data processing with predictive analytics.

The system combines:
- **Apache Spark** for Big Data processing  
- **Machine Learning models** for accurate demand prediction  
- **Optimisation logic** to reduce overproduction  
- **Anomaly detection** to identify inefficient operational days  

---

## Key Objectives

- Predict daily food consumption accurately.
- Recommend optimal food preparation quantities.
- Reduce food wastage and associated financial loss.
- Detect abnormal waste patterns using Isolation Forest.
- Provide actionable insights through visual analytics.
- Demonstrate end-to-end ML + Big Data integration.

---

## System Architecture

Data Collection  
↓  
Apache Spark Processing  
↓  
Feature Engineering  
↓  
Machine Learning Model Training  
↓  
Prediction & Optimization  
↓  
Anomaly Detection  
↓  
Visualization & Insights  

---

## Project Structure

```text
Smart-Food-Waste-Prediction-and-Optimization-System/
│
├── data/
│   └── food_waste_dataset_enhanced.csv
│
├── notebooks/
│   └── main.ipynb
│
├── models/
│   └── (trained models available via GitHub Releases)
│
├── README.md
└── .gitignore

```

## Dataset Description

* **Records:** 20,000  
* **Format:** CSV  
* **Type:** Structured tabular dataset  

### Key Features:
| Feature | Description |
| :--- | :--- |
| **Date and Day** | Temporal patterns |
| **Weather conditions** | Impact of climate on attendance |
| **Student count** | Core demand driver |
| **Meal type** | Breakfast, Lunch, Dinner |
| **Food waste (kg)** | Target for reduction |
| **Event indicator** | Special occasions/holidays |

---

## Machine Learning & Anomaly Detection

### Predictive Modeling
The system evaluates multiple regression models to find the best fit:
* **Linear Regression**
* **Random Forest Regressor**
* **Gradient Boosting Regressor**

### Anomaly Detection
Implemented using **Isolation Forest** to identify days with unusually high food wastage, helping managers spot specific operational failures.

---

---

## Visualization and Analytics

The system includes multiple visual insights generated via **Matplotlib** and **Seaborn**:

* **Model Performance Comparison:** Evaluating R² and Error metrics across different algorithms.
* **Actual vs. Predicted Trends:** Visualizing how closely the model tracks real-world food consumption.
* **Waste Distribution & Cost Analysis:** Breaking down the financial impact of overproduction.
* **Anomaly Detection Plots:** Clear identification of outlier days using Isolation Forest results.
* **Before vs. After Optimization:** Side-by-side comparison showing the effective percentage of waste reduction.

---




## How to Run the Project
### 1. Requirements
Ensure you have Python installed.

```bash
pip install pyspark pandas numpy scikit-learn matplotlib seaborn
```

### 2. Execution Steps
1. Navigate to the `notebooks/` directory.
2. Open `main.ipynb` in **VS Code** or **Jupyter Notebook**.
3. Run all cells sequentially.
4. The system will output predictions, optimized quantities, and anomaly reports.


## Trained Model Files

Due to GitHub file size limitations, trained `.pkl` model files are stored in the **Releases** section.  
👉 [**Download Models Here**](https://github.com/ajydeep/Smart-Food-Waste-Prediction-and-Optimization-System/releases)

> **Note:** Alternatively, the models can be regenerated locally by running the notebook end-to-end.

---
