# 🩺 Diabetes Prediction: Machine Learning & Dimensionality Reduction

Welcome to this comprehensive project focused on predicting diabetes outcomes using supervised machine learning techniques. The analysis is based on a real-world dataset and demonstrates how models like **Support Vector Machines (SVM)** and **Logistic Regression** perform under both standard and dimensionality-reduced conditions.

---

## 📊 Dataset Overview

The dataset used is a classic **diabetes dataset** commonly used for binary classification tasks. Each row represents a patient, and each column captures various medical predictors such as:

- Number of pregnancies
- Glucose concentration
- Blood pressure
- Skin thickness
- Insulin level
- Body mass index (BMI)
- Diabetes pedigree function
- Age

**Target variable**: `Outcome`  
- `0` = Non-diabetic  
- `1` = Diabetic

---

## ⚙️ Project Structure

### 1. **Model Comparison (No Dimensionality Reduction)**  
📄 `diabetes_classification_logreg_svm.ipynb`  
In this notebook:
- Logistic Regression and SVM models are trained and evaluated.
- Performance metrics (accuracy, precision, recall, F1-score) are calculated.
- A comparison is made to understand which model handles the original features better.

### 2. **PCA + Model Evaluation**  
📄 `diabetes_pca_logreg_svm.ipynb`  
In this notebook:
- PCA (Principal Component Analysis) is applied to reduce dimensionality.
- The reduced dataset is used to train both Logistic Regression and SVM again.
- Results are compared with the original feature-based models.

---

## 📈 Key Techniques Used

- **Data preprocessing**: handling missing values, normalization
- **Model training**: Logistic Regression, SVM (with tuning)
- **Dimensionality Reduction**: Principal Component Analysis (PCA)
- **Evaluation metrics**: accuracy, confusion matrix, classification report
- **Visualization**: PCA component plots, model comparisons

---

## ✅ Results Summary

| Approach             | Accuracy | Notes |
|----------------------|----------|-------|
| Logistic Regression (original data) | 80.21% | Baseline performance |
| SVM (original data)                | 77.08% | Compared well depending on kernel |
| Logistic Regression (PCA)         | 72.72% | Faster training, slight drop/improvement in accuracy |
| SVM (PCA)                         | 72.07% | Performance varied, less overfitting in some cases |


---

## 💡 Insights

- PCA helped in reducing overfitting and improving model interpretability.
- SVM showed strong performance, especially with proper kernel selection.
- Logistic Regression remains a solid baseline with interpretable coefficients.

🧠 Future Work
Apply other dimensionality reduction techniques (e.g., t-SNE, LDA)

Explore deep learning models like neural networks

Use model explainability tools (e.g., SHAP, LIME)

🤝 Contributing
Feel free to fork this repo, open issues, or suggest enhancements!

📬 Contact
Created with ❤️ by Gabriel Bastos
📧 [fagvew3@gmail.com]
🔗 [www.linkedin.com/in/gabriel-bastos-9674a0220]
