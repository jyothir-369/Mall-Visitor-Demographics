# 🛍️ Mall Visitor Demographics — Customer Segmentation via K-Means Clustering

A data-driven clustering project that segments mall customers using **unsupervised machine learning** to uncover actionable insights for marketing and retail strategy.

---

## 🧠 Problem Context

Retail businesses often struggle to understand the diversity of their customer base. Without structured segmentation, marketing efforts, layout planning, and inventory decisions may miss the mark. This project applies **K-Means Clustering** to group mall visitors based on demographic and behavioral features.

---

## 🎯 Objectives

- 📊 Perform **Exploratory Data Analysis (EDA)** to uncover trends and anomalies
- 📐 Identify optimal number of clusters using the **Elbow Method**
- 🔀 Implement **KMeans Clustering** to segment customers
- 🎨 Visualize clusters with enhanced plots
- 💡 Provide business-level insights for targeted strategies

---

## 📂 Repository Structure

Mall-Visitor-Demographics/ ├── data/ │ └── Mall_Customers.csv # Dataset ├── notebooks/ │ └── segmentation-analysis.ipynb # Main analysis notebook ├── visuals/ │ ├── elbow_plot.png # Elbow method visualization │ └── clusters_2d.png # Final clustered output ├── requirements.txt # Python dependencies └── README.md # Project documentation


---

## 📈 Dataset Overview

- **Source**: [Kaggle - Mall Customer Segmentation](https://www.kaggle.com/datasets)
- **Size**: 200 rows × 5 columns

| Column Name           | Description                                      |
|-----------------------|--------------------------------------------------|
| `CustomerID`          | Unique customer identifier                       |
| `Gender`              | Customer gender (Male/Female)                    |
| `Age`                 | Age in years                                     |
| `Annual Income (k$)`  | Annual income in thousands USD                   |
| `Spending Score`      | Scaled score (1–100) based on customer behavior  |

---

## ⚙️ Technologies & Libraries

| Domain         | Tools / Libraries                     |
|----------------|----------------------------------------|
| Programming    | Python 3.10                            |
| Data Handling  | pandas, numpy                          |
| Visualization  | matplotlib, seaborn                    |
| ML & Clustering| scikit-learn (KMeans)                  |
| Environment    | Jupyter Notebook / Google Colab        |

---

## 🔍 Methodology

### 🧼 Data Preprocessing
- Checked for nulls, outliers, and incorrect data types
- Label encoding for categorical columns (e.g., Gender)

### 📊 Exploratory Data Analysis
- Distribution plots for Age, Income, and Spending Score
- Heatmaps and pairplots to explore feature relationships

### 📐 Cluster Detection
- Applied Elbow Method (k = 1–10)
- Chose optimal `k = 5` based on WCSS

### 🔀 KMeans Clustering
- Standardized features: Age, Income, Spending Score
- Fitted KMeans model and assigned cluster labels

### 🎨 Visualization
- 2D scatter plots with cluster labels
- Clear visual interpretation of customer segments

---

## 🧠 Insights

| Cluster | Description                          | Strategy Suggestion                        |
|--------|--------------------------------------|--------------------------------------------|
| 0      | Young, low income, low spenders      | Promote offers; entry-level campaigns      |
| 1      | High income, low spenders            | Loyalty programs; experience enhancements  |
| 2      | High income, high spenders           | Premium brand targeting                    |
| 3      | Low income, high spenders (impulsive)| Flash sales; gamified experiences          |
| 4      | Average profile                      | Monitor for behavior change & promotions   |

---

## 📈 Business Impact

- 🎯 Optimize ad campaigns based on demographic clusters
- 🏬 Allocate shop space based on demand segments
- 💰 Increase customer lifetime value via tailored engagement
- 😊 Enhance satisfaction with personalized experiences

---

## 🚀 Running the Project

### 1️⃣ Clone Repository

```bash
git clone https://github.com/jyothir-369/Mall-Visitor-Demographics.git
cd Mall-Visitor-Demographics
2️⃣ Install Dependencies
bash
pip install -r requirements.txt
3️⃣ Launch Notebook
bash
jupyter notebook notebooks/segmentation-analysis.ipynb
🛠️ Future Enhancements
⏳ Add time series analysis to track visitor trends

🧾 Merge with purchase data for richer segmentation

🤖 Try alternative clustering algorithms (DBSCAN, GMM)

🖼️ Deploy as a dashboard using Streamlit or Dash

👨‍💻 Author
Jyothir Raghavalu Bhogi 🎓 CSE | AIML Enthusiast | Data & ML Projects 🔗 GitHub • LinkedIn • 📬 jyothirraghavalu369

🪪 License
MIT License — Free to use, modify, and share with attribution.


---

Would you like me to generate a banner image or badge row (e.g., Python version, last updated, license) to make this even more eye-catching? I can also help you write a LinkedIn post to showcase this project professionally.
