# 🏋️ Model Fitness: Customer Churn Prediction

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![Scikit-Learn](https://img.shields.io/badge/ML-Scikit--Learn-orange.svg)
![Seaborn](https://img.shields.io/badge/Viz-Seaborn-green.svg)
![Status](https://img.shields.io/badge/Status-Completed-success.svg)

## 📖 Project Overview
**Model Fitness**, a premium gym chain, is developing a data-driven strategy to improve customer retention. The management team is concerned about "churn" (customers leaving).

This project focuses on analyzing customer profiles and digital interaction data to **predict the probability of churn** for each customer in the upcoming month. The goal is to design retention strategies based on behavioral patterns.

## 🎯 Business Objectives
1. **Learn to predict** the probability of churn (at the individual level) for the next month.
2. **Create user clusters** (segmentation) to identify distinct behavioral groups.
3. **Analyze key features** that impact retention (e.g., contract period, group visits, age).
4. **Provide recommendations** to reduce churn and improve customer engagement.

## 📂 Data Description
The dataset contains 4,000 records of gym members with the following features:
* **User Data:** `gender`, `Near_Location` (lives/works nearby), `Partner` (employee of a partner company), `Promo_friends` (referral).
* **Behavioral Data:** `Contract_period` (1, 6, 12 months), `Group_visits`, `Age`, `Avg_additional_charges_total`.
* **Engagement:** `Month_to_end_contract`, `Lifetime` (months since first visit), `Avg_class_frequency`.
* **Target Variable:** `Churn` (1 if the user left, 0 if they stayed).

## 🛠️ Methodology & Tech Stack
**Tools:** Python, Pandas, Scikit-learn, Seaborn, Matplotlib, SciPy.

**Key Steps:**
1. **Exploratory Data Analysis (EDA):**
   * Visualized feature distributions for churned vs. loyal customers.
   * Computed a **Correlation Matrix** to identify multicollinearity and strong predictors.
2. **Machine Learning (Supervised - Classification):**
   * Trained and compared two models: **Logistic Regression** and **Random Forest Classifier**.
   * **Metrics Used:** Accuracy, Precision, Recall, and ROC-AUC.
3. **User Clustering (Unsupervised):**
   * Standardized data using `StandardScaler`.
   * Built a **Dendrogram** to determine the optimal number of clusters.
   * Applied **K-Means Clustering** to segment users into 5 distinct groups.

## 💡 Key Findings
> *Insights derived from the model and clustering analysis:*

* **Strongest Predictors:** The features most strongly correlated with retention are `Lifetime`, `Avg_class_frequency_current_month`, and `Contract_period`.
* **High-Risk Segments:** Users with 1-month contracts who rarely attend group classes are significantly more likely to churn.
* **Model Performance:** The **Logistic Regression** model achieved an Accuracy of `[Insertar Score, ej: 0.92]` and a Recall of `[Insertar Score]`.
* **Cluster Insights:** The "Loyal" cluster typically lives near the gym and has a 12-month contract, while the "At-Risk" cluster visits less than once a week.

## 🚀 Recommendations
* **Contract Incentives:** Promote 12-month contracts with discounts to shift users away from 1-month plans.
* **Group Integration:** Create "Newbie" group classes to encourage social engagement early in the membership.
* **Partner Programs:** Strengthen corporate partnerships as these employees show lower churn rates.

## 💻 How to Run
1. Clone the repository:
   ```bash
   git clone (https://github.com/Kshadow098/14.ModelFitness.git)
