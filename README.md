# WEEK-5-ASSIGNMENT
1. Problem Definition (6 points)
Hypothetical Problem: Predicting student dropout rates in higher education institutions.

Objectives:

Identify students at risk of dropping out early.

Recommend personalized interventions to retain students.

Improve overall student retention rates.

Stakeholders:

University Administration

Students and Parents

KPI:
Percentage reduction in dropout rate over one academic year.

2. Data Collection & Preprocessing (8 points)
Data Sources:

Student academic records (grades, attendance)

Learning Management System (LMS) usage logs

Potential Bias:
Socioeconomic status may be underrepresented, leading to biased predictions against disadvantaged students.

Preprocessing Steps:

Handle missing data using imputation techniques (e.g., mean or mode).

Normalize numeric features to standardize scales.

Encode categorical variables (e.g., gender, program) using one-hot encoding.

3. Model Development (8 points)
Chosen Model:
Random Forest — it handles both categorical and numerical data well, provides feature importance, and is robust to overfitting.

Data Splitting Strategy:
Split data into 70% training, 15% validation, and 15% test set.

Hyperparameters to Tune:

max_depth – Controls tree complexity and helps prevent overfitting.

n_estimators – Number of trees in the forest; affects model accuracy and training time.

4. Evaluation & Deployment (8 points)
Evaluation Metrics:

Precision – Important to avoid false positives (e.g., mislabeling a student as at risk).

Recall – Ensures most at-risk students are identified (true positives).

Concept Drift:
Occurs when data patterns change over time, reducing model performance.
Monitoring Strategy: Use rolling windows of accuracy, retrain periodically on recent data.

Deployment Challenge:
Scalability – Integrating the model into existing LMS platforms across multiple departments with varying data formats.
