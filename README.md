# High-vs-Low-Anxiety-Classifier
This project uses machine learning to classify individuals into high or low anxiety categories based on their digital behavior patterns. The dataset includes simulated data on screen time, app usage, sleep hours, and social media consumption.

🧠 Objective
To build a robust classification model that can predict whether a person has high anxiety (score ≥ 7) or low anxiety based on their digital activity and self-reported scores.

📁 Dataset
Name: mental_health_digital_behavior_data.csv

Features:
-daily_screen_time_min: Total screen time in minutes
-num_app_switches: Number of app switches
-sleep_hours: Hours slept
-notification_count: Number of notifications received
-social_media_time_min: Time spent on social media
-focus_score: Self-reported focus score (1–10)
-mood_score: Self-reported mood score (1–10)
-anxiety_level: Self-reported anxiety level (1–10) — used to create a binary label
-high_anxiety: Binary target variable derived from anxiety_level (1 if ≥ 7, else 0)

🧪 Methodology

1. Data Cleaning:
Dropped missing values.

2. Feature Engineering:
Created a binary classification target: high_anxiety.

3. Feature Scaling:
Applied StandardScaler to normalize feature values.

4. Model Building:
Used a Stacking Classifier with-
Base learners: RandomForestClassifier, XGBClassifier
Meta learner: LogisticRegression

5. Evaluation:
Generated a classification report.
Calculated accuracy on the test set.

🚀 How to Run
1. Install dependencies:
!pip install pandas scikit-learn xgboost
2. Ensure the dataset is named mental_health_digital_behavior_data.csv.
3. Run the notebook High&LowAnxiety.ipynb.

📈 Output
Classification Report: Includes precision, recall, F1-score.
Accuracy: Overall accuracy of the model on the test data.

🔮 Potential Improvements
Add hyperparameter tuning (GridSearchCV).
Introduce cross-validation scoring.
Include model explainability using SHAP or LIME.
Deploy the model with Streamlit or Flask.

🧑‍💻 Author
Developed by Diya Goswami
For mental health and AI integration research and exploration.
