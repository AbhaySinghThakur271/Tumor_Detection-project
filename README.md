# Tumor_Detection-project
 Tumor Detection Data Analysis
This project focuses on analyzing a dataset related to tumor characteristics to explore correlations and distribution of features relevant to tumor diagnosis (benign or malignant). The dataset is processed using Python libraries such as pandas, NumPy, Seaborn, and Matplotlib.

 Dataset Overview
File: Tumor_Detection.csv

Total Records: 569

Total Features: 32 (1 target column diagnosis, 30 numerical features, and 1 ID column)

 Target Variable
diagnosis:

M = Malignant

B = Benign

 Features Grouped by Type
Feature Group	Description
features_mean	Mean values of tumor characteristics (e.g., radius_mean, texture_mean, etc.)
features_se	Standard error of the features
features_worst	Worst (largest) values recorded for the features

 Libraries Used python

import numpy as np
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

 Data Preprocessing
Dropped the id column (non-informative for modeling)

Grouped features into:

features_mean

features_se

features_worst

Checked for null values and ensured data consistency

 Visualizations
Countplot of diagnosis to view class distribution

Correlation matrix to understand relationships among features

Summary statistics using df.describe()

 Key Insights
Features like radius_mean, perimeter_mean, and area_mean show strong correlations with diagnosis

Many features are highly correlated with each other, suggesting redundancy

Malignant tumors are often associated with higher mean and worst values of several features

 Project Structure

tumor_detection_project/
│
├── Tumor_Detection.csv
├── Tumor_Detection-project.ipynb
└── README.md
