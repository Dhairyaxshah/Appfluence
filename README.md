# 📱 App Market Analysis & Popularity Prediction  
### Supervised & Unsupervised Machine Learning on App Store and Google Play Data

---

## 📌 Project Overview

This project applies data science and machine learning techniques to analyze mobile app marketplaces and uncover patterns related to **app popularity, market structure, and competitive positioning**.

Using real-world datasets from the **Apple App Store** and **Google Play Store**, the project combines:

- Exploratory Data Analysis (EDA)
- Supervised Machine Learning for popularity prediction
- Unsupervised Machine Learning for market segmentation

The objective is not only to predict app success, but also to understand **what types of apps exist in the market**, how they differ, and how developers can strategically position new apps.

---

## 🎯 Project Objectives

- Analyze app characteristics such as price, size, ratings, reviews, and categories
- Predict app popularity using supervised learning models
- Discover natural market segments using unsupervised clustering
- Compare app market structures across iOS and Android platforms
- Translate machine learning outputs into actionable business insights

---

## 🗂️ Datasets Used

- **Google Play Store Apps Dataset**
- **Apple App Store Apps Dataset**

Both datasets were cleaned and preprocessed to handle missing values, remove inconsistencies, and standardize features prior to analysis.

---

## 🧪 Methodology

### 1️⃣ Exploratory Data Analysis (EDA)

EDA was conducted in a separate notebook to understand:
- Category and genre distributions
- Free vs paid app dynamics
- Install and engagement patterns
- Relationships between price, size, ratings, and popularity
- Structural differences between App Store and Google Play

Insights from EDA directly informed feature selection and modeling decisions.

---

### 2️⃣ Supervised Machine Learning – Popularity Prediction

**Problem Framing**
- App popularity metrics (installs and rating counts) are highly skewed
- Regression was avoided in favor of classification

**Targets**
- Apps were categorized into **Low**, **Medium**, and **High** popularity classes

**Models Used**
- Logistic Regression (baseline)
- Random Forest Classifier (final model)

**Evaluation Metrics**
- Accuracy
- Precision, Recall, F1-score
- ROC-AUC (multi-class)
- Cross-validation (F1 macro)

Random Forest significantly outperformed Logistic Regression across all metrics on both platforms.

---

### 3️⃣ Unsupervised Machine Learning – Market Segmentation

**Approach**
- KMeans clustering applied to engineered feature space
- Elbow Method and Silhouette Score used to select optimal number of clusters (k = 4)

**Key Steps**
- Feature scaling and encoding
- Cluster assignment and validation
- PCA used for 2D visualization of clusters
- Clusters interpreted and labeled based on real-world characteristics

**Identified App Store Segments**
- Mainstream Free Apps
- Low Engagement / Niche Apps
- Premium & Specialized Apps
- High-Engagement Flagship Apps

---

### 4️⃣ Cross-Platform Validation

The unsupervised clustering framework was replicated on the **Google Play Store** dataset to assess generalizability.

Despite platform-specific differences, similar market structures emerged across both ecosystems, confirming the robustness of the approach.

---

## 📊 Key Insights

- Free, mainstream apps dominate both marketplaces by volume
- High-engagement flagship apps are rare but highly influential
- Premium apps focus on depth and functionality rather than scale
- Language support and accessibility correlate strongly with engagement
- Market segmentation provides context that pure popularity prediction cannot

---

## 🧠 Why This Project Matters

This project demonstrates how combining **supervised and unsupervised learning** provides both:
- Predictive power (what will be popular)
- Structural understanding (what types of apps exist)

Such insights are valuable for:
- App developers
- Product managers
- Startups and market analysts
- Data-driven decision making in digital platforms

---

## 🛠️ Tools & Technologies

- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Google Colab / Jupyter Notebook

---

## 🚀 Future Improvements (Optional)

- Category-specific clustering
- Time-based trend analysis
- Alternative clustering algorithms (e.g., DBSCAN)
- Interactive dashboards for exploration

---

## 👤 Authors

This project was completed as a collaborative group effort, with contributions across:
- Data cleaning and EDA
- Supervised learning
- Unsupervised learning
- Cross-platform analysis and interpretation

---

## 📎 Note

This repository focuses on **analysis and insights**, not deployment.  
The notebooks are structured to tell a complete, end-to-end data science story.
