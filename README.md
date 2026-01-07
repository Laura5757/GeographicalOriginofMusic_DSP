# GeographicalOriginofMusic_DSP
This repository contains the implementation, statistical analysis, and machine learning pipeline for classifying the geographical origin of music based on its audio features.

The dataset used in this project is avaliable in: https://archive.ics.uci.edu/dataset/315/geographical+original+of+music 

## Overview
The project investigates the relationship between musical audio characteristics and their cultural-geographical origins. It compares different feature sets (Default with 68 variable vs. Chromatic with 116 variables) and evaluate various machine learning algorithms to identify the most robust way to discover the musical structure of 33 different countries.

## Key Features
- Dimensionality Reduction: Evaluation of PCA and SVD techniques to compress high-dimensional audio data into 56 principal components while retaining 99% variance.
- Statistical Validation: Hypothesis testing using Kruskal-Wallis, paired t-tests, and Bonferroni corrections to ensure results are not due to chance.
- Comparative Modelling: Head-to-head performance analysis between K-Nearest Neighbors (KNN), Random Forest (RF), and Support Vector Machines (SVM).
- Visual Analysis: Visualisations including t-SNE manifolds, network connectivity graphs of musical proximity, and Silhouette analysis for cluster cohesion.
  
## Main Findings
- Country Prediction: Musical features are highly significant predictors of origin.
- Universal Structures: Musical variability and countries' cohesion are statistically consistent across continents, suggesting a universal music structure.
- Model Robustness: SVM result as the most resilient model, maintaining high accuracy even under significant dimensionality reduction.
- Cohesion: Silhouette analysis (scores between -0.2 and 0.2) suggests that musical borders are fuzzy.

### Language: Python 
Libraries: scikit-learn, pandas, numpy, scipy (statistical tests), matplotlib/seaborn (visualisation), networkx (network graph).

#### Note:
There is no need to download any file apart from the code due to the code obtains the datasets directly from the UCI repository.

