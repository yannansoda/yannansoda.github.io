## Forest cover type

_Comparing classification algorithms and explore hyperparameter tuning_


### Project description

This is a [notebook](https://www.kaggle.com/code/yannansu/forestcovertype-hyperparametertuning) for the [Cat in the Dat](https://www.kaggle.com/competitions/forest-cover-type-prediction) competition on Kaggle.

> Random forests? Cover trees? Not so fast, computer nerds. We're talking about the real thing.
> In this competition you are asked to predict the forest cover type (the predominant kind of tree cover) from strictly cartographic variables (as opposed to remotely sensed data). 

**The objective of this competition is to predict an integer classification for the forest cover type in the test set. 
In this project, I will first explore the variables and then compare different classification models. Hyperparameter tuning will be applied to the best model. Finally, the model will be applied to the test set.**

### Aim & Methods
I started with a couple of questions:
1. What are the features in the dataset? What are their data types? Are there any missing values?
2. How is the classification problem like? The target features belong to binary or multiple classes?
3. What are the model options? How to evaluate their performances?
4. Which model performs the best? 
5. How to obtain optimal parameters with hyperparamter tuning? 

Therefore, the analysis includes the following parts:
1. Exploratory data analysis
2. Data preprocessing (feature scaling)
3. Model training and evaluation
4. Hyperparameter tuning
5. Model prediction


### Conclusions & Takeaways

- I tested mutilple calssification models, including:
  - Logistic Regression
  - K-Nearest Neighbors
  - Naive Bayes
  - Decision Trees
  - Random Forest
  - Gradient Boosting 
  - Support Vector Machines

- The best model of the evaluated ones is Random Forest with the parameters that I found using RandomizedSearchCV and GridSearchCV.
- Things to try in the future:
  - other new models?


_For more details see [My Notebook on Kaggle](https://www.kaggle.com/code/yannansu/forestcovertype-hyperparametertuning)._
