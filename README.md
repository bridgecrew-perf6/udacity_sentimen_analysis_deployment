# SageMaker Deployment Project

## Itroduction

A basic binary Sentiment Analysis model is created based on IMDB movie reviews. The main part where we want to focus is not the model or training but the deployment.<br>
The deployment is very crutial part of any Machine Learning project. Here we have leveraged **AWS Sagemaker** and other AWS services like **S3**, **Lambda**, **API Gateway** to create a webapp which shows if the typed movie review is poitive or negetive.

## About the Notebooks
The soul of these project are the **Jupyter Notebook**. There are 3 notebooks where **python3** is used as programming language. <br>
- The _SageMaker Project.ipynb_ is where the whole project is completed. Here we have used **PyTorch 0.4** to create the **RNN** model. 
- The _SageMaker Project-experiment-16.ipynb_ here I have tried to achieve same using **PyTorch 1.6** but Sagemaker works differently with recent pytorch version. More details in mentioned under Issues.
- The _SageMaker Project-experiment.ipynb_ is kind of a scrap book which I kept to refer later.

## Issue
As mentioned earlier I am unable to use **PyTorch 1.6** model for predictions. While loading the model in deployed invironment it is looking for searching for model artifacts in wrong directory, which is causing an error. Go through _SageMaker Project-experiment-16.ipynb_ the error message is pasted.
