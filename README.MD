# COMPANY BANKRUPTCH PREDICTION

In this project we try predict whether a company will go bankruptch or not
we are given data of the financials of the companies

## Apendix

## Part 1 - EDA - Visuals

We Perform EDA on the given data.
Some key visualizations include

1) Count plot to see how many companies have gone bankrupt.
2) See bankruptcy wrt Liability-asset flag 
( 1 - goes bankruptcy 0 - doesnt go bankruptcy)
3) Countplot of bankruptcy wrt Net Income flag = 1
4) Correlation plot
5) Finding features which are positively correlated and negatively correlated with target(bankruptcy)
6) Plot Bar graph of corellation of top 6 positive and negative featues with bankruptcy 0 or 1 ?
7) Heatmap of correlation withing positively and negatiely correlated attributes

### Summary of EDA
-Companies which posses many asset and asset more tha liabibilies and shareholders equity have less chances of going bankrupt

- An organization cannot guarantee not being bankrupt, although owning several assets.

- The organizations in the dataset are running into losses for the past two years as their net income poses to be negative.

-Companies whose net ioncome decreases or becomes negative ie less income and more expenditure have higer chance of bankruptcy.

- The Top features in predicting bankruptcy are :
    'Roa(C) Before Interest And Depreciation Before Interest', 
    'Roa(A) Before Interest And % After Tax',
    'Roa(B) Before Interest And Depreciation After Tax',
    'Pre-Tax Net Interest Rate', 
    'After-Tax Net Interest Rate',
    'Non-Industry Income And Expenditure/Revenue',
    'Continuous Interest Rate (After Tax)',
    'Net Value Per Share (B)',
    'Net Value Per Share (A)', 'Net Value Per Share (C)',
    'Persistent Eps In The Last Four Seasons', 
    'Cash Flow Per Share'.

- It is observed that “Debt Ratio %, Current Liability To Assets, Current Liability To Current Assets" attributes are a few of the attributes that have a high correlation with the target attribute.

- An increase in the values of the attributes “Debt Ratio %, Current Liability To Assets, Current Liability To Current Assets” causes an organization to suffer heavy losses, thus resulting in bankruptcy.

- An increase in the values of the attributes that have a negative correlation with the target attribute helps an organization avoid bankruptcy.

- There seems to be a relation between attributes that have a high correlation with the target attribute and a low correlation with the target attribute.

- We observed several correlations among the top 12 attributes, one of which being “Net Worth/Assets and Debt Ratio %” that is negatively correlated with one another.


## Part 2 - Data Sampling 
    - Since aur dataset is unbalanced we use SMOTE for oversampling
    - Train Test Split
    - Feature Selection using Mutual Interest

## Part 3 Model Building

### Models used
We build different model 
( Logistic Regression , SVM , 
K-Nearest Neighbour , Decision Tree , Random Forest , XGBoost )
and compare their accuracy.

|      Model             |  Accuracy |
|________________________|___________|
|  Logistic Regression   |  91.1 %   |
|  SVM                   |  91.4 %   |
|  K-Nearest Neighbour   |  94.2 %   |
|  Decision Tree         |  95.6 %   |
|  Random Forest         |  97.2 %   |
|  XGboost               |  98.4 %   |
