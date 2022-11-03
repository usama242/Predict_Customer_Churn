# Predict Customer Churn

- Project **Predict Customer Churn** of DevOps Engineer Nanodegree Udacity

## Project Description

In this project, the mentors provided us with a working ml project _churn_notebook.ipynb_ and the goal of the project is to create a library file and a test file that respect the norms to develop a software.

In this file, we present a sophisticated way to run our code.
We should mention that this code uses **python 3.6**

## Clean code results

This version of our code yield the following result using pylint and autopep8 commands

```
pylint churn_library.py
....
Your code has been rated at 8.70/10
```

```
pylint churn_script_logging_and_tests.py
....
Your code has been rated at 9.73/10
```

## Creating virtual env

It is a good idea to create a virtual environment first

```
python -m venv .venv
```

This folder is then used to install the needed packages listed in the requirement file.

```
pip install -r requirements.txt
```

## Running Files

Running the library file using the following command.

```
(env_name)$ python churn_library
```

The following steps executed:

- Loading the data.
- Encoding the categorical data.
- Creating EDA figures and saving then into the ./images/eda.
- Performing the feature engineering on the data.
- Train the Random Forest and Logistic Regression models and save them into the ./models file, then save the roc curves under ./images/results/.
- Find the feature importance if the random forest model and saving the yielded figure under ./images/results


| Training model can take a long time to converge

During All these steps, we log the different messages for debugging into the ./logs/churn_library.log

Running the Test file **churn_script_logging_and_tests.py**

```
(env_name)$ pytest churn_script_logging_and_tests.py
```

we excetued the steps below

- Collectes the different test of the churn library functions
- Runs these test.
- Saves the log message into ./logs/churn_library_test.log
