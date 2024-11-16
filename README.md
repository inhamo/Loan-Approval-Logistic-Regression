# 🚀 Loan Default Prediction: Handling Imbalanced Data for High Performance

## 📘 Overview

This project focuses on predicting loan default likelihood using a logistic regression model. The dataset presented challenges such as imbalanced classes and noisy data, which were addressed through robust data cleaning, feature engineering, and undersampling techniques.

**Key Highlights:**
- End-to-end pipeline for data preprocessing, feature engineering, and modeling.
- Tackling imbalanced data with undersampling to improve model performance.
- Optimization of the logistic regression model using hyperparameter tuning and feature selection.

---

## 📂 Project Structure

```
Loan_Default_Prediction/
├── data/                  # Placeholder for dataset
├── notebooks/             # Jupyter notebooks for exploration and model building
├── src/                   # Scripts for data processing, modeling, and evaluation
├── results/               # Outputs such as confusion matrix plots and metrics
├── README.md              # Project documentation (this file)
└── requirements.txt       # Dependencies for the project
```

---

## 🛠️ Steps in the Project

### 1. **Data Understanding and Cleaning**
- Analyzed the dataset for missing values, duplicates, and outliers.
- Removed unrealistic values (e.g., ages below 18 or over 99).
- Filtered employment and credit history fields based on logical constraints.

### 2. **Feature Engineering**
- Created domain-specific features like:
  - **Age Group**: Categorized applicants into Young, Middle-aged, and Elderly groups.
  - **Risk Level**: Mapped loan intent and age group to risk categories.
  - **Financial Strain Risk**: Derived based on loan-to-income ratio.
- Dropped irrelevant columns and capped extreme outliers in income.

### 3. **Dealing with Imbalanced Data**
- Addressed the class imbalance (only ~2% of defaults) by:
  - Using **undersampling** to create a balanced dataset.

### 4. **Modeling**
- Used **Logistic Regression** as the base model.
- Optimized hyperparameters (`C`, `penalty`, and `solver`) via **GridSearchCV**.
- Selected the top 10 features using Recursive Feature Elimination (RFE).

### 5. **Evaluation**
- Evaluated the model on metrics such as Accuracy, Precision, Recall, F1-Score, and AUC.
- Achieved high performance despite the imbalanced nature of the dataset.

---

## 🎯 Results

| Metric       | Value   |
|--------------|---------|
| **Accuracy** | 93.67%  |
| **Precision**| 92.11%  |
| **Recall**   | 95.11%  |
| **F1-Score** | 93.58%  |
| **AUC**      | 0.9816  |

The model demonstrated robust performance, accurately identifying loan defaults while maintaining a balance between precision and recall.

---

## 📊 Visualization
- Confusion Matrix showing classification performance:
![Confusion Matrix](results/confusion_matrix.png) *(Replace with your actual path)*

---

## 🚀 Getting Started

### Prerequisites
Ensure you have the following installed:
- Python 3.8+
- Libraries: See `requirements.txt`

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Loan_Default_Prediction.git
   cd Loan_Default_Prediction
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Add your dataset to the `data/` directory.

### Run the Pipeline
1. Preprocess the data:
   ```bash
   python src/preprocess.py
   ```
2. Train and evaluate the model:
   ```bash
   python src/train_model.py
   ```

---

## 📈 Key Learnings
- The importance of **domain knowledge** in crafting meaningful features.
- Effective strategies for addressing **class imbalance** and ensuring model fairness.
- The power of **hyperparameter tuning** and **feature selection** to enhance model performance.

---

## 🤝 Contributing
Contributions are welcome! If you'd like to improve this project, feel free to fork it and submit a pull request.

---

## 📧 Contact
If you have any questions or feedback, feel free to reach out:
- **Email:** itnhamo@gmail.com
- **LinkedIn:** [Innocent Nhamo](https://www.linkedin.com/in/innocent-nhamo-467008254/)

---

### ⭐ If you find this project useful, give it a star! 😊

