# Neural_Network_Charity_Analysis
# Overview analysis

The project will help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. The dataset is composed by the columns (EIN, APPLICATION_TYPE, AFFOLIATION, CLASSIFICATION, USER_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONDIERATIONS, ASK_AMT, and IS_SUCCESSFUL).


# Results

## Data Processing

Target: IS_SUCCESSFUL COLUMN
Features for the model: Every Column except for IS_SUCCESSFUL
Removed: EIN

## Compiling, Training, and Evaluating the Model

The number of neurons, layers, and activation functions I selected for my neural network model:

For my neural network model I had 2 hidden layers. My first layer had 80 neurons, the second has 30 there is also an output layer. The first and second hidden layer have the "relu" activation function and the activation function for the output layer is "sigmoid."

Attempt 1: Removed additional feature, that is the 'USE_CASE' column. Rest of the model components stayed the same, however model accuracy went down to 63%.
Attempt 2: Adding Additional neurons to hidden layers and additional hidden layers are added. The accuracy went down again, this time it was 53%.
Attempt 3: Changing activation function of output layer from "sigmoid" to "tanh." The accuracy of the model went down even more to 50%.

![alt text](https://github.com/Herbert-0820/School_District_Analysis/blob/main/Screen%20Shot%202021-09-24%20at%209.00.40%20PM.png)




# Summary

The model ended up with the accuracy score of 46.68% after optimization. The initial neural network had a accuracy score of 69%. This loss in accuracy can be explained from the fact that the model overfitted. Furthermore, we could further also optimize our neural network by removing more features or simply adding more data to the dataset to increase accuracy. Since our accuracy score was not particularly up to the standard with neural networks, we could have used the Random Forest classifiers. This is because random forest is a robust and accurate model due to their sufficient number of estimators and tree depth. Also the random forest models have a faster performance than neural networks and could have avoided the data from being overfitted.

