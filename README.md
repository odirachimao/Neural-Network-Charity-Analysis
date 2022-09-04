# Neural-Network-Charity-Analysis

## OVERVIEW OF THE ANALYSIS: 

This project uses deep-learning neural networks using TensorFlow in Python to analyze the success of Alphabet Soup's long term donations to multiple organizations. Here we look to see whether applicants will be successful or not. 


## RESULTS:

## Data Preprocessing: 

- The column "IS_SUCCESSFUL" is the target for our deep learning neural network because it contains binary data that tells us if the charity donation was used effectively. 

- The columns "APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT" are features of our neural network. Encoding of the categorical variables, spliting into training and testing datasets and standardization have been applied to the features.

- The columns "EIN" and "NAME" are identification information and have been removed from the input data as they added no value to the model. 

## Compiling, Training, and Evaluating the Model:

- This network model is consist of two hidden laters with 80 and 30 neurons respectively. There are 43 features and 25,724 samples in this input data. The output layer is made of a unique neuron as it is a binary classification. We used the activation function ReLU to speed up the training process for hidden layers, and Sigmoid for the output layer. We also used the optimizer Adam and the loss function binary_crossentropy for compilation. 

- The model accuracy is under 75%. This is not a satisfying performance to help predict the outcome of the charity donations.

- To increase the performance of the model, we applied bucketing to the feature ASK_AMT and organized the different values by intervals. We increased the number of neurons on one of the hidden layers, then we used a model with three hidden layers. 


## SUMMARY: 

Overall, we conclude that the deep learning neural network model is outperforming because it did not reach the target of 75% accuracy. Since we are in a binary classification situation, we could use a supervised machine learning model such as the Random Forest Classifier to combine a multitude of decision trees to generate a classified output and evaluate its performance against our deep learning model.
