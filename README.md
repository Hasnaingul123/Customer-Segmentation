# Customer-Segmentation
A machine learning project that applies K-Means clustering to segment customers into distinct groups, enabling targeted marketing strategies and data-driven business decisions.

Author: Hasnain Gul
## Project Overview
This project focuses on **Customer Segmentation** using unsupervised machine learning techniques. The main goal is to analyze customer data and segment them into meaningful groups based on behavioral and demographic patterns. These segments allow businesses to design **targeted marketing strategies**, improve **customer retention**, and enhance **business decision-making**.  

The project implements the **K-Means clustering algorithm** to partition the customer base into clusters. Each stage of the data science workflow, from data preprocessing to model persistence, is documented and executed step by step.

---

## Features & Technologies
The following core Python libraries are used in this project, each serving a specific purpose:

- **pandas**: For loading and manipulating structured datasets.  
- **numpy**: For numerical computations and array-based operations.  
- **matplotlib.pyplot**: For data visualization and exploratory analysis.  
- **seaborn**: For advanced visualizations and statistical plotting.  
- **scikit-learn**:
  - `StandardScaler`: For normalizing features to ensure balanced clustering.  
  - `KMeans`: The clustering algorithm used to create customer groups.  
  - `silhouette_score`: For evaluating the quality of clustering.  
- **joblib**: For saving the trained KMeans model to disk for future reuse.

---

## Methodology

### 1. Data Preprocessing
- **Load the dataset** using pandas.  
- Handle **missing values** (e.g., removing or imputing).  
- Select relevant **numerical and categorical features**.  
- Convert categorical data if necessary.  

### 2. Exploratory Data Analysis (EDA)
- Plot **histograms** and **boxplots** to examine feature distributions.  
- Use **scatter plots** and **pair plots** to identify relationships between features.  
- Summarize insights with correlation heatmaps.  

### 3. Feature Scaling
- Apply **StandardScaler** from scikit-learn to normalize numerical features.  
- This ensures that all features contribute equally to distance-based clustering.  

### 4. Model Training (Clustering)
- Use the **KMeans algorithm** to create clusters.  
- Apply the **Elbow Method** to identify the optimal number of clusters by analyzing the inertia score.  
- Validate the result using the **Silhouette Score**, which measures how well customers are assigned to their clusters.  

### 5. Model Evaluation
- Compare cluster results from different values of *k*.  
- Select the best *k* based on the Elbow curve and the highest silhouette score.  
