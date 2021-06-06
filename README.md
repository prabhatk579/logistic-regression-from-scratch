<h1 align = center>Logistic Regression Basics</h1>

## Requirements
- numpy
- pandas
- matplotlib
- seaborn
- sklearn

##### Dataset used is [Iris Dataset](https://archive.ics.uci.edu/ml/datasets/iris)

### Dataset Description
This dataset consists of IRIS flower species on the basis of flowers attribute measurements namely “Sepal Length”, “Sepal Width”, “Petal Length” and “Petal Width”. It consists of four features namely **SepalLengthCm, SepalWidthCm, PetalLengthCm** and **PetalWidthCm** and three calsses namely **Iris-Setosa**, **Iris-Virginica** and **Iris-virsiclolor**. It consisits of 150 entries and dataset is balanced (i.e. each class have equal amount of entries).

We start by visualizing the dataset to know how the dataset is distributed and if it is balanced or not. To plot our data, we used `seaborn.pairplot()`; it will show us the distribution of with respect to every feature.

## Preperation for logistic regression

For Logistic regression; we start by removing a class from the dataset as we are doing silmple binary logistic regression.
After removing any class, we check for outliers and remove them from our data.

### Model construction

We change the classes name to a binary number for simplified differentiation between the classes.

After changing classes names to integers, we then devide the data in testing and training data, the most common split is 80% training data and 20% testing data.

## Creating usesr defined function for logistic regression

We create a user defied function `weightInitialization` which will assign weights to each entries. We then define **Sigmoid** function to classify our data. **Cost Function** is defined next along with the **Descent Gradient**.

Then we create a user defined function for logistic regression and cross check the answer with the library function.
