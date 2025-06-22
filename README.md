# Dry-Eye-Disease-Prediction-and-Prevention
## Overview
This project aims to develop an intelligent system leveraging machine learning techniques to assess DED risk based on lifestyle patterns. By employing both supervised and unsupervised learning, the system identifies hidden risk factors and provides personalized recommendations for symptom management and early detection.

## Objective
- Develop a machine learning system to assess DED risk based on individual lifestyle factors.
- Identify hidden risk factors and provide personalized recommendations

## Dataset Description
The dataset comprises 20,000(13,037 Yes and 6,963 No) with 26 features, including:

- **Demographics**: Gender, Age, Height, Weight
- **Lifestyle Habits**: Screen time, Sleep quality, Caffeine and alcohol consumption
- **Health Indicators**: Heart rate, Blood pressure, Medical conditions
- **Environmental Factors**: Smart device use before bed, Blue-light filter usage
- **Eye Health Symptoms**: Eye strain, Redness, Irritation
- **Target Variable**: Dry Eye Disease (Yes/No)

## Unsupervised Learning
The unsupervised learning phase consists of two distinct techniques: clustering and autoencoders.

- **Clustering**: Implemented using K-Means, Hierarchical Clustering, DBSCAN, and Gaussian Mixture Models (GMM) to identify lifestyle behaviors linked to eye health. The clustering results were used to add additional features to the dataset, enhancing the model's predictive capability.

- **Autoencoder**: Explored for dimensionality reduction and feature extraction, separate from clustering.


## Supervised Learning
Following the unsupervised phase, three supervised learning models were employed:
- **Logistic Regression**
- **LightGBM**
- **XGBoost**
  
All three models were tuned and trained on the same sample, allowing for a direct comparison of their results in predicting DED. SMOTE was applied to address class imbalance during training.


## Personalized Recommendations
Generated lifestyle profiles for each cluster and provided tailored advice based solely on the clustering results. This approach helps users understand their behaviors and make informed adjustments to their lifestyle to mitigate DED symptoms.
