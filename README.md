# Stroke Risk Prediction

This project uses machine learning to predict the risk of stroke based on patient health data. It was developed as part of an MSc Statistical Machine Learning Course.

## Project Overview

The notebook `stroke-risk-prediction.ipynb` walks through the entire data science process:
- Loading and exploring the dataset
- Cleaning and preprocessing the data
- Selecting important features
- Handling class imbalance
- Training machine learning models
- Evaluating model performance
- Interpreting the results

## Technologies Used

- Python 3
- Kaggle Notebook
- Dataset (Taken from Kaggle)
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

## How to Run

1. Clone this repository:
git clone https://github.com/your-username/stroke-risk-prediction.git
2. Open the folder and launch the notebook using Jupyter:
cd stroke-risk-prediction
jupyter notebook stroke-risk-prediction.ipynb
3. Run all cells in order.
4. Note - **I have attached a seperate dataset. If anyone wants to use that dataset, it's needed to change the section of the notebook ***Loading Dataset***.**
**(e.g., data = pd.read_csv('stroke-data.csv')**

**Another point to be noted that, if anyone use Jupyter notebook, the package ***pip install imbalanced-learn*** is needed to run in the terminal**

## Dataset
The dataset includes medical and lifestyle details such as:
- Age
- Gender
- Hypertension
- Heart disease
- Smoking status
- BMI
- Glucose level

The target variable is whether the patient has had a stroke.

## Objective

The aim is to build an accurate and interpretable model that can help flag individuals at higher risk of stroke for early medical intervention. Here I focused on **Recall** and **ROC-AUC** rather than **Accuracy**. **Recall** tells how many actual positive cases a model correctly predicted. 
**Formula**
$$
\text{Recall} = \frac{\text{True Positives (TP)}}{\text{True Positives (TP)} + \text{False Negatives (FN)}}
$$
- True Positives (TP): Correctly predicted positives
- False Negatives (FN): Actual positives that the model missed

## Importance of Recall
Recall is especially important when missing positive cases is costly.
Examples:
- Medical diagnoses (missing a stroke patient can be dangerous)
- Fraud detection
- Disease outbreaks

## License

This project is for academic and educational purposes only.

