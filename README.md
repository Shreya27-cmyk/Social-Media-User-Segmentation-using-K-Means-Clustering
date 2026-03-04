# 📊 Social Media User Segmentation using K-Means Clustering

## 🚀 Project Overview

This project applies **Unsupervised Machine Learning (K-Means Clustering)** to segment social media users based on behavioral metrics such as engagement, activity level, and audience size.

The clustered results are transformed into actionable business insights using an interactive **Power BI dashboard**.

---

## 🎯 Problem Statement

Social media platforms generate massive volumes of user interaction data. However, businesses struggle to identify:

* High-value users
* Influencers
* Passive users
* At-risk users

Without segmentation, marketing strategies become generic and inefficient.

This project solves that problem by grouping users into meaningful behavioral clusters.

---

## 🧠 Machine Learning Approach

### 1️⃣ Data Cleaning

* Removed missing values
* Checked duplicates
* Verified data types

### 2️⃣ Feature Selection

Used behavioral metrics:

* Daily Time Spent
* Posts
* Likes
* Comments
* Followers
* Engagement Score

### 3️⃣ Data Preprocessing

* Applied **StandardScaler**
* Normalized features (important for distance-based clustering)

### 4️⃣ Algorithm Used

* **K-Means Clustering**

### 5️⃣ Optimal Cluster Selection

* Elbow Method
* Silhouette Score

Final clusters selected: **K = 4**

---

## 📌 Identified User Segments

| Cluster          | Description                 |
| ---------------- | --------------------------- |
| Influencers      | High followers & engagement |
| Content Creators | High activity & posting     |
| Silent Browsers  | Moderate usage, low posting |
| Low Active Users | Low engagement & activity   |

---

## 📊 Power BI Dashboard

The clustering results were exported to Power BI and visualized across three analytical pages:

### 🔹 Page 1 – Overview

* Cluster Distribution
* Key KPIs
* Engagement summary

### 🔹 Page 2 – Engagement Analysis

* Time spent comparison
* Posts & comments analysis
* Engagement rate
* Feature correlation
* Cluster comparison matrix

### 🔹 Page 3 – Business Insights

* Revenue potential
* Conversion probability
* Retention risk analysis
* Action plan matrix

---

## 🧮 DAX Measures Used

```DAX
Engagement Rate = 
DIVIDE(
SUM(Likes) + SUM(Comments),
SUM(Followers)
)
```

Other measures:

* Total Likes
* Average Followers
* Conversion Rate
* Risk Classification

---

## 🛠 Tools & Technologies

* Python
* Pandas
* NumPy
* Scikit-Learn
* Matplotlib / Seaborn
* Power BI
* DAX

---

## 📈 Business Impact

✔ Identifies high-value users
✔ Improves targeted marketing
✔ Detects churn risk
✔ Supports data-driven decisions
✔ Converts ML insights into strategy

---

## 🏁 Conclusion

This project demonstrates how unsupervised machine learning can transform raw behavioral data into structured user segments and how those insights can be converted into business intelligence dashboards for decision-making.

---

## 📂 Repository Structure

```
📁 data/
📁 notebooks/
📁 powerbi/
📄 clustering_model.py
📄 dataset.csv
📄 README.md
```

---

