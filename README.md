# instructor-effectiveness-modeling
Machine learning project for instructor effectiveness modeling using learner outcomes, engagement, and feedback data in an EdTech setting.

# Instructor Effectiveness Modeling.

## Overview

This project was completed as part of the Data Science.

The objective is to analyze instructor performance using learner outcomes, engagement metrics, and learner feedback collected across multiple course batches. Since instructor effectiveness labels were not provided, a composite Instructor Effectiveness Score was designed and used to classify instructors into Low, Medium, and High effectiveness tiers.


## Dataset

The dataset consists of **2,000 course batches** taught by **120 instructors**.

Each record contains:

- Batch ID
- Instructor ID
- Course ID
- Learner outcome metrics
- Engagement metrics
- Feedback metrics


## Project Workflow

1. Data Loading & Inspection
2. Data Cleaning
3. Exploratory Data Analysis (EDA)
4. Correlation Analysis
5. Instructor Effectiveness Score Design
6. Batch-to-Instructor Aggregation
7. Effectiveness Tier Creation
8. Machine Learning Model Training
9. Model Evaluation
10. Feature Importance Analysis
11. Business Insights & Limitations


## Models Used

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier

Models were compared using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix


## Feature Engineering

- Normalized numerical features using MinMaxScaler.
- Converted dropout rate into a retention metric.
- Designed a composite Instructor Effectiveness Score using:
  - Learner Outcomes
  - Learner Engagement
  - Learner Feedback
- Aggregated batch-level data to instructor-level using mean statistics.
- Included the number of batches taught (`batch_count`) as an additional feature.
- Created effectiveness tiers using quantile-based binning.


## Key Findings

- Learner outcome metrics were the strongest indicators of instructor effectiveness.
- Completion rate and dropout rate showed a strong negative correlation.
- Engagement and feedback metrics provided complementary predictive information.
- Random Forest offered strong predictive performance while providing interpretable feature importance.


## Limitations

- Instructor effectiveness labels were not available and were constructed from existing features.
- The model does not account for course difficulty, learner demographics, or instructor experience.
- Results should be used as decision-support rather than as the sole basis for instructor evaluation.



## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook


## Repository Structure

```
├── Neeraj_Kumar_Instructor_Effectiveness_Modeling.ipynb
├── README.md
```


## Author

**Neeraj Kumar**

Data Science | Machine Learning | Python | SQL
