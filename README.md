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

![image](https://user-images.githubusercontent.com/68247343/140558318-0631ee8a-007f-4d9d-a2d8-c242c75e8b0c.png)

### `- Optimize the Model`

In order to achieve a target predictive accuracy higher than 75% the model was  optimized. 

For 1 attempt the module was optimized as following:

  - dropping column

![image](https://user-images.githubusercontent.com/68247343/140558173-7ca5720d-ca80-4ad7-a2ec-d3f7e608664b.png)

  - creating more bins for rare occurrences in columns

![image](https://user-images.githubusercontent.com/68247343/140558199-798fe036-a254-496c-893d-d9feb1fee781.png)

But the accuracy was decreased as on the screenshort

![image](https://user-images.githubusercontent.com/68247343/140558263-e04eb345-5d58-42b1-b9b7-ca43b4f30836.png)

For 2 attempt the module was optimized as following:

  - adding more neurons to a hidden layer and hidden layers
 
 ![image](https://user-images.githubusercontent.com/68247343/140558404-5ca34f24-0a42-4eee-8ff6-6e89ad075592.png)

The accuracy increased a bit but still low as on the screenshort:

![image](https://user-images.githubusercontent.com/68247343/140558437-d3cb51f1-f5fc-4744-b3da-23a6127c1f5b.png)

For 3 attempt the module was optimized as following:

  - using different activation functions for the hidden layers

![image](https://user-images.githubusercontent.com/68247343/140558479-b4b8d884-f52d-4257-882c-8aa784bd8254.png)

  - adding the number of epochs to the training regime

![image](https://user-images.githubusercontent.com/68247343/140558512-e7326d9b-db43-4595-a975-cb9b6116eb56.png)

The accuracy increased but didn't achieve the target predictive accuracy higher than 75%.

![image](https://user-images.githubusercontent.com/68247343/140558523-15d53fad-f8ba-445d-82f1-4212993af682.png)

The result of the Ensemble Classifier algorithm can be found in the [AlphabetSoupCharity_Optimzation](./AlphabetSoupCharity_Optimzation.ipynb) file.

## `The Neural Network Charity Analysis Summary`

The overall results of the deep learning model is the optimized model was not capable to achieve the target predictive accuracy higher than 75% with the modifications as dropping column in initial datasets, creating more bins for rare occurrences in columns, increasing the number of values for each bin, adding more neurons to a hidden layer and  hidden layers, using different activation functions for the hidden layers and adding the number of epochs to the training regime.

As recomendation to achieve the target performance as the predictive accuracy higher than 75% it can be to keep all initial data and define the deep neural net model with 2 layers as followng model with 75,4% accuracy.

![image](https://user-images.githubusercontent.com/68247343/140558641-01cc1d8a-1464-45f5-a255-93cf47f5285f.png)

![image](https://user-images.githubusercontent.com/68247343/140558657-fed15f75-297d-434c-a56a-808f414379a0.png)


The overall results of the deep learning model is the optimized model was not capable to achieve the target predictive accuracy higher than 75% with the modifications as dropping column in initial datasets, creating more bins for rare occurrences in columns, increasing the number of values for each bin, adding more neurons to a hidden layer and  hidden layers, using different activation functions for the hidden layers and adding the number of epochs to the training regime.
