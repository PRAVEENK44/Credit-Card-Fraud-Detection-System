# Credit Card Fraud Detection System

A high-performance machine learning solution designed to identify and flag fraudulent credit card transactions in real-time. This system utilizes advanced ensemble learning techniques to ensure financial security with minimal false positives.

## 🚀 Overview

Fraudulent transactions represent one of the most significant challenges in modern fintech. This project implements a robust detection pipeline capable of analyzing transaction patterns and classifying them as legitimate or fraudulent with high precision.

### Key Features
- **High-Performance Modeling**: Leverages XGBoost (Extreme Gradient Boosting) for state-of-the-art classification accuracy.
- **Class Imbalance Management**: Implements SMOTE (Synthetic Minority Over-sampling Technique) to handle the 0.17% fraud ratio in the dataset.
- **Real-Time Inference**: A Flask-based API designed for low-latency transaction validation.
- **Comprehensive Analytics**: Deep feature importance analysis and model evaluation metrics (Precision-Recall, AUC-ROC).

---

## 🛠️ Technology Stack

- **Core Logic**: Python 3.10+
- **Machine Learning**: XGBoost, Scikit-Learn, Pandas, NumPy
- **API Framework**: Flask
- **Data Engineering**: SMOTE (imbalanced-learn), StandardScaler

---

## 📊 Technical Architecture

The system follows a standard data science lifecycle:
1.  **Exploratory Data Analysis (EDA)**: Identification of transaction patterns and feature correlations.
2.  **Preprocessing**: Custom encoders for categorical data (State, Job, Category) and standard scaling for numerical features (Amount).
3.  **Resampling**: Addressing class imbalance using SMOTE to improve model recall for minority classes.
4.  **Training**: Gradient Boosted Trees with early stopping and hyperparameter optimization.
5.  **Validation**: Stratified K-Fold cross-validation to ensure model stability.

---

## 📈 Performance Results

The final model achieves industry-leading performance on the Kaggle Credit Card Fraud dataset:

| Metric | Score |
| :--- | :--- |
| **Accuracy** | 96.0% |
| **Precision** | >98% |
| **Recall** | >95% |
| **AUC-ROC** | 0.99 |

---

## 📂 Repository Structure

```text
├── app/
│   ├── models/          # Pre-trained models and encoders
│   ├── static/          # Application assets and generated metrics
│   ├── templates/       # UI components for the inference engine
│   └── main.py          # Flask application entry point
├── research/            # Jupyter notebooks and EDA artifacts
├── LICENSE              # MIT License
├── requirements.txt     # Production dependencies
└── README.md            # Technical documentation
```

---

## 🔧 Installation & Setup

1. **Clone the Repository**
   ```bash
   git clone https://github.com/PRAVEENK44/Credit-Card-Fraud-Detection-System.git
   cd Credit-Card-Fraud-Detection-System
   ```

2. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run Monitoring Dashboard**
   ```bash
   python app/main.py
   ```
   Access the interface at `http://127.0.0.1:5000`.

---

## ⚖️ License

Distributed under the MIT License. See `LICENSE` for more information.
