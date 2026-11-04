# Hospital Readmission Prediction

This project predicts whether a patient is readmitted to the hospital or not.  used the **Diabetes 130-US Hospitals** dataset to predict whether a patient would be readmitted within 30 days.

I trained and compared a **Decision Tree** and a **Random Forest** model.

## What I Did

- Downloaded and cleaned the dataset from UCI.
- Converted readmission status into a binary target.
- Split the data by patient ID to avoid having the same patient in training and testing.
- Handled missing values and encoded categorical features.
- Trained two classification models and compared them with a basic baseline.
- Evaluated accuracy, precision, recall, F1 score, ROC-AUC and average precision.
- Visualized a confusion matrix, a Decision Tree and feature importance.
- Saved the selected model using Joblib.

## Tools Used

Python, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, Requests and Joblib.

## How to Run

1. Open `Hospital_Readmission_Prediction.ipynb` in Google Colab.
2. Run all the cells in order. The notebook downloads the public dataset automatically.
3. Check the evaluation results and visualizations.
4. The final cell saves `hospital_readmission_model.joblib` in the Colab session.

If you are running locally, install the packages listed in `requirements.txt` first.

## Dataset

[Diabetes 130-US Hospitals (UCI Machine Learning Repository)](https://archive.ics.uci.edu/dataset/296/diabetes+130-us+hospitals+for+years+1999-2008)

## Note

This is an educational ML project. The positive class is relatively rare, and a model with good accuracy can still miss readmissions or give false alerts. The results should not be used for medical decisions.
