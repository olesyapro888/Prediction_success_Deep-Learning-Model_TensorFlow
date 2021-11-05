# Neural Network Charity Analysis. Project 19 of the UofT.
## `-Contents-`	
	
- [Overview of the Neural Network Charity Analysis](#Overview-of-the-Neural-Network-Charity-Analysis)	
- [Resources](#resources)	
- [The Neural Network Charity Analysis Result](#The-Neural-Network-Charity-Analysis-Result)
  - [Preprocessing Data for the Neural Network Model](#--Preprocessing-Data-for-the-Neural-Network-Model)
  - [Compile, Train, and Evaluate the Model](#--Compile-,-Train-,-and-Evaluate-the-Model)
  - [Optimize the Model](#--Optimize-the-Model)
- [The Neural Network Charity Analysis Summary](#The-Neural-Network-Charity-Analysis-Summary)
## `Overview of the Neural Network Charity Analysis`	
	
The purpose for the project is to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

The analysis consists of three technical analysis deliverables and a written report as the following: 

- Preprocessing Data for a Neural Network Model;
- Compile, Train, and Evaluate the Model;
- Optimize the Model;
- Submit a Written Report on the Neural Network Model.
## `Resources`	
The analysis is created using next software: Jupyter-notebook 6.3.0, Python 3.8.8, Pandas 1.2.4, machine learning libraries for Python: tensorflow 2.6.0, scikit-learn 0.24.1, Visual Studio Code 1.58.0.

## `The Neural Network Charity Analysis Result`
### `- Preprocessing Data for the Neural Network Model`	

In order to compile, train, and evaluate the neural network model later the dataset was preprocessed.

The target for the model was considered the variable 'IS_SUCCESSFUL' because the purpose is to predict whether applicants will be successful if funded by Alphabet Soup.

The features for the model were considered the variables such as APPLICATION_TYPE,	AFFILIATION	CLASSIFICATION,	USE_CASE,	ORGANIZATION,	STATUS,	INCOME_AMT,	SPECIAL_CONSIDERATIONS,	ASK_AMT.

The variables EIN, NAME for the model were removed from the input data.

The result of preprocessing Data for the Neural Network Model can be found in the [AlphabetSoupCharity](./AlphabetSoupCharity.ipynb) file.

### `- Compile, Train, and Evaluate the Model`

To create a binary classification model that can predict if an Alphabet Soup–funded organization will be successful based on the features in the dataset the neural network model was created. 

The result of the Compile, Train, and Evaluate the Model can be found in the [AlphabetSoupCharity](./AlphabetSoupCharity.ipynb) file.

Since the purpose to create binary classification, the neurons were selected 80 and 30 and the layers were selected 2 and the activation functions were selected 'relu'(It can be used for classification) for hidden layers and 'sigmoid' (is ideal for binary classification) for output layer.

The target model performance was achieved following:

screen del 2
### `- Optimize the Model`

In order to achieve a target predictive accuracy higher than 75% the model was  optimized. 

For 1 attempt the module was optimized as following:

  - dropping column

screen

  - creating more bins for rare occurrences in columns

screen


But the accuracy was decreased as on the screenshort

screen

For 2 attempt the module was optimized as following:

  - adding more neurons to a hidden layer

screen

  - adding more hidden layers

The accuracy increased a bit but still low as on the screenshort:

scree

For 3 attempt the module was optimized as following:

  - using different activation functions for the hidden layers

screen

  - adding the number of epochs to the training regime

screen

The accuracy increased but didn't achieve the target predictive accuracy higher than 75%.

screen

The result of the Ensemble Classifier algorithm can be found in the [AlphabetSoupCharity_Optimzation](./AlphabetSoupCharity_Optimzation.ipynb) file.

## `The Neural Network Charity Analysis Summary`

The overall results of the deep learning model is the optimized model was not capable to achieve the target predictive accuracy higher than 75% with the modifications as dropping column in initial datasets, creating more bins for rare occurrences in columns, increasing the number of values for each bin, adding more neurons to a hidden layer and  hidden layers, using different activation functions for the hidden layers and adding the number of epochs to the training regime.

As recomendation to achieve the target performance as the predictive accuracy higher than 75% it can be to keep all initial data and define the deep neural net model with 2 layers.
