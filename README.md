# Online-News-Popularity-Prediction

## Project Overview
• This case is about prediction popularity of an online news, i.e., to predict the popularity based on the number of shares in social networks.  
• There are 61 features in total, where 58 predictive, 2 non-predictive and 1 target/goal features. An important part of this project is to indentify the key features.  

## Description of Project Folders
### 00_data
 - `OnlineNewsPopularity.csv`  
There are 39,644 online news.  
There are 61 features in total, where 58 predictive, 2 non-predictive and 1 target/goal features.  

### 01_target_clustering  
 - `5151 Clustering.ipynb`  
The objective can be fulfilled by a classification-based approach.  
For classification-based approach, the target values need to be converted to different class labels. This is done with the aid of clustering analysis on the target.  

### 02_EDA  
 - `5151 EDA.ipynb`   
This file contains EDA for the distributions of the target and different features.  

### 03_models 
 - `02-01_statistical_features.ipynb`   
This file creates features based on statistical characteristics.

 - `02-02_lda_based_features.ipynb`  
This file creates features based on the most frequent words for each class.

### 03_model  
This folder contains the models for running.
 - `5151 LGBM.ipynb`  
 - `5151 XGB.ipynb`  
 - `5151 Logistic Regression.ipynb`  
LGBM has the best performance.  
Step 1: After initial feature selection (by domain knowledge), the selected features are fed into the model. Bayes Optimization is used for parameters tuning.    
Step 2: Feature importance for the features are obtained and sorted in a decending order.  
Step 3: The features are fed into the model again one by one in the order of feature importance. A feature is kept if the model performance increases, or removed if the model performance drops.  
Step 4: The final selected features are used for the final round of model training, with the hyper-parameters retuned with Bayes Optimization.  

### 04_report
This folder contains the final project presentation slides. 
