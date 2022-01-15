# Project Proposal

Contributors: Cici Du, James Kim, Rohit Rawat, Tianwei Wang

A data analysis project for DSCI 522 (Data Science workflows); a course in the Master of Data Science program at the University of British Columbia.

## Summary

This project aims to predict the default chances of a customer based on the payment history of the customer. The data has been taken from UCI Machine Learning Repository and the link can be found here. The default rate of customers have a direct impact on the financials of a credit card company. It is important to predict and implement processes to attenuate and adopt methods to minimize this rate. By targeting customers who are at the risk of defaulting, the company can plan and mitigate it. The research question which we aim to answer through this analysis is to identify the factors which can predict the default of a customer. The problem statement is as follows:
##### Given characteristics (gender, education, age, marriage) and payment history, is the customer likely to default on his or her credit card payment next month or not? 

## Dataset

The data set used in this project is of cases of customers credit card default payments in Taiwan sourced by I-Cheng Yeh at the Department of Information Management, Chung Hua University, Taiwan. It was downloaded from the UCI Machine Learning Repository (Dua and Graff 2019) and can be found [here](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients). Each row in the data set represents variables associated with a customer and his or her credit card information, including a boolean value of default. There are 30,000 observations in the data set and 23 features. There are no observations with missing values in the data set.

## Process

We will begin with doing basic exploratory data analysis on our training dataset, identifying the type of columns, searching for missing values, scaling some of the features and converting categorical variables into relevant features. The possible supervised techniques we could put to use can be DecisionTree, Logistic Regression and SVC since we are doing a classification problem. We will check the coefficients of our components if we use Logistic Regression or draw a truncated tree if we use DecisionTree.

After chosing our final model, we will re-fit the model on the entire training data set after preprocessing, and then evaulate it’s performance on the test data set. At this point we will look at overall accuracy as well as misclassification errors (from the confusion matrix) to assess prediction performance. These values will be reported as a table in the final report.”


## Usage
```
python src/download_data.py --url=https://archive.ics.uci.edu/ml/machine-learning-databases/00350/default%20of%20credit%20card%20clients.xls --out_file=data/data.csv
```

## Dependencies
This list will continue to be modified during the project. 
- Python 3.7.3 and Python packages:
- docopt==0.6.2
- requests==2.22.0
- pandas==0.24.2

## License
The Credit Card Default Prediction materials here are licensed under the Creative Commons Attribution 2.5 Canada License (CC BY 2.5 CA). If re-using/re-mixing please provide attribution and link to this webpage.


## References
 
1. “Yeh, I. C., & Lien, C. H. (2009). The comparisons of data mining techniques for the predictive accuracy of probability of default of credit card clients. Expert Systems with Applications, 36(2), 2473-2480.” 
2. The dataset can be found [here.](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients)

Changed
