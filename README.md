# deep-learning-challenge
Assignment 21
Step 1: Preprocess the Data
Using  Pandas and scikit-learn’s StandardScaler(),  preprocessed the dataset. This step prepares  for Step 2, where compiled, trained, and evaluated the neural network model.

Uploading the starter file to Google Colab.

Read in the charity_data.csv to a Pandas DataFrame,  identified:
the target(s) for model ['IS_SUCCESSFUL']
the feature(s) for model(['EIN', 'NAME']
Droped the EIN and NAME columns.
Determined the number of unique values for each column.

For columns that have more than 10 unique values, determine the number of data points for each unique value.

Used the number of data points for each unique value to pick a cutoff point to bin "rare" categorical variables together in a new value, Other, and then check if the binning was successful.

Used pd.get_dummies() to encode categorical variables.

Splitted the preprocessed data into a features array, X, and a target array, y. Used these arrays and the train_test_split function to split the data into training and testing datasets.

Scaled the training and testing features datasets by creating a StandardScaler instance, fitting it to the training data, then using the transform function.

Step 2: Compile, Train, and Evaluate the Model
Using your knowledge of TensorFlow, you’ll design a neural network, or deep learning model, to create a binary classification model that can predict if an Alphabet Soup-funded organization will be successful based on the features in the dataset. You’ll need to think about how many inputs there are before determining the number of neurons and layers in your model. Once you’ve completed that step, you’ll compile, train, and evaluate your binary classification model to calculate the model’s loss and accuracy.

Continue using the file in Google Colab in which you performed the preprocessing steps from Step 1.

Create a neural network model by assigning the number of input features and nodes for each layer using TensorFlow and Keras.

Created the first hidden layer and choose an appropriate activation function.
Added a second hidden layer with an appropriate activation function.
Created an output layer with an appropriate activation function.
Checked the structure of the model.

Compiled and trained the model.
Create a callback that saves the model's weights every five epochs.
Evaluated the model using the test data to determine the loss and accuracy.
Saved and exported  results to an HDF5 file. Name the file AlphabetSoupCharity.h5.

Step 3: Optimized the Model
Used following methods to optimize your model:

Dropping more or fewer columns.
Creating more bins for rare occurrences in columns.
Increasing or decreasing the number of values for each bin.
Add more neurons to a hidden layer.
Add more hidden layers.
Use different activation functions for the hidden layers.

Made at least three attempts at optimizing  model
Created a new Google Colab file and name it AlphabetSoupCharity_Optimization.ipynb.
Imported  dependencies and read in the charity_data.csv to a Pandas DataFrame.
Preprocessed the dataset as in Step 1. 
Designed a neural network model.
Saved and exported your results to an HDF5 file. Name the file AlphabetSoupCharity_Optimization.h5.
Step 4: Wrote a Report on the Neural Network Model
