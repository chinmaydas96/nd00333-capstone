# Predict Heart Disease Using Azure Machine Learning

* This project is a part of Udacity Machine Learning Engineer with Microsoft Nanogree's Capstone project.

* In this project we will implement hyperdrive and AutoML for heart disease prediction dataset.

* We will deploy the model and do the inference with the sample json file for each model.



## Project Set Up and Installation

## Dataset





### Overview

* In this project we used kaggle's heart disease dataset.

* [Link](https://www.kaggle.com/andrewmvd/heart-failure-clinical-data)

* People with cardiovascular disease or who are at high cardiovascular risk (due to the presence of one or more risk factors such as hypertension, diabetes, hyperlipidaemia or already established disease) need early detection and management wherein a machine learning model can be of great help.


### Task

* This is a classification problem.

* Death due to Heart Failure is predicted using information usch as anaemia, diabetes, high blood pressure, platelets, serum_creatinine, serum_sodium, creatinine_phosporous and ejection_fraction.


* We will use these features to predict if the patient has heart disease or not.


### Access

* I have uploaded the csv data into the azure ml dataset directory, from there I will directly use the dataset for hyperdrive and automl.


## Automated ML
*TODO*: Give an overview of the `automl` settings and configuration you used for this experiment

* Azure machine learning studio has an AutoML functionality in which we can directly upload the dataset and it will run multiple model to get the best model with optimum metrics. 

* And the best model also can be deployed and consumed with restAPI.

* The following configuration is used here : 

	* experiment_timeout_minutes : the time in minutes after the experiment timeouts which is set to 20.

	* n_cross_validations the number of cross validations which is performed on the training data, set to 5

	* may_concurrent_iterations describes the maximal number of tasks solfed in parallel, here 5.

	* primary_metric the choosen metric - AUC_weighted

![](images/parameters.png)

### Results
*TODO*: What are the results you got with your automated ML model? What were the parameters of the model? How could you have improved it?

*TODO* Remeber to provide screenshots of the `RunDetails` widget as well as a screenshot of the best model trained with it's parameters.

## Hyperparameter Tuning
*TODO*: What kind of model did you choose for this experiment and why? Give an overview of the types of parameters and their ranges used for the hyperparameter search


### Results
*TODO*: What are the results you got with your model? What were the parameters of the model? How could you have improved it?

*TODO* Remeber to provide screenshots of the `RunDetails` widget as well as a screenshot of the best model trained with it's parameters.

## Model Deployment
*TODO*: Give an overview of the deployed model and instructions on how to query the endpoint with a sample input.

## Screen Recording
*TODO* Provide a link to a screen recording of the project in action. Remember that the screencast should demonstrate:
- A working model
- Demo of the deployed  model
- Demo of a sample request sent to the endpoint and its response

## Standout Suggestions
*TODO (Optional):* This is where you can provide information about any standout suggestions that you have attempted.
