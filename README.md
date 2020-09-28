# Feature_Selection
Feature selection is one of the vital concepts in machine learning which hugely impacts the performance of the model.
It is a process to automatically or manually select those features that have a major contribution to the prediction. It
is not necessary that more data would result in highly good predictions, sometimes irrelevant and redundant features
can make the learning process more complex and may result in overfitting.
Feature selection is important for a few reasons.
• Enhance the generalization capability of the model by reducing overfitting.
• Drastically reduces the training time with lesser computation cost.
• Increases model accuracy by making the algorithms simpler.
The first task for any classification and regression problems is to analyze the data. Finding the missing value in
the data is an important aspect of feature cleaning as certain algorithms cannot work when missing values are present
and even if some algorithm can handle the missing data, it may lead to inaccurate conclusions.
There are several methods available for feature selections such as : <br>
Filter Methods - Does not rely on ML algorithms, focuses on quick screening and removal of irrelevant, redundant,
constant, correlated features. Some of the basic filter methods include: <br>
• Variance - Identification of features that shows the constant value for the majority of observations. <br>
• Correlation – Identification of features that are highly correlated to each other by measuring how strongly one
variable depends on the other. <br>
• Analysis Of Variance – These are statistical methods that measures whether the means of two groups are
significantly different from each other when the continuous features are grouped together by the target vector. <br>
• Mutual Information – Measures mutual dependence of two features. It measures how much information the
presence and absence of any features contributes to make the correct predictions. <br>
Wrapper Methods - Wrapper methods use a search strategy to look through the possible subsets of features and
evaluate each subset of features using a Machine Learning algorithm (Random Forest in our case). The most common
search strategy group is Sequential search, including Forward Selection, Backward Elimination, and Exhaustive Search <br>
• Forward Feature Selection - It is an iterative method in which all features are individually evaluated, and then
one is selected that results in the best performance. In the second step, remaining features are evaluated again
and best feature is selected and added to the list, the loop continues by adding one feature at a time in each
iteration. <br>
• Backward Feature Elimination - It starts by fitting the model with all the available features. After that one
feature is removed after each iteration, which produces the least significant feature among the available ones. <br>
• Exhaustive Feature Selection - This method searches across all possible feature combinations. The aim is to find
the best performing feature subset. For each subset, the features are fitted to a machine learning algorithm and
the subset with best score is selected. <br>
Tree-based classifiers such as Random Forests not only performs well in prediction problems
but also provides a way to select features. Random Forest is based on decision trees utilizing the bagging algorithm
and the Ensemble Learning technique. It creates decision trees based on the subset of the data and combines the
output and makes decisions on the majority of votes. For the mentioned dataset, Random Forest could be helpful for
better interpretability of the model and it is validated by Out of bag score which is helpful in getting the validation
accuracy when the dataset is smaller in size.
