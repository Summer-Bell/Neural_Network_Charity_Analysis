# Neural Network Charity Analysis

## Neural Network Charity Analysis
By using machine learning and neural networks I created a model that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.
With over 34,000 organizations the dataset needed to use a binary classifier.

### Purpose
First the data from [charity_data.csv](Resources/charity_data.csv) needed to be preprocessed so that it could be used in a neural network model.
Next the deep learning model was designed.
The code for this binary classification model is in [AlphabetSoupCharity.ipynb](AlphabetSoupCharity.ipynb).
The next step involved compiling, training and evaluating the model.
Finally the model was optimized with the goal of reaching 75% accuracy.
My three attempts to optimize data are in [AlphabetSoupCharity_Optimization.ipynb](AlphabetSoupCharity_Optimization.ipynb).


## Results
-  Data Preprocessing
	- What variable(s) are considered the target(s) for your model?
		- The IS_SUCCESSFUL column.
	
	- What variable(s) are considered to be the features for your model?
		- Every column except the IS_SUCCESSFUL column.
	
	- What variable(s) are neither targets nor features, and should be removed from the input data?
		- Both the EIN, ORGANIZATION and NAME columns were dropped because they were noisy variables.
		
-  Compiling, Training, and Evaluating the Model
	- How many neurons, layers, and activation functions did you select for your neural network model, and why?
		- My original model contained two layers with the activation function relu. 
		- The first layer had 80 neurons and the second layer had 30 neurons.
		- My output layer was sigmoid.
		- I choose the sigmoid function because it is effectively a logistic regression model.
	
	- Were you able to achieve the target model performance?
	 	- No my model did not achieve target performance.

	- What steps did you take to try and increase model performance?
	 	- I removed a noisy variable ORGANIZATION.
	 	- I added additional neurons and hidden layers.
	 	- I changed the activation function in both the hidden layers and output layers.
	
## Neural Network Charity Analysis Summary
Creating successful deep learning models does take trail and error.
The changes I made to my model did not increase the accuracy of the model.
My original model had the best accuracy score of 70%.
I would remove more noisy variables and continue to adjust the number of neurons in the two hidden layer without changing the activation functions to improve accuracy.
In addition I would increase the number of EPOCH's.




