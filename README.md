#   Bank Card Fraud Detection - Unsupervised Anomaly Detection 

![Myers Briggs Personality Types](images/img1.jpg)

## Project Purpose 

The purpose of this project is to apply various unsupervised anomaly detection techniques to find fraudulent activities in the credit card data. 

## Tools & Modules Used

*   Python3
*   Data Analysis - Pandas | Numpy | Matplotlib | Seaborn
*   Anomaly Detection Techniques - 
    * Isolation Forest
    * Local Outlier Factor
*   Deep Learning Techniques - 
    * AutoEncoder
    * CNN

## Dataset

The datasets contains transactions made by credit cards in September 2013 by european cardholders.

It contains only numerical input variables which are the result of a PCA transformation. Due to confidentiality issues, the original features are converted into PCA features - V1, V2, … V28. The only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-senstive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

## Challenges faced

   The dataset is highly imbalanced with less than 1% of data as fraud transactions. To handle the imbalance issue and for faster execution of the code, a sample of the data was taken (stratified sample). 


## Result

Anomaly detection techniques like Isolation Forest and Local Outlier Factor did not work well on this highly imbalanced dataset. Deep Learning techniques like AutoEncoders with the Logistic Regression Model and a Convolution Neural Network model performed well on this dataset. 