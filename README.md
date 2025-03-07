# **Food_Recognition_Classification**

This repository presents an advanced **machine learning model** designed to analyse the relationship between **ingredients, healthiness ratings, and likability** of food items. The project explores how the presence of **oil** in a dish influences its perceived healthiness and preference ratings. The methodology incorporates **feature selection, classification models, and model performance evaluation**.

---

## **1. Project Overview**
This project investigates key factors influencing food preferences, focusing on **ingredients, healthiness ratings, and likeness scores**. The primary objective is to **understand how the presence of oil in food impacts its overall health perception and consumer preference**.

### **Key Objectives**
- **Identify correlations** between oil presence, health ratings, and likability.
- **Develop machine learning models** for predictive analysis.
- **Evaluate classification performance** using accuracy, precision, recall, and F1-score.

---

## **2. Dataset**
The **MLEndYD dataset** is used for this study, which is loaded via `yummy_small_load` from the `mlend` library. The dataset consists of:

- **Ingredients** – The list of ingredients in a dish.
- **Healthiness Rating** – A numerical score indicating the dish’s health perception.
- **Likeness Score** – A rating based on consumer preference.

The dataset is processed by:
- **Reading image attributes** from a CSV file and storing them in a **Pandas DataFrame**.
- **Extracting relevant features** for machine learning analysis.

---

## **3. Problem Formulation**
This study addresses a common dilemma: **balancing taste and health in food consumption**. Specifically, it investigates:

- The role of **oil** in food taste enhancement.
- The **long-term health implications** of consuming oily food.
- The **correlation between oil presence, health perception, and likability**.

By exploring these relationships, the study provides insights into how **ingredients shape consumer food choices**.

---

## **4. Methodology**
The project follows a structured **machine learning pipeline**:

### **Model Training and Validation**
1. **Data Splitting**
   - The dataset is divided into **training and testing sets**.

2. **Label Encoding**
   - Converts the `healthiness_status` variable into a numerical format.

3. **Feature Selection**
   - Identifies key predictive features (**presence of oil**).

4. **Handling Missing Values**
   - Uses **mean imputation** to ensure data completeness.

5. **Model Selection**
   - **Random Forest** and **Support Vector Machine (SVM)** classifiers are chosen.

6. **Model Training**
   - Both models are trained on the **training dataset**.

7. **Model Validation**
   - Performance is assessed on the **testing dataset**.

### **Model Performance Assessment**
1. **Accuracy Score**
   - Measures the overall correctness of predictions.

2. **Classification Report**
   - Provides **precision, recall, F1-score, and support metrics**.

3. **Confusion Matrix**
   - Visual representation of **true positives, false positives, true negatives, and false negatives**.

### **Rationale**
- **Comprehensive Evaluation**: Multiple performance metrics ensure a holistic understanding.
- **Interpretability**: Detailed insights into precision, recall, and error distribution.
- **Comparative Analysis**: Allows performance comparison between **Random Forest and SVM models**.

---

## **5. Transformation Stage**
The dataset undergoes the following transformations:

### **Feature Extraction**
1. **Healthiness Status**
   - A new categorical column (`healthiness_status`) is created based on **healthiness and likeness scores**.

2. **Oil Presence**
   - A **binary feature (`has_oil`)** is created to indicate whether a dish contains **specific oil-related ingredients**.

---

## **6. Model Evaluation**
At the end of the training process, models are evaluated using:

- **Accuracy Score** – Overall model performance.
- **Precision & Recall** – Trade-off between false positives and false negatives.
- **F1-Score** – Balance between precision and recall.
- **Confusion Matrix** – Breakdown of classification outcomes.

### **Performance Insights**
- **Random Forest vs. SVM**:
  - The **Random Forest classifier** demonstrated **higher generalisation** on unseen data.
  - The **SVM model** performed well on **specific food categories** but required hyperparameter tuning.

---

## **7. Visualisation & Monitoring**
Key plots and metrics are generated to track model performance:

- **Feature Importance Plot**: Highlights key factors influencing food likability and health ratings.
- **Classification Reports**: Summarises **precision, recall, and F1-scores**.
- **Confusion Matrix**: Graphical representation of **correct and incorrect predictions**.

---
