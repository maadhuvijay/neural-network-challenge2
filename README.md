# neural-network-challenge2

## Predict employee churn  
  This project is to create a neural network that HR can use to predict whether employees are likely to leave the company. Additionally, HR believes that some employees may be better suited to other departments, so we have to predict the department that best fits each employee. These two columns should be predicted using a branched neural network.

  ### Part 1: Preprocessing
Import the data and view the first five rows.

Determine the number of unique values in each column.

Create y_df with the attrition and department columns.

Create a list of at least 10 column names to use as X data. You can choose any 10 columns you’d like EXCEPT the attrition and department columns.

Create X_df using your selected columns.

Show the data types for X_df.

Split the data into training and testing sets.

Convert your X data to numeric data types however you see fit. Add new code cells as necessary. Make sure to fit any encoders to the training data, and then transform both the training and testing data.

Create a StandardScaler, fit the scaler to the training data, and then transform both the training and testing data.

Create a OneHotEncoder for the department column, then fit the encoder to the training data and use it to transform both the training and testing data.

Create a OneHotEncoder for the attrition column, then fit the encoder to the training data and use it to transform both the training and testing data.

  ### Part 2: Create, Compile, and Train the Model
Find the number of columns in the X training data.

Create the input layer. Do NOT use a sequential model, as there will be two branched output layers.

Create at least two shared layers.

Create a branch to predict the department target column. Use one hidden layer and one output layer.

Create a branch to predict the attrition target column. Use one hidden layer and one output layer.

Create the model.

Compile the model.

Summarize the model.

Train the model using the preprocessed data.

Evaluate the model with the testing data.

Print the accuracy for both department and attrition.

 ### Part 3: Summary
Briefly answer the following questions in the space provided:

1. Is accuracy the best metric to use on this data? Why or why not?

*Accuracy might be the best metric if the feature values are balanced. Here the attrition and department features are not balanced sets. So, "Accuracy" might not be the best metric.
What activation functions did you choose for your output layers, and why?*

2. What activation functions did you choose for your output layers, and why?

*I used 'Softmax' activation function for department output layer as it is a categorical classification column and used sigmoid activation for attrition column as it is a binary column.*
  
3. Can you name a few ways that this model could be improved?

*Ways to improve the model performance: Use class weighting, Experiment with different loss functions, Hyperparameter tuning.*
  
