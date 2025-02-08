> # **EDA and Machine Learning : Global Road Accidents**
- **[View the notebook `on GitHub`](https://github.com/mayur-de/Data_Analysis_and_Modeling/blob/2af18b8ca68159655d73ab2f7879462619f928f2/EDA_ML_Road_Accidents/EDA%20-%20Global%20Road%20Accidents.ipynb)**
- **[View the notebook `on Kaggle`](https://www.kaggle.com/code/mayurkumardeshmukh/comprehensive-eda-global-road-accident)**
- **[View the Machine Learning notebook `on GitHub`](https://github.com/mayur-de/Data_Analysis_and_Modeling/blob/fee2d82f3033ffdae025c407eae661f17170e3eb/EDA_ML_Road_Accidents/ML%20-%20%5BClassification%5D%20-%20Road%20Accidents.ipynb)**

> ## Overview
- This document provides a comprehensive EDA of a dataset containing **132,000 accident entries** over **30 columns**.
- Machine learning models are applied to classify and predict various target variables related to road accidents.

> ## EDA: Key Findings
- **Data Inspection**: No null values or duplicates were found. Data types were adjusted, and a new 'Date' feature was created.
- **High-Level Data Overview**:
  - Numerical variables showed low correlations.
  - Categorical variables' frequency distributions were visualized.
- **Key Metrics**:
  - **Accident Data**: 
    - Total accidents: **132,000**
    - Total fatalities: **263,398**
    - Total injuries: **1,255,083**
    - Total accidents involving alcohol: **12,500** (approx. 9.5% of total accidents)
  - **Economic Impact**: 
    - Total medical cost: **$3.3 billion**
    - Total economic loss: **$6.6 billion**
  - **Emergency Response**:
    - Average emergency response time: **32.49 minutes**
    - Percentage of accidents with delayed emergency response (over 60 minutes): **8%**
  - **Temporal Analysis**:
    - Accidents peaked in **July** with **11,500** accidents recorded.
    - The **highest severity** was recorded on **weekdays**, particularly between **4 PM - 7 PM**.

> ## Analysis Insights
- **Temporal Trends**: Accident trends were analyzed by year, month, and time of day, revealing patterns in severity and impact.
- **Geographic Trends**: Accident severity and impact were analyzed by country and urban/rural areas.
- **Driver & Vehicle Factors**: Driver age, gender, fatigue, and alcohol levels were analyzed for their role in accident severity.
- **Environmental & Road Conditions**: Weather, road type, conditions, and traffic volume were considered in relation to accident severity.
- **Severity & Impact**: Relationships between accident severity, causes, and vehicle involvement were examined.

> # **Machine Learning**
- **[View the Machine Learning notebook `on GitHub`](https://github.com/mayur-de/Data_Analysis_and_Modeling/blob/fee2d82f3033ffdae025c407eae661f17170e3eb/EDA_ML_Road_Accidents/ML%20-%20%5BClassification%5D%20-%20Road%20Accidents.ipynb)**
## `1.` Classification: Model Evaluation Summary

## `1.1` Logistic Regression
- **Accuracy:** 33.56%, similar to random guessing.
- **Precision, Recall, and F1-Score:** Low (~33-34%) across all classes, indicating poor classification performance.
- **Confusion Matrix:** Predictions are almost evenly spread across classes, showing poor feature separability.

## `1.2` Random Forest Classifier
- **Accuracy:** 33.52%, no significant improvement over Logistic Regression.
- **Precision, Recall, and F1-Score:** Consistently low (~33-34%) across all severity levels.
- **Confusion Matrix:** High misclassification across all classes.
- **Feature Importance:** Economic factors (`Economic Loss`, `Medical Cost`, `Insurance Claims`) dominate, while road/weather conditions seem less predictive.

## `1.3` XGBoost
- **Accuracy:** 33.22%, still close to random guessing.
- **Precision, Recall, and F1-Score:** Similar to other models (~33%), indicating no significant learning of patterns.
- **Confusion Matrix:** High misclassification rate, failing to separate accident severity levels effectively.

## **Overall Conclusion: Classification**
- All three models perform poorly, with accuracy around 33%, indicating an inability to distinguish between severity levels.
- The models struggle due to:
  - **Poor feature separability**.
  - **Lack of strong predictive variables**.
  - **Imbalanced data**.
