# Market Prediction Using PyCaret (AutoML) and ExtraTreesClassifier 🚀
This is a challenge published by [Jane Street Group in Kaggle.](https://www.kaggle.com/c/jane-street-market-prediction)
This repository lists the notebooks developed to arrive at a solution that was published in Kaggle: https://www.kaggle.com/jlfdatascience/jane-street-extratreesclassifier-pca-pipeline

**Description**: The supplied dataset contains a set of features, feature_, goes 0 ... 129, representing actual stock market data. Each row in the data set represents a trading opportunity, for which we will be predicting a stock value: 1 to make the trade and 0 to pass it. Each operation has an associated weight and resp, which together represents a return on the trade. In the training set, tren.csv, you are given a resp value, as well as several other resp_ values of 1,2,3,4 that represent returns at different time horizons.


## 1. Aproach by AutoML
Approaching the best model with PyCaret
With this AutoML library we can have a quick approximation to the models that best respond to the data provided.

## 2. Jane Street ExtraTreesClassifier | PCA | Pipeline
We developed a prediction model with **ExtraTreesClassifier()** method.  In this case as the available data are very heavy with almost 2.4 million records, 130 variables and a weight of more than 5 GB, it is proposed to reduce the dimensionality with **PCA (Main Component Analysis) + Cross Validation + Pipeline** (encapsulated in a SKlearn method).
