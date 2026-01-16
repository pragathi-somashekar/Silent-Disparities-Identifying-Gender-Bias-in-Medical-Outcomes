📌 **Overview**

This project analyzes potential **gender bias in medical outcome predictions** using large-scale healthcare data and distributed Big Data techniques. The goal is to determine whether machine learning models systematically favor one gender in clinical risk estimation and whether such disparities persist after controlling for clinical factors.

Using **PySpark**, distributed DataFrames, and scalable ML pipelines, the project processes thousands of patient records to examine patterns in diagnosis accuracy, model calibration, and prediction fairness across genders.


 📂 **Data & Preprocessing**

The dataset includes demographic variables, diagnostic codes, lab values, vitals, and medical outcomes. Key steps include:

* Data ingestion using **Spark SQL** and DataFrames
* Cleaning missing values & outlier handling
* Feature engineering (risk indicators, categorical encoding)
* Normalization & train–validation–test splits
* Building scalable ML pipelines using Spark MLlib


🔍 **Key Steps & Analysis**

* **Descriptive statistics & visualizations** to compare male vs. female outcome distributions
* Heatmaps, bar charts, and probability curves to observe systemic differences
* Statistical testing to identify whether performance gaps are significant
* Analysis of mean predicted risk vs. actual outcomes across gender groups


🤖 **Models Implemented**

Using Spark MLlib:

* Logistic Regression
* Random Forest Classifier
* Decision Tree Classifier
* Gradient-Boosted Trees

Each model is evaluated on:

* Accuracy & F1-score
* ROC-AUC
* Calibration curves
* Gender-wise prediction differences


📈 **Results**

Across models, the **difference in predicted risk between genders was minimal**, suggesting limited evidence of gender-based algorithmic bias. Logistic Regression and Random Forest showed the strongest performance and produced nearly identical mean probability estimates for male and female patients. Disparities—when present—were statistically small and model-dependent rather than demographic-driven.


📌 **Conclusion**

This project demonstrates how **Big Data tools and scalable ML pipelines** can be used to evaluate fairness in healthcare analytics. The results indicate that the models learned clinical patterns without disproportionately misclassifying one gender, supporting more equitable and unbiased medical decision systems.


📁 **Repository Includes**

* PySpark preprocessing scripts
* SQL queries & feature engineering code
* ML pipelines for all models
* Visualizations and fairness metrics
* Complete PDF final report


 ✨ **Tech Stack**

* **PySpark**, Spark SQL
* Spark MLlib
* Python
* Pandas, NumPy
* Matplotlib / Seaborn
