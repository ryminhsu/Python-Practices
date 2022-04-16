The project aims to explore the insightful information in relation to Covid 19 

We conducted different models to answer difrent quitions






**Project (a): Association mining to find hotspots based on a Patient Route Data**

During the initial outbreak of COVID-19 in South Korea, the routes travelled by positive patients were reported. The “PatientRoute” dataset consists of 1509 observations where each observation presents a positive patient’s visit at a location and the time. There is a total of 891 unique patients and 151 unique locations.

Consider each patients’ route as a transaction in the dataset ‘D1.csv’ and build an association mining model on this dataset to identify what are the common routes that positive patients have travelled. The task is to conduct Association mining on this data set.

Answer the following concerning this data and analysis.
1. What variables did you include in the analysis? Justify your choice.
2. Does this dataset require any pre-processing before building the association mining model?
3. Conduct association mining and answer the following:
a. What is the ‘min_support’ threshold set and discuss why it is chosen?
b. Report the top 5 frequently occurring rules and interpret them.
4. Identify at least 10 common routes that positive patients from the Seoul province in the Dongjak-gu city have travelled.
5. Can you perform sequence analysis on this dataset? If yes, present your results. If not, rationalize why?
6. How the outcome of this study can be used by the decision-makers?


Project (b): Clustering mobility data
Tasks
Suppose a city council management team wants to understand people’s mobility for each category of location. Your task is to conduct clustering on this data set and describe the minimum number of effective clusters identified.
Answer the following concerning this data and clustering analysis (add screenshots as appropriate).
1. Identify the data quality problems in this dataset such as unusual data types, missing values, etc, and explain how to fix them?
2. 3. Build a clustering model to profile the category of locations visited by the people. Answer the followings:
a. What clustering algorithm have you used?
b. List the attributes used in this analysis.
c. What is the optimal number of clusters identified? How did you reach this optimal number?
d. Did you normalise the variables? What was its effect on the model – Does the variable normalization process enable a better clustering solution?
3. For the model with the optimal number of clusters,
a. Visualize the clusters using ‘pairplot’ and interpret the visualization.
b. Characterize the nature of each cluster by giving it a descriptive label and a brief description. Hint: use cluster distribution.
4. Build another clustering model using an algorithm that helps to profile the people’s mobility only in the following countries:
• Australia
• United Kingdom
• Japan
• Latvia
• Romania
• Slovenia
• Kenya
Use the best setting (e.g., variable normalisations, optimal K, etc) obtained in the previous model. Answer the followings:
a. What clustering algorithm have you used?
b. List the attributes used in this analysis.
c. What difference do you see in this clustering interpretation when compared to the previous one?


Project (c): Building and Evaluating Predictive models
In Assessment 1, you have explored the data set created by Nexoid3. You are now provided with D3.csv, a processed dataset of D1.csv (as part of Assesssment1). Use this processed data to perform predictive modelling with different methods namely Decision tree, Logistic Regression and Neural networks. This dataset consists of rich geographical, behaviour, segmentation, health conditions, and risk values. The pre-processed data, ready for mining, consists of 5111 observations. The objective is to classify if a patient is covid19_positive (1) or not (0). Use ‘covid19_positive’ as the target variable and the rest of the variables as input variables.

Tasks
Your task is to build various predictive models including decision tree, regression model, and neural network on this data set and compare them.
Answer the followings (add screenshots as appropriate).
Predictive modeling using Decision Tree
1. Build a decision tree using the default setting. Answer the followings:
a. What is the classification accuracy of training and test datasets?
b. What is the size of the tree (number of nodes and rules)?
c. Which variable is used for the first split?
d. What are the 3 important variables in building the tree?
e. What parameters have been used in building the tree? Detail them.

What is the classification accuracy of training and test datasets?
b. What is the size of the tree (i.e. number of nodes and rules)?
c. Which variable is used for the first split?
d. What are the 3 important variables in building the tree?
e. Report if you see any evidence of model overfitting.
3. What is the difference do you see between these two decision tree models (with and without fine tuning)? How do they compare performance-wise? Produce the ROC curve for both DTs. Explain why those changes may have happened.
4. From the better model, can you identify which patients could potentially be "COVID-19 Positive"? Can you provide general characteristics of those patients?
Predictive modeling using Regression
1. Build a regression model using the default regression method with all inputs. Build another model tuned with GridSearchCV. Choose a better model to answer the followings:
a. Explain why did you choose that model?
b. Name the regression function used.
c. Did you apply standardization of variables? Why would you normalise the variables for regression mining?
d. Report on which variables are included in the regression model.
e. Report the top-3 important variables (in the order) in the model.
f. What is classification accuracy on training and test datasets?
g. Report any sign of overfitting in this model.
2. Build another regression model on the reduced variables set. Perform dimensionality reduction with Recursive feature elimination. Tune the model with GridSearchCV to find the best parameter setting. Answer the followings:
a. Was dimensionality reduction useful to identify a good feature set for building the accurate model?
b. What is classification accuracy on training and test datasets?
c. Report any sign of overfitting.
d. Report the top-3 important variables (in the order) in the model.
3. Produce the ROC curve for all different regression models. Using the best regression model, can you identify which patients could potentially be "COVID-19 Positive"? Can you provide general characteristics of those patients?
Predictive modeling using Neural Networks
1. Build a Neural Network model using the default setting. Answer the following:
a. Explain the parameters used in building this model, e.g., network architecture, iterations, activation function, etc.

the training process converge and resulted in the best model?
2. Refine this network by tuning it with GridSearchCV. Report the trained model.
a. Explain the parameters used in building this model, e.g., network architecture, iterations, activation function, etc.
b. What is classification accuracy on training and test datasets?
c. Did the training process converge and resulted in the best model? Do you see any sign of over-fitting?
3. Would feature selection help in improving the model? Build another Neural Network model with reduced features set. Perform dimensionality reduction by selecting variables with the decision tree (use the best decision tree model). Tune the model with GridSearchCV to find the best parameters setting. Answer the followings:
a. Did feature selection favor the outcome? Any change in network architecture? What inputs are being used as the network input?
b. What is classification accuracy on training and test datasets?
c. How many iterations are now needed to train this network?
d. Do you see any sign of over-fitting? Did the training process converge and resulted in the best model?
4. Produce the ROC curve for all different NNs. Using the best neural network model, which patients could potentially be " COVID-19 Positive"? Can you provide general characteristics of those patients? Is it easy to comprehend the performance of a neural network model for decision making?

Final remarks: Decision making
1. Finally, based on all models and analysis, is there a model you will use in decision making? Justify your choice. Draw a ROC chart and Accuracy Table to support your findings.
2. Can you summarise the positives and negatives of each predictive modelling method based on this analysis?
