# DATA
https://www.kaggle.com/datasets/arockiaselciaa/creditcardcsv


## Overview


Credit card fraud is any dishonest act and behaviour to obtain information without the proper authorization from the account holder for financial gain. For many banks, retaining high profitable customers is the number one business goal. Banking fraud, however, poses a significant threat to this goal for different banks. In terms of substantial financial losses, trust and credibility, this is a concerning issue to both banks and customers alike.

The data set includes credit card transactions made by European cardholders over a period of two days in September 2013. Out of a total of 2,84,807 transactions, 492 were fraudulent. This data set is highly unbalanced, with the positive class (frauds) accounting for 0.172% of the total transactions. The data set has also been modified with Principal Component Analysis (PCA) to maintain confidentiality. Apart from ‘time’ and ‘amount’, all the other features (V1, V2, V3, up to V28) are the principal components obtained using PCA. The feature 'time' contains the seconds elapsed between the first transaction in the data set and the subsequent transactions. The feature 'amount' is the transaction amount. The feature 'class' represents class labelling, and it takes the value 1 in cases of fraud and 0 in others.


## Methodology

The project pipeline can be briefly summarized in the following steps:

1. Exploratory data analysis

   • Univariate analysis

   • Bivariate analysis

2. Prepare the data for modelling 

   • Check the skewness of the data and mitigate it for fair analysis

   • Handling data imbalance as we see only 0.172% records are the fraud transactions

3. Split the data into train and test set

   • Scale the data (normalization)

4. Model building

   • Train the model with various algorithm such as Logistic regression, Support Vector machine , Decision Tree,K Nearest Neighbour , Random forest, XGBoost etc.
   • improved performance of models using Ensemble Techniques i.e., AdaBoost, Gradient Boosting and RF
   • Tune the hyperparameters with Grid Search Cross Validation and find the optimal values of the hyperparameters

7. Model evaluation 

   • As we see that the data is heavily imbalanced, Accuracy may not be the correct measure for this particular case

   • We have to look for a balance between Precision and Recall over Accuracy

   • We also have to find out the good ROC score with high TPR and low FPR in order to get the lower number of misclassifications
  ## Results
  Obtained highest f1 score of 0.89 and AUC score of 0.91 using random forest with XGBoost technique.
