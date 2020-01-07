# Caravan-Insurance-Policy-Prediction-Machine Learning  
# Problem Statement    
We want you to predict whether a customer is interested in a caravan insurance policy from other data about the
customer. Information about customers consists of 86 variables and includes product usage data and sociodemographic
data derived from zip area codes.  
The training set contains over 5000 descriptions of customers, including the information of whether or not they
have a caravan insurance policy. A test set contains 4000 customers of whom target variable is not shared with
you.  
Our Target/Dependent Variable is V86.
<br/>
<br/>
# Solution-
we have two data sets-  
1)carvan_train.csv(Training Data) 
2)carvan_test.csv(Testing Data)<br/>

# Steps-  
1)Read both train and test data using python pandas library.    
2)Concatenate both train and test data for data preprocessing and data cleaning.    
3)Check for data types and unique values of all the columns.    
4)Columns "V1","V4","V5","V6","V10","V42","V44" are categorical columns.    
5)Plot all the categorical columns using catplot of seaborn library.    
6)Create (n-1) dummies of all the categorical columns.    
7)Check Null values and impute Null values by mean in train data except columns "V86" and column "data".    
8)Data preprocessing is done and now split the data into train and test data.    
9)Again split train data into 80% and 20% using sklearn train test split.    
10)80% data will be used for training and 20% data will be used to check the performance of the model.    
11)Differentiate target variable and predictors in both the data sets.    
12)Build logistics regression model on train data with 10 fold cv using sklearn's GridSearchCV.    
13)Find the best estimator of grid search and fit on train data(x_train,y_train).    
14)Do the prediction on 20% test data and find the maximum KS cutoff for hardclasses(0 or 1).    
15)Build confusion matrix,find accuracy and f-beta score.    
16)Then fit on whole train data and do the prediction on whole test data.    
17)To get better performance use other model like Random Forest.    
18)Build random forest model using sklearn's RandomizedSearchCV with 10 fold CV.    
19)Find the best estimator of RandomizedSearchCV and fit on 80% train data.    
20)Do the prediction on 20% test data.    
21)Then find KS_cutoff,Accuracy,fbeta score,confusion matrix to check our model performance.    
22)Fit on whole train data using best estimator of RandomizedSearchCV.    
23)Do the prediction on whole test data.    
24)Save prediction(hardclasses) in an csv file.    
25)Both the models perform well.  
