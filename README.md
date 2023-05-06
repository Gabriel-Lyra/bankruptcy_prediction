# Taiwanese Bankruptcy Prediction

This was a project based on a [Kaggle Dataset](https://www.kaggle.com/datasets/fedesoriano/company-bankruptcy-prediction) for our class on IF699 at CIn UFPE

Professor: [Hansenclever Basani](https://www.cin.ufpe.br/~hfb/)

Group: [Andre Filho](https://github.com/mrdedede); [Gabriel Lyra](https://github.com/Gabriel-Lyra); [Matheus Belfort](https://github.com/mrbelf)

## Notes for anyone trying to run our code:

For a better visualization and optimization of the code, we do recommend using [Google Colab](https://colab.research.google.com) to load and run it, after loading the repo there, the code should be workable as a normal jupyter notebook

## Rules for the Project
Following the steps needed to achieve the completion of our final project according to the description of this assignment, we would need to follow the following steps:

1. Try different models in order to check the best fitting of them for the prediction
    * XGBoost
    * Linear Regression
    * SVM
    * KNN
    * Random Forest
    * Decision Tree
    * Neural Networks
2. Try different ensembles of different approaches in order to achieve better results:
    * Voting
    * Stacking
    * Bagging
3. Hyperparameter Optimaztion
4. Model Evaluation
    * F1
    * ROC

## Context
For financial institutions, the ability of predicting whether a business would go bankrupt or not is a matter of huge importance, especially due to possible lendings and financings that directly correlate the risk of investing with the interest rate

However, one problem that lots of institutions go through is that the demonstrative dataset of a company usually is way too big for a proper analysis to be run.

Our current dataset has over 6800 entries, each one of them contains a maximum of 95 features and a label column, meaning that processing this dataset is a very computational-demanding task

## Previous results:

Previous approaches generally focused in more exploratory data analysis with a variety of models for oversampling, re-sampling and, some feature selection approaches as well

## Our results:

As long as a conservative client must be interested, this is how far our model goes on...

1. Results
![conservative-results](https://github.com/Gabriel-Lyra/bankruptcy_prediction/blob/main/conservative-res.png)

2. ROC Curve
![conservative-roc](https://github.com/Gabriel-Lyra/bankruptcy_prediction/blob/main/conservative-roc.png)

Our results show a good precision and recall of data, when compared our given labels to the ones already present in the dataset.
This means our results is satisfactory for conservative financial institutions that must be willing to give out loans to enterprises

## What else could we do in a next time?

1. Removal of correlated columns in order to avoid weighting the results in any direction
2. Make plots and an exploratory data analysis of the dataset itself, through analysis of distributions and boxplots, for instance
3. Weighting or expanding the dataset in order to get a balanced number of "bankrupted" entries (only ~3% is under this category)
4. Make a smarter use of feature engineering in order to achieve better processing speeds and results
5. After running PCA we should run KNN in order to better classsify each member, this would probably give us a better accuracy
