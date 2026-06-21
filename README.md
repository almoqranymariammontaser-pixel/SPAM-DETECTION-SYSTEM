# 📧 Spam Detection System using Machine Learning & NLP

## 📌 Project Overview

This project aims to automatically classify SMS messages as either:

- Ham (Legitimate Message)
- Spam (Unwanted/Advertising Message)

The project uses Natural Language Processing (NLP) techniques and multiple Machine Learning algorithms to build an accurate spam detection system.

---

## 🎯 Objectives

- Clean and preprocess text messages.
- Extract meaningful features using TF-IDF.
- Handle class imbalance.
- Train and compare multiple machine learning models.
- Evaluate model performance using several metrics.
- Save trained models for future deployment.

---

## 📂 Dataset

Dataset: **SMS Spam Collection Dataset**

Features:

- Message Text
- Label (Ham / Spam)

Target Variable:

- 0 → Ham
- 1 → Spam

---

## 🧹 Data Preprocessing

The following preprocessing steps were applied:

### Text Cleaning

- Convert text to lowercase
- Remove URLs
- Remove numbers
- Remove punctuation
- Remove extra spaces

### NLP Processing

- Tokenization
- Stopwords Removal
- Lemmatization

### Feature Engineering

Additional feature:

- Spam Keywords Detection

Examples:

- Free
- Winner
- Prize
- Cash
- Offer
- Urgent
- Congratulations

---

## ✂️ Train-Test Split

The dataset was divided into:

- 80% Training Data
- 20% Testing Data

Stratified splitting was used to preserve class distribution.

---

## 🔤 Feature Extraction

### TF-IDF Vectorization

Parameters:

- Max Features: 5000
- N-Grams: (1,2)
- Min Document Frequency: 2
- Max Document Frequency: 0.9

---

## 🤖 Machine Learning Models

The following models were trained and evaluated:

### 1. Naive Bayes

Multinomial Naive Bayes with balanced sample weights.

### 2. Logistic Regression

Balanced Logistic Regression for spam classification.

### 3. Support Vector Machine (SVM)

Linear kernel SVM with probability estimation.

### 4. Random Forest

Ensemble model using multiple decision trees.

### 5. Decision Tree

Optimized Decision Tree with overfitting protection.

---

## 📊 Evaluation Metrics

Models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Cross Validation

---

## 📈 Visualizations

The project generates:

- Model Accuracy Comparison
- Precision Comparison
- Recall Comparison
- F1 Score Comparison
- Confusion Matrices
- Cross Validation Results

---

## 💾 Saved Outputs

After training, the project automatically saves:

```text
models/
├── naive_bayes_model.pkl
├── logistic_regression_model.pkl
├── svm_model.pkl
├── random_forest_model.pkl
└── decision_tree_model.pkl
```

Additional outputs:

```text
results/
├── comparison_results.csv
├── visualizations/
└── evaluation_reports
```

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- NLTK
- Scikit-Learn
- Matplotlib
- Seaborn
- TF-IDF Vectorizer

---

## 📁 Project Structure

```text
Spam-Detection-System/
│
├── spam_detection.ipynb
├── spam.csv
├── models/
├── results/
└── README.md
```

---

## 🚀 How to Run

### Clone Repository

```bash
git clone https://github.com/your-username/spam-detection-system.git
```

### Install Dependencies

```bash
pip install pandas numpy nltk scikit-learn matplotlib seaborn scipy
```

### Run Notebook

```bash
jupyter notebook
```

Open:

```bash
spam_detection.ipynb
```

---

## 🎓 Key Learning Outcomes

- Natural Language Processing (NLP)
- Text Cleaning and Preprocessing
- TF-IDF Feature Extraction
- Feature Engineering
- Machine Learning Classification
- Model Evaluation
- Cross Validation
- Model Persistence using Pickle

---

## 👩‍💻 Author

**Mariam Montasser**

Computer Science Student

GitHub: https://github.com/your-username

---

## ⭐ If you found this project useful, consider giving it a star!
