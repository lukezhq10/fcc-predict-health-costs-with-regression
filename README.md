# Linear Regression Health Costs Calculator
This includes the Linear Regression Health Costs Calculator project from FreeCodeCamp under the Machine Learning with Python course at https://www.freecodecamp.org/learn/machine-learning-with-python/machine-learning-with-python-projects/linear-regression-health-costs-calculator

# Project Description
We cleaned the dataset, split it into train and test datasets, created a Sequential CNN model and trained it using the train dataset to create a health costs calculator, where given multiple variables such as age, sex, bmi, etc. we are able to predict the health cost expenses with an accuracy of Mean Absolute Error < 3500.

Originally, the model wasn't able to pass the challenge. The model was updated to be more accurate by:
1. increasing the learning rate of the RMSprop optimizer from the default learning rate=0.001 to 0.05. The RMSprop optimizer adjusts the learning rate for each weight based on the historical gradient magnitudes. This adaptation helps the optimization process to find the minimum of the loss function more efficiently. Increasing the learning rate allows the model to make larger updates to the weight during training, improving our model accuracy.
2. increasing the number of epochs. At first, we started with epochs=10 while training the model and ended up with epochs=500. Increasing epochs means more training iterations and improved learning by the model. There is an overfitting risk with this however.
