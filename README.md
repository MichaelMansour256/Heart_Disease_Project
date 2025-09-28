# 🫀 Heart Disease Prediction Project

This project applies **machine learning** techniques to predict the likelihood of heart disease using patient health data. It explores **data preprocessing, feature engineering, dimensionality reduction (PCA), clustering, classification, and model optimization** to build an end-to-end predictive pipeline.

---

## 📊 Dataset

The dataset contains **297 rows** and **14 features**, including:

* Demographic features: `age`, `sex`
* Clinical measurements: `trestbps`, `chol`, `thalach`, `oldpeak`
* Categorical features: `cp`, `restecg`, `slope`, `ca`, `thal`
* Target: `0 = No Disease`, `1 = Disease`

---

## ⚙️ Project Workflow

1. **Exploratory Data Analysis (EDA)**

   * Visualizations of target distribution
   * Correlation heatmaps
   * Feature histograms and boxplots

2. **Data Preprocessing**

   * Scaling numerical features with `StandardScaler`
   * Encoding categorical features with `OneHotEncoder`
   * Handling missing values

3. **Dimensionality Reduction**

   * PCA applied to reduce feature space
   * Explained variance plotted to choose best `n_components`

4. **Clustering Analysis**

   * **K-Means** clustering (Elbow Method)
   * **Hierarchical Clustering** with dendrograms
   * Comparison of clusters with actual disease labels

5. **Feature Selection**

   * Random Forest & XGBoost feature importance
   * Recursive Feature Elimination (RFE)
   * Chi-Square tests for categorical relevance

6. **Modeling & Evaluation**

   * Logistic Regression, Random Forest, XGBoost
   * Metrics: Accuracy, Precision, Recall, F1-score
   * ROC & AUC curve analysis

7. **Hyperparameter Tuning**

   * GridSearchCV and RandomizedSearchCV used to optimize models
   * Comparison between baseline and tuned models

8. **Model Saving**

   * Best model saved using `joblib` in `.pkl` format

---

## 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/MichaelMansour256/Heart_Disease_Project.git
cd Heart_Disease_Project
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## 📈 Results

* PCA reduced dimensionality while retaining >90% variance with fewer features.
* XGBoost with hyperparameter tuning achieved the **best performance**.
* Clustering provided insights into patient groups, though less accurate than supervised models.

---

## 📂 Project Structure

```
Heart_Disease_Project/
│── data/                 # Dataset files
│── notebooks/            # Jupyter Notebooks for each stage
│── models/               # Saved trained models (.pkl)
│── requirements.txt      # Dependencies
│── README.md             # Project documentation
```

---

## 🛠️ Technologies Used

* Python 3.x
* Pandas, NumPy, Matplotlib, Seaborn
* Scikit-learn
* XGBoost
* Joblib

---

## 👨‍💻 Author

Developed by **Michael Mansour**
📧 Contact: https://www.linkedin.com/in/michaelmansourghaly/
