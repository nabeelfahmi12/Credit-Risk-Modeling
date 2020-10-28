# Objectives: 

#### - To classify which accounts is good or bad for credit risks based on signals from attributes.

#### - Comparing model performance of the following methods:
        - Random Forest
        - Gausian Naive Bayes, and
        - Pipline of the following models:
            - LogisticRegression
            - LinearDiscriminantAnalysis
            - KNeighborsClassifier
            - DecisionTreeClassifier
            - GaussianNB
            - RandomForestClassifier
            - Support Vector Mechnism
            - Gradient Boost Classifier (XGBoost)
## Steps of the Modeling Approach

1. Import Libraries and Dataset
2. Exploratory Data Analysis and Feature Engineering
3. Correlation Analysis
4. Data Preprocessing and Setting the Machine Learning Environment
5. Modeling and Assessing Model Performances

    5.1 Model 1: Using Random Forest to predict credit score
    
    5.2 Setting the Hyperparameters and Creating the Classifier

    5.3 Printing the Model Output

    5.4 Refitting the Model with the best Model Parameters

    5.5 Testing the Model (predicting using the best refit model)

    5.6 Model 2 (Gaussian Naive Bayes)

    5.7 Predicting Probability and the ROC Curve

    5.8 Pipeline of Models

    5.9 Implementing Pipeline of Models

    - Setting the Hyperparameters
    - Creating the classifier (Grid Searching)
## Attributes:

1. Age (numeric)

2. Sex (text: male, female)

3. Job (numeric: 0 - unskilled and non-resident, 1 - unskilled and resident, 2 - skilled, 3 - highly skilled)

4. Housing (text: own, rent, or free)

4. Saving accounts (text - little, moderate, quite rich, rich)

6. Checking account (numeric, in DM - Deutsch Mark)

7. Credit amount (numeric, in DM)

8. Duration (numeric, in month)

9. Purpose (text: car, furniture/equipment, radio/TV, domestic appliances, repairs, education, business, vacation/others)

10. Risk (Value target - Good or Bad Risk)


### The Results: 
    
LR: 0.387574 (0.077970)

LDA: 0.428815 (0.093162)

KNN: 0.263130 (0.035560)

CART: 0.522094 (0.092761)

NB: 0.596300 (0.081365)

*************************
RF: 0.326068 (0.120938)

SVM: 0.182230 (0.088462)

XGB: 0.422917 (0.110550)
    
***********************
All of the models show low Recall:

- The best results are from CART, NB and XGBoost.

# Conclusion:

### Based on accuracy ratio, the performance of the approaches are ranked:
    
    -1st: Pipeline Method
    -2nd: Decision Trees
    -3rd: Gaussian Naive Bayes
