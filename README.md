🛍️ Mall Visitor Demographics — Customer Segmentation via K-Means Clustering
Data-driven clustering of mall customers to derive actionable marketing and retail strategies.

🧠 Problem Context
Retail businesses often struggle with understanding customer diversity. Without a structured understanding of who visits a mall, efforts in marketing, layout planning, or product stocking may underperform. This project solves that by applying unsupervised machine learning to cluster customers into meaningful segments based on demographic and behavioral features.

🎯 Objectives
Perform Exploratory Data Analysis (EDA) to extract trends and anomalies.

Identify optimal number of clusters using the Elbow Method.

Implement KMeans Clustering to group customers.

Visualize multi-dimensional clusters with enhanced plots.

Provide business-level insights for segmentation-based targeting.

📂 Repository Structure
bash
Copy
Edit
Mall-Visitor-Demographics/
│
├── data/
│   └── Mall_Customers.csv             # Dataset
│
├── notebooks/
│   └── segmentation-analysis.ipynb    # Main analysis notebook
│
├── visuals/
│   ├── elbow_plot.png                 # Elbow method visualization
│   └── clusters_2d.png                # Final clustered output
│
├── README.md                          # Documentation (You're here!)
└── requirements.txt                   # Python dependencies
📈 Dataset Overview
📁 Source: Kaggle - Mall Customer Segmentation

📊 Size: 200 rows × 5 columns

Column Name	Description
CustomerID	Unique customer identifier
Gender	Customer gender (Male/Female)
Age	Age in years
Annual Income (k$)	Annual income in thousands USD
Spending Score	Scaled score (1–100) based on customer behavior

⚙️ Technologies & Libraries
Domain	Tools / Libraries
Programming	Python 3.10
Data Handling	pandas, numpy
Visualization	matplotlib, seaborn
ML & Clustering	scikit-learn (KMeans)
Environment	Jupyter Notebook / Google Colab

🔍 Methodology
Data Cleaning & Preprocessing

Check for nulls, outliers, incorrect data types.

Label encoding for categorical columns (e.g., Gender).

Exploratory Data Analysis (EDA)

Distribution plots for Age, Income, and Spending Score.

Heatmaps and pairplots to understand feature relationships.

Cluster Detection

Elbow method applied to range of cluster values (k = 1–10).

Chose optimal k = 5 based on WCSS (Within Cluster Sum of Squares).

KMeans Clustering

Standardized relevant features: Age, Income, Spending Score.

KMeans model fitted to find clusters.

Assigned cluster labels to each row.

Visualization

2D scatter plots with hue = cluster label.

Visual interpretation of customer groups.

📊 Visual Examples
Elbow Plot (to choose optimal k)	Final Customer Segments (2D Projection)

🧠 Insights
Cluster #	Description	Business Strategy Suggestion
0	Young, low income, low spenders	Promote offers; entry-level campaigns
1	High income, low spenders	Loyalty programs, experience enhancements
2	High income, high spenders	Premium brand targeting
3	Low income, high spenders (impulsive)	Flash sales, gamified experiences
4	Average profile	Monitor for behavior change & promotions

📈 Business Impact
By segmenting the customer base, mall management can:

Optimize ad campaigns based on demographic clusters.

Allocate shop space based on demand segments.

Increase customer lifetime value via tailored engagement.

Enhance customer satisfaction with personalized experiences.

🚀 Running the Project
1️⃣ Clone Repository
bash
Copy
Edit
git clone https://github.com/jyothir-369/Mall-Visitor-Demographics.git
cd Mall-Visitor-Demographics
2️⃣ Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
3️⃣ Launch Notebook
bash
Copy
Edit
jupyter notebook notebooks/segmentation-analysis.ipynb
🛠️ Future Enhancements
⏳ Add Time Series: Track visitor changes over months.

🧾 Incorporate Purchases: Merge with sales data for richer analysis.

🤖 Try Alternative Algorithms: DBSCAN, GMM, Hierarchical Clustering.

🖼️ Deploy as Dashboard: Use Streamlit or Dash for real-time clustering.

🧑‍💻 Author
Jyothir Raghavalu Bhogi
🎓 CSE | AIML Enthusiast | Data & ML Projects
🔗 GitHub • LinkedIn • 📬 jyothirraghavalu@gmail.com
