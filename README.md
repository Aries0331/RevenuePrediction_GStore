# Kaggle Competition: Google Analytics Customer Revenue Prediction

## Background
The 80/20 rule has proven true for many businesses–only a small percentage of customers produce most of the revenue. 
As such, marketing teams are challenged to make appropriate investments in promotional strategies.

## Methodology
* Data: 1 million user transaction data from Google Store with 53 features
* Identify the 80/20 rule by drawing a graph summing up the total transaction for each customer
* Feature Analysis: Visualize the relation between different features and revenue by Matplotlib
  * For example, device type V.S revenue, Date V.S revenue, GEO location V.S revenue
* Data Cleaning
  * For NULL in categorical columns, fill 'unknown'
  * For numerical data, fill NULL with most frequent value
  * For Boolean features, fill NULL with 'False'
  * Convert categorical columns to type 'str' 
  * Convert numerical columns to type 'float' 
* Baseline Model: LightGBM
  * Separate training dataset into training and validation
  * Training until validation scores don't improve for 100 rounds
* Feature Importance:Identify the top features that contribute to the revenue
