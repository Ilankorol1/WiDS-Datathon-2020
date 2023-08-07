# WiDS-Datathon-2020

## As part of a course in Data science, we were asked  to partcipate in an old competition in Kaggle.

## Part-1
 Harvard Privacy Lab, has provided a dataset of more than 130,000 hospital Intensive Care Unit (ICU) visits from patients, spanning a one-year timeframe. This data is part of a growing global effort and consortium spanning Argentina, Australia, New Zealand, Sri Lanka, Brazil, and more than 200 hospitals in the United States.

Labeled training data are provided for model development; you will then upload your predictions for unlabeled data to Kaggle and these predictions will be used to determine the results.
## We have reached the results of 0.84 accuracy as can be seen in the report.
We did it with extracting some Preprocessing:
1) Analysis of categorical characteristics.
![image](https://github.com/Ilankorol1/WiDS-Datathon-2020/assets/103121260/92318c8c-8170-43ad-9009-7055d27cc2dd)
2) Checking columns with unique values.
3) Analysis of categorical characteristics with in-hospital death.
![image](https://github.com/Ilankorol1/WiDS-Datathon-2020/assets/103121260/3026324a-1eca-4f14-9fac-a258bede6b3e)
### 4) Dealing with missing values
  We removed all the features that had more than 80% missing valuse.
5) Completing missing values:
  a. For numerical characteristics that are in a normal distribution, we decided to fill in the missing data at the median of the column.
  b. For numerical characteristics that are not normally distributed, we decided to fill the missing data with the mean value of the column. This makes it possible to maintain the         general statistics of the characteristic and not affect the distribution of the characteristic.
  c. For categorical features, we decided to fill the missing data with the most common value in the column. This helps maintain the original category distribution and not affect the   characteristic distribution.
6) Description of normalization/binning/encoding and feature creation operations.
7) Removing features with high correlation.

## Part-2
### Activating a method for selecting relevant characteristics:
We chose to use chi square to select the most significant features for our predictive model. The chi square test is a statistical tool that allows us to examine the dependence between characteristics and our target variable.

### We chose to test 6 models that were of particular interest to us.
First, we used the train_test_split function from the sklearn library to split the data into training and test sets.
Next, we defined six different machine learning models:
1. Gradient Boosting
2. Logistic Regression
3. Decision Tree
4. Random Forrest (ensemble method)
5. Naive Bayes
6. Neural Network

### For the best resulrts we used different weights for each Model:
![image](https://github.com/Ilankorol1/WiDS-Datathon-2020/assets/103121260/0b65c976-1167-4569-9064-c8804e1faf15)
![image](https://github.com/Ilankorol1/WiDS-Datathon-2020/assets/103121260/2b6368a7-c94a-4765-ae29-346ff5830f88)

