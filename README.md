# **Group Project 268701**
## **Artificial Intelligence & Machine Learning 2022 - 2023**

### *Group Members:*
- Davide Beltrame
- Demetrio Francesco Cardile
- Mariasole Mohn

### **Introduction**
We have received bank details and credit-related data from the greatest financial company in the world: 
we need to help develop targeted products for their users by dividing them into 
three credit score brackets: Poor, Standard and Good. 
In the following sections we will explain how we thought of an efficient data-driven solution to tackle this problem.


### **Methods**

Through exploratory data analysis we perform a deep analysis of the dataset, highlighting some interesting features, 
and trying to extrapolate as much information as possible from data.
First of all, we get a general understanding of the dataset using ad hoc pandas methods in order to discover its size,
the type of variables that it contains and the number of null values.
Although it may be conceived as data cleaning, we will handle missing values in exploratory data analysis 
in order to plot data and have a better understanding through visualization. 
The following strategy to handle missing values is adopted: missing values are replaced by the mode, 
both in the case of categorical and numerical data. 
To get a further insight on data, we show the most interesting statistical features for each numerical variable,
Such as mean, standard deviation, quartiles, minimum and maximum;
After an insights on categorical variables, given by bar plots and histograms, we remove outliers and 
eliminate the ID column , useless for statistical purposes (it is used solely to differentiate every data point).

Before any consideration over the methods we are going to use for this classification problem (our classifiers), 
we remark the importance of splitting our data into three different sets:
- Training set: as its name suggests, it is used to train the classifier. It makes up for 75% of the data points.
- Test set. For 25 % of the data points.
- Validation set.

In order to choose our models, we had to make a choice among the classification methods we have studied:
- K-NN
- SVM
- Kernel SVM
- CART
- Random Forests
- ANN
- XGBoost

We excluded Logistic Regression because the default model is limited to binary classification problems. 
By searching on the web, we found out that an option could have been to transform the problem into a 
multiple binary classification problem. 
Nevertheless, we decided not to proceed in this way. Firstly because other more complex models would have 
very likely performed better and secondly because it seemed a process too long and complex.


### **Experimental Design**
After building our models by calling the sklearn functions, we have performed the task of Hyperparameter tuning.
Hyperparameters are the variables that determine the network structure and how the network is trained. 
The process of Hyperparameter tuning has the goal of finding the best settings for the ML algorithm, that is 
the setting of hyperparameters producing highest accuracy and lowest error rate. 
To achieve this task we use the grid search algorithm which involves iterating between the tuning values and 
testing their effects on performance.
The optimisation process is repeated many times until no further improvement occurs.
- Baseline(s): describe the method(s) that you used to compare your work to 
- Evaluation Metrics(s): which ones did you use and why?

### **Results**
- Main finding(s): report your final results and what you might conclude from your work 
- Include at least one placeholder figure and/or table for communicating your findings 
- All the figures containing results should be generated from the code.

### **Conclusions**
- Summarize in one paragraph the take-away point from your work.
- Include one paragraph to explain what questions may not be fully answered by your work as well as natural next steps for this direction of future work