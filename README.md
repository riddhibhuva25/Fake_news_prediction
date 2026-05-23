35

# 🛍️ Customer Segmentation using K-Means Clustering

## 📌 Project Overview

This project focuses on segmenting mall customers into different groups using **K-Means Clustering**, an unsupervised machine learning algorithm.

Customer segmentation helps businesses better understand customer behavior and create targeted marketing strategies.

The model groups customers based on:

* Annual Income
* Spending Score

The project also includes:

* Exploratory Data Analysis (EDA)
* Data Visualization
* Feature Scaling
* Elbow Method
* Silhouette Score Evaluation
* Cluster Visualization
* Customer Segment Prediction Function

---

# 🎯 Objective

The main objectives of this project are:

* Identify distinct customer groups
* Understand customer spending behavior
* Apply unsupervised learning techniques
* Find the optimal number of clusters using the Elbow Method
* Evaluate clustering quality using Silhouette Score
* Build a reusable customer segment prediction function

---

# 🧠 Machine Learning Concepts Used

* Unsupervised Learning
* Clustering
* K-Means Algorithm
* Feature Scaling
* Elbow Method (WCSS/Inertia)
* Silhouette Score
* Customer Profiling

---

# 🛠️ Technologies & Libraries Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn

---

# 📂 Dataset Information

> ⚠️ **Note:** The dataset file is not included directly in this repository due to size optimization. Follow the download link below to add it locally.

The dataset contains mall customer information including:

| Feature                | Description                                  |
| ---------------------- | -------------------------------------------- |
| CustomerID             | Unique customer identifier                   |
| Gender                 | Male/Female                                  |
| Age                    | Customer age                                 |
| Annual Income (k$)     | Annual income in thousand dollars            |
| Spending Score (1-100) | Customer spending score assigned by the mall |

### 📥 Dataset Download Instructions:
1. Download the dataset from Kaggle: [Mall Customers Dataset](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)
2. Extract the file, rename it to `Mall_Customers.csv` if necessary, and place it in the root folder of this project.

---

# 📊 Exploratory Data Analysis (EDA)

Performed several EDA steps including:

* Dataset shape and information
* Missing value checking
* Duplicate row detection
* Distribution analysis
* Gender distribution visualization
* Income vs Spending scatter plots
* Histograms and KDE plots

---

# ⚙️ Data Preprocessing

### Steps performed:

* Removed `CustomerID` column
* Selected important clustering features:

  * Annual Income
  * Spending Score
* Applied `StandardScaler` for feature scaling

Why scaling?
Because K-Means is a distance-based algorithm and scaling ensures all features contribute equally.

---

# 📉 Elbow Method

The Elbow Method was used to determine the optimal number of clusters.

### Observations:

* Sharp decrease in WCSS from K=1 to K=5
* Curve starts flattening after K=5
* Optimal clusters selected: **K = 5**

---

# 🤖 K-Means Clustering

The final clustering model was trained using:

KMeans(n_clusters=5, random_state=42)

The model grouped customers into 5 distinct segments.

---

# 📏 Model Evaluation
### Silhouette Score

Silhouette Score was used to evaluate clustering quality.

A higher silhouette score indicates:

Better cluster separation
Better clustering performance

---
# 📈 Cluster Visualization

The clusters were visualized using scatter plots:

X-axis → Annual Income
Y-axis → Spending Score
Different colors represent different customer segments

This helps understand customer behavior patterns visually.

---

# 👥 Customer Segment Profiling

Cluster-wise analysis was performed using:

Mean values
Median values
Cluster sizes

This helps businesses understand:

High-income high-spending customers
Low-income low-spending customers
Target customer groups

---
# 🔮 New Customer Segment Prediction

A reusable function was created to predict the segment of a new customer.

### Example:
def assign_customer_segment(income_k, spending_score, scaler, model):

This function predicts which cluster a new customer belongs to.

---

# 📌 Project Workflow
Data Collection
       ↓
Exploratory Data Analysis
       ↓
Data Preprocessing
       ↓
Feature Scaling
       ↓
Elbow Method
       ↓
K-Means Clustering
       ↓
Model Evaluation
       ↓
Cluster Visualization
       ↓
Customer Profiling
       ↓
Prediction Function

---
# 🚀 Results
Successfully segmented customers into meaningful groups
Identified customer spending patterns
Achieved good clustering separation using K-Means
Built a practical clustering workflow for business analytics

---
# 📷 Sample Visualizations

The project includes:

Histograms
Count plots
Scatter plots
Elbow curve
Silhouette score visualization
Cluster plots

---
# 💡 Real-World Applications

Customer segmentation is widely used in:

Targeted Marketing
Personalized Recommendations
Customer Retention
Business Strategy
Product Marketing
Retail Analytics

---

# ▶️ How to Run the Project
### 1. Clone Repository
git clone https://github.com/riddhibhuva25/Customer_segmentation_clustering
### 2. Install Dependencies
pip install -r requirements.txt
### 3. Run Jupyter Notebook
jupyter notebook

---
# 📚 Key Learnings

Through this project, I learned:

* How K-Means clustering works
* Importance of feature scaling
* How to select optimal clusters
* How to evaluate clustering models
* Customer behavior analysis
* Data visualization techniques

  ---
# 🙋‍♀️ Author

Riddhi Patel

Machine Learning Enthusiast | Data Science Learner

GitHub: https://github.com/
LinkedIn: https://linkedin.com/
# ⭐ If you found this project useful, give it a star!
