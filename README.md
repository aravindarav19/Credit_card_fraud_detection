
# Credit Card Fraud Detection Using Random Forest

## Project Overview

This project focuses on building a machine learning model to detect fraudulent credit card transactions. It uses the Random Forest algorithm and addresses class imbalance with SMOTE (Synthetic Minority Over-sampling Technique). The dataset comprises anonymized features and real transaction data, providing a robust foundation for fraud detection.

---

## Objectives

- Detect fraudulent transactions with high accuracy.
- Address the class imbalance problem in the dataset.
- Provide a model evaluation using key metrics like Precision, Recall, F1 Score, and ROC AUC Score.

---

## Dataset

- **Source**: [Provide dataset source, if applicable]
- **Total Records**: 284,807 transactions
- **Features**:
  - **Time**: Transaction timestamp
  - **Amount**: Transaction amount
  - **V1 to V28**: Anonymized features derived from PCA
  - **Class**: Target variable (0 = Non-Fraud, 1 = Fraud)

---

## Key Steps

### 1. Data Preprocessing
- Ensured target column `Class` is of integer type.
- Handled missing values using forward fill.
- Scaled numerical features using `StandardScaler`.

### 2. Handling Class Imbalance
- Used SMOTE to oversample the minority class (fraudulent transactions).

### 3. Model Development
- **Algorithm**: Random Forest Classifier
- **Parameters**:
  - `n_estimators`: 100
  - `random_state`: 42
- **Data Split**: 80% training, 20% testing (stratified split).

### 4. Model Evaluation
- **Metrics**:
  - Accuracy: 1.00
  - Precision: 0.87
  - Recall: 0.83
  - F1 Score: 0.85
  - ROC AUC Score: 0.98
- **Confusion Matrix**:
  - True Positives: 81
  - True Negatives: 56,852
  - False Positives: 17
  - False Negatives: 12

---

## Results

The Random Forest model demonstrated high accuracy and a good balance between precision and recall. Using SMOTE improved the model's ability to identify fraudulent transactions effectively.

### Highlights:
- High Precision minimizes false alarms.
- Improved Recall ensures fraudulent transactions are detected.
- An excellent ROC AUC score of 0.98 confirms robust performance.

---

## Future Work

- Hyperparameter tuning for further optimization.
- Experimenting with additional features or different algorithms.
- Incorporating real-time detection capabilities.

---

## Files in This Repository

1. **`Credit Card Fraud Detection Using Random Forest.ipynb`**: Jupyter Notebook containing the full implementation.
2. **`creditcard.csv`**: Dataset used for the analysis.
3. **`Credit_Card_Fraud_Detection_Presentation.pptx`**: Project presentation summarizing key findings.

---

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/credit-card-fraud-detection.git
   ```
2. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook "Credit Card Fraud Detection Using Random Forest.ipynb"
   ```

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---
