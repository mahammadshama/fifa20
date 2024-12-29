# FIFA Player Clustering Project

## Project Overview

This project focuses on analyzing the FIFA 20 dataset to cluster players into meaningful groups using unsupervised learning techniques. The aim is to assist in optimizing team management and strategy by identifying players' strengths, roles, and performance styles.


---

## Dataset Details

**Dataset Size: 18,278 rows and 104 columns**

**Source: FIFA 20 player statistics**

**Key Features: Player attributes such as pace, shooting, dribbling, defending, and physicality**



---

## Business Case

Clustering players into meaningful groups allows for better decision-making in:

Identifying players who excel in specific roles or play styles

Optimizing recruitment and team management strategies



---

## Project Workflow

### 1. Exploratory Data Analysis (EDA)

Tools: Sweetviz for univariate analysis, bivariate analysis

Dropped unnecessary columns like sofifaid, shortname, playerurl, longname, dob.


## Key Insights:

### Task 1: Rank the top 10 countries with the most players.

Top Countries:

England: 1667 players

Germany: 1216 players

Spain: 1035 players



### Task 2: Plot the distribution of overall rating vs age.

Players generally improve until around age 30, after which performance declines.


### Task 3: Offensive player roles vs salaries.

Strikers (ST): Highest-paid offensive players with an average salary of 10,256.49.

Left Wingers (LW): 9,681.81

Right Wingers (RW): 6,208.79



---

## 2. Data Preprocessing

Addressed 244,935 null values in 48 columns:

Dropped columns with 90%+ null values and irrelevant features (e.g., team jersey number, loaned from, nation position).

Imputed missing values:

Mean: contract valid until

Median: release clause error

Zero: Remaining columns


**Converted categorical data into numerical data.**

**Applied StandardScaler for feature scaling.**



---

### 3. Dimensionality Reduction

Principal Component Analysis (PCA):

Reduced features to 22 components to retain 95% variance.




---

## 4. K-Means Clustering

Optimal Clusters: 2 (using Elbow Method)

Silhouette Score: 0.622



---

## Key Findings

**1. Clusters Identified:**

Players were grouped into two distinct clusters based on attributes.

Each cluster represents different performance styles and roles.



**2. Model Performance:**

The silhouette score of 0.62 indicates moderate separation, demonstrating reasonable effectiveness of the clustering model.





---

## Project Conclusion

This project demonstrated the use of unsupervised learning techniques to derive actionable insights from the FIFA 20 dataset. The clustering approach highlighted distinct player attributes, offering potential for data-driven decisions in player recruitment, strategy formulation, and performance analysis.



## Future Work

Explore different clustering techniques (e.g., DBSCAN, Hierarchical Clustering).

Use advanced dimensionality reduction techniques such as t-SNE or UMAP for better visualization.

Integrate player clustering insights with real-world applications like team performance simulations.
