# Stroke Prediction Capstone

TS Academy Data Science capstone: a group project (team of 12) predicting stroke risk and segmenting patients using the Kaggle Stroke Prediction Dataset.

## Dataset
[Stroke Prediction Dataset (Kaggle)](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset): 5,110 patient records. The data is not included in this repository.

## Tools
Python, Pandas, NumPy, SQL, SQLite, Scikit-learn, Matplotlib, Google Colab

## My Contribution
- Feature engineering and encoding (age group, comorbidity count, glucose category)
- K-Means clustering of patients
- Coordinated the group and reviewed the team's work

## Key Results
- Stroke rate rises sharply with age: 13.15% for patients 60+ versus 0.79% for ages 30–44.
- Patients with hypertension had a 13.25% stroke rate, compared with 3.97% without.
- K-Means grouped patients into 4 segments. The older group with heart and blood-sugar conditions had the highest stroke rate (14.10%).
- Final model: Logistic Regression with a tuned decision threshold (0.12). ROC AUC 0.84 and F1 0.30, versus 0.50 and 0.04 for a baseline that ignores the data.
- Stroke cases are rare in the data, so the threshold was chosen on validation data to avoid leaking information from the test set.

## How to Run
Open `stroke-prediction-capstone.ipynb` in Google Colab and run all cells.
