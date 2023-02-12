# Customer-Churn-Prediction

> feature engineer and assess which classification model can best predict if a customer churns

<img src="churn.jpg" width="500" height="275">

## Introduction 

The goal of this project is to **analyze and predict customer churn in Teleco customers**. Specifically, we explore the Teleco Customers data set to uncover any relationships between the target variable (*churn*) and other variables in the dataset. From here, we seek to build a model that can accurately classify if a customer has churned, with a focus on **finding a model that has a high recall and is suitably accurate across the board**.

## Data

The data set is a Teleco Customer Churn data set from [Kaggle](https://www.kaggle.com/blastchar/telco-customer-churn). Our outcome of interest is `churn`, a binary variable - customers who left within the last month. There are 16 other categorical variables and 4 numerical variables. 

## Methodology & Models



The goal of our modelling is now to ascertain which model can  most accurately classify if a customer has churned. Parameters and features may be transformed and selected using GridSearchCV and PCA. Specifically, we shall examine eight different models, all listed below: 


* **K-nearest Neighbors Classification**
    * A non-parametric classification algorithm that uses a distance metric to determine the *k* nearest neighbors of a data point and then classifies the data point based on the majority vote of its *k* nearest neighbors.

<br>

* **Logistic Regression**
    * A linear classification algorithm that predicts a binary outcome (0 or 1) based on a linear combination of independent variables. The algorithm uses a logistic function to model the probability of a binary outcome and then classifies the data point based on the predicted probability.

<br>

* **Ridge Classification**
    * A regularization technique for linear regression that seeks to reduce the magnitude of the coefficients in the linear regression model. The ridge classification algorithm is used to prevent overfitting and improve the generalization performance of the model.

<br>

* **Lasso Classification**
    * Another regularization technique for linear regression that seeks to reduce the magnitude of the coefficients in the linear regression model by setting some coefficients to zero; Ridge reduces the magnitude of the coefficients but does not set any coefficients to zero.
    The lasso classification algorithm is used to perform feature selection and improve the generalization performance of the model.

<br>

* **Decision Tree Classification**
    * A tree-based classification algorithm that creates a binary tree structure to classify data points based on a series of if-else statements. The algorithm splits the data into smaller and smaller subsets based on the most important feature until each subset only contains data points of a single class.

<br>

* **Random Forest Classification**
    * An ensemble of decision trees created by randomly selecting a subset of features for each tree in the forest. The random forest classification algorithm combines the predictions of all the trees to produce a final prediction.

<br>

* **Support Vector Classification (SVC)**
    * A linear classification algorithm that finds the hyperplane that best separates the data points into two classes. The algorithm seeks to maximize the margin between the two classes and is commonly used for linearly separable data.

<br>

* **Gradient Boost Classification**
    * An ensemble of decision trees that are fit one at a time and use the errors from the previous tree to inform the next tree. The gradient boost classification algorithm seeks to reduce the error of the model by adding trees to the model until the error plateaus.

The models were evaluated based on recall, precision, and F1-score to determine the most accurate model. 

## Results

The final model could predict churn 83% of the time, though it also classified that many non-churners would churn. Our final model was a logistic model using a mix of categorical and continuous variables. The *classical* statistical method for binary classification could predict churn 83% of the time, though it also classified that many non-churners would churn. This may be of a surprising result, beating a lot of algorithms which have claimed superior classification performance.

## Conclusion

This project demonstrates the use of classification models to predict customer churn in Teleco customers. The results showed that the final model, a logistic model using a mix of categorical and continuous variables, was able to predict churn 83% of the time.


## Getting Started

This project is implemented in Python. To run this project, the following software and packages are required:

- Python
- pandas
- numpy
- scipy

To run this project, clone or download the repository and open the jupyter notebook. The code and data are included in the repository.

## Contributions

If you want to contribute to this project, feel free to submit a pull request or open an issue in the repository.


## Contact

For any questions or queries, please email: sngpav003@myuct.ac.za


