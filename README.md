# ASU_DABC_HW21
deep-learning-challenge
Step 4: Write a Report on the Neural Network Model
For this part of the assignment, you’ll write a report on the performance of the deep learning model you created for Alphabet Soup.
The report should contain the following:
1.	Overview of the analysis: Explain the purpose of this analysis.
Using the features in the provided dataset implement machine learning and neural networks a binary classifier model that can predict whether applicants will be successful if funded by Alphabet Soup 

2.	Results: Using bulleted lists and images to support your answers, address the following questions:
•	Data Preprocessing
o	What variable(s) are the target(s) for your model?
The target variable for my model is IS_SUCCESSFUL column which indicates if the money was used effectively
o	What variable(s) are the features for your model?
The features variable for my model are APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT.
o	What variable(s) should be removed from the input data because they are neither targets nor features?
•	The variables that should be removed from the input data because they are neither targets nor features are EIN and NAME—Identification columns.

•	Compiling, Training, and Evaluating the Model
o	How many neurons, layers, and activation functions did you select for your neural network model, and why?
I used model tune up function to find top 3 models with best model hyperparameters. Used second best model hyperparameters for my final model. It suggested to use 5 layers and tanh activation function instead of relu.
o	Were you able to achieve the target model performance?
No, I wasn’t able to achieve the target model performance of 75% of better of accuracy. 
o	What steps did you take in your attempts to increase model performance?
o	Dropped columns based on Decision Tree for feature importances evaluation. To reduce the noise in the system used 6 columns instead of 43. 
o	Created more bins for rare occurrences in INCOME_AMT column
o	Used model tune up function to optimize: 
	Number of neurons in hidden layer
	Number of hidden layers
	Activation functions for the hidden layers.
o	Added the number of epochs to the training regimen.
3.	Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.
In summary, a target predictive accuracy higher than 75% was not achieved for this machine learning and neural networks a binary classifier model. For future work, I would recommend to take a close look at ASK_AMT column. This is the only numerical variable. Need to find and remove outliers or use a different scaler that is better than the Standard scaler for data with outliers and then redo all the steps above to tune in the model for a target predictive accuracy higher than 75%. 
