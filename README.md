# Sensor rankings using Random Forests
A task to rank features according to importance
### Dataset

The file task_data.csv contains an example data set that has been artificially
generated. The set consists of 400 samples where for each sample there are 10
different sensor readings available. The samples have been divided into two
classes where the class label is either 1 or -1. The class labels define to what
particular class a particular sample belongs.

## Reason for selecting Random Forest Classifier

Random Forest algorithm works great with a small dataset. With random forest, you can train a model with a relative small number of samples and get pretty good results. As we have a relatively small dataset of 400 samples Random forest classifier would be a great algorithm.

## Strengths of Random forests
- The algorithm has little or no overfitting. The main reason is that it takes the average of all the predictions, which cancels out the biases.
- Random forest algorithms are usually highly accurate and robust depending on the number of decision trees participating in the process. Which we use 100 (n_estimators)
- Random forest uses gini importance or mean decrease in impurity (MDI) to calculate the importance of each feature. Gini importance is also known as the total decrease in node impurity. This is how much the model fit or accuracy decreases when you drop a variable. The larger the decrease, the more significant the variable is.

## Weakness of Random Forest Algorithm
- The algorithm fails when there are rare outcomes or rare predictors,as the algorithm is based on bootstrap sampling.
- When you have a large collection of decision trees it is hard to have an intuitive grasp of the relationship existing in the input data.

## Scalability of Random Forest with respect to number of features and/or samples

Random Forest has the power to handle a large data set with higher dimensionality


