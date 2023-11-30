# FraudDetection
Fraud detection using machine learning and deep learning techniques on a card-not-present dataset


The dataset used in this work is IEEE-CIS Fraud Detection, which was made available on Kaggle as a beginning point for use in a competition to design a transaction fraud detection model by the IEEE Computational Intelligence Society (IEEE-CIS) in association with the Vesta company. This dataset includes data on online card-not-present transactions, or transactions that take place over the internet. 

It is divided into two files. Train transaction files contain 394 transaction features, and train identity files have 41 identification features. Based on the transactions' ID, the identification and transaction datasets can be merged to produce a dataset of 590540 transaction records with 434 attributes.

A great many values in the combined dataset are missing. As a result, the majority of the columns in this study have been eliminated based on the number of missing data and domain knowledge. Different methods, such imputation and placements, are used to fill in the remaining missing data. Following simple preprocessing, 48 attributes and 590540 records left in the dataset. The pre-processing steps that were done are described in the files.

After following pre-processing steps and conducting an analysis of the dataset, the original dataset was further narrowed down by using dimension reduction techniques. Correlation map, chi-squared test and feature engineering techniques such as information gain and Random Forest Feature Importance were used to make decisions on selecting features and PCA(Principal Component Analysis) was applied as the dimension reduction technique. 

The dataset which underwent PCA was later used to make sample datasets. Under-sampling was applied to investigate the levels of impact of class imbalance. 3 ratios were used to make 3 sample datasets. 
1. 1 fraud transaction : 9 Normal transactions
2. 1 fraud transaction : 3 Normal transactions
3. 1 fraud transaction : 1 Normal transaction

The under-sampled datasets were exported seperately. 

Below tasks were carried on each dataset seperately.
  Exploratory Data Analysis
  Develop and evaluate Random Forest models
  Develop and evaluate Neural Network models
  Develop GAN models and generate synthetic data
  Test combined dataset of synthetic and original data on a Random Forest Classifier
