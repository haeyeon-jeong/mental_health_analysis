# Mental Health Stress Analysis & Prediction

## Authors

Haeyeon Jeong | Sai Rachana Kandikattu | Abirham Getie | Yonathan Shimelis  

---

## Project Overview

This project analyzes mental health survey data to identify key factors influencing stress and treatment behavior. Using statistical analysis and machine learning models, we explore patterns in mental health outcomes and build predictive models for growing stress.

### Key Questions
- What are the top factors influencing growing stress?
- Do individuals with a family history seek treatment?
- What factors impact stress among students?

---

## Dataset

- Source: Mental Health Survey Dataset (Kaggle)
  https://www.kaggle.com/datasets/bhavikjikadara/mental-health-dataset  
- Size: ~292,000 records  
- Type: Survey-based categorical data  

### Features Include
- Demographics: Gender, Country, Occupation  
- Behavioral: Days Indoors, Work Interest, Changes in Habits  
- Mental Health: Mood Swings, Family History, Treatment  
- Target Variable: `Growing_Stress`  

---

## Data Preprocessing

- Removed missing values  
- Dropped irrelevant columns (`Timestamp`, `Country`, `self_employed`)  
- Converted categorical variables to numeric format  
- Removed ambiguous `"Maybe"` values from target variable  
- Applied one-hot encoding for categorical features (Occupation)  

---

## Exploratory Data Analysis

- Distribution analysis using count plots and pie charts  
- Correlation heatmaps  
- Chi-square statistical testing  

### Key Insights
- Family history has a strong relationship with treatment  
- Increased indoor time is associated with higher stress  
- Mood swings strongly correlate with stress levels  
- Students show distinct stress patterns  

---

## Models Implemented

### Logistic Regression
- Accuracy: ~54%  
- AUC: 0.58  

---

### Decision Tree
- Accuracy: ~84%  
- AUC: ~0.94  

---

### Random Forest (Best Model)
- Accuracy: ~91%  
- AUC: ~0.97  

---

### K-Nearest Neighbors (KNN)
- Lower performance  
- High variance and overfitting  

---

## Key Findings

### Top Factors Influencing Stress
- Mental Health History  
- Days Indoors  
- Work Interest  
- Mood Swings  
- Changes in Habits  

---

### Family History vs Treatment
- Strong statistical relationship (p < 0.05)  
- Individuals with family history are more likely to seek treatment  

---

### Student-Specific Insights
- Changes in habits  
- Days indoors  
- Mood swings  
- Social weakness  
- Gender differences  

---

## Model Evaluation

- Accuracy Score  
- Confusion Matrix  
- ROC Curve & AUC  
- Cross-validation  

---

## How to Run

1. Open the file:
- Team7_Mental_Health_Code_Analysis.py  

2. Make sure the dataset is in the same directory:
- Download `Mental Health Dataset.csv.zip`
- Unzip it to get `Mental Health Dataset.csv`  
- Place the `.csv` file in the same directory as the Python script  

3. Install dependencies:
```bash
pip install numpy pandas matplotlib seaborn scikit-learn plotly altair yellowbrick
```
---

## Presentation

- `report/Team7_Mental_Health_Analysis_F.pdf` contains the presentation slides for this project  

This file summarizes the problem, methodology, analysis, models, and key findings.

