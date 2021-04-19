# Kaggle-Toxicity-Prediction

## FOLLOWING STEPS WERE DONE
## THIS IS A  BINARY CLASSIFICATION PROBLEM

#### DIFFERENT MODELS SUCH AS LOGISTIC REGRESSION, DECISION TREE CLASSIFIER, BAGGING CLASSIFIER, VOTING AND STACKING CLASSIFIER, XGBOOST CLASSIFIER AND GARDIENT BOOSTING CLASSIFIER WAS APPLIED.

### STEP 1: DATA PREPARATION
> Reading train.csv and feamat.csv using the pandas dataframe and preparing a whole together bigger dataset using the left join using the chemical id. After merging both train and feamat, we get a combined dataframe which has (77413, 1077) shape meaning that there are 77413 rows and 1077 columns.


### STEP 2: DATA PREPROCESSING
> Dealing with INF values: For this we replaced inf values with nan values.
> Dealing with NAN values: For this, we use two different ways. First, nan values are filled with 0 using fillna(0) function. Secondly, sklearn's SimpleImputer class is used to fill nan values with mean value.
> Class Distribution: Class distribution was checked and it was seen that this is a class of unbalanced dataset and to make the dataset balanaced, sklearn's SMOTE and RandomUnderSampler was used.
> Encoding Object Datatype: V1 column was of object datatype and the values were encoded using LabelEncoder() from sklearn.
> Internal 80-20 split: Using train_test_split from sklearn library, the dataset was split into 80-20 ratio where 80% of the samples belonged to the training data and 20% of the samples belonged to the testing data.
> Normalization: Feature normalization was done using StandardScaler() from sklearn library.
 
 
### STEP 3: MODEL TRAINING
1. K Fold cross validation was used.
2. Grid search CV was used for hyperparameter tuning
3. Cross val score was calculated
4. F1_macro score was obtained both on the training and testing data
5. For Feature Selection, model’s inbuilt feature importances, recursive feature elimination and ANOVA were used.



README file

Requirements for running the code –
System requirements: Windows10
                     Kaggle or Google Collaboratory 
                     RAM: 8GB 
                  
Libraries –
1) Numpy - 1.19.5
2) Pandas - 1.2.1
3) ScikitLearn - 0.24.1

In this we have run code on KAGGLE, to which you require only Kaggle account approved by proffesor. However, in order to run the code on other platforms like Jupyter Notebook and others you need to : 
To run the code, open ‘ML_project’ in Jupyter Notebook
To open Jupyter Notebook on your system, please follow these steps –
1) Open Command Prompt/Terminal on your system
2) Type ‘jupyter notebook’
3) Press Enter
4) Jupyter notebook will open in your browser
5) Upload the file – ‘ML_project’
6) Access the notebook and it opens in a new tab
