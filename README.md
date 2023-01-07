# ML-final

## Description

This project is an implementation for a Kaggle competition. The goal of the competition is to predict product failures by using a Machine Learning Model given the results of an extensive testing study.

Competition link: https://www.kaggle.com/competitions/tabular-playground-series-aug-2022


## Environment
The training and inference notebooks are both written in Colab using Jupyter Notebook. The trained models were stored in a pickle file, then loaded into the inference notebook for testing.

The packages used in notebooks include: `pandas`, `pickle`, `numpy`, `dataclasses` and `sklearn`.


## Training Notebook

The training notebook contains three parts:
+ Data Loading and Pre-processing
+ Grid Search to find the best parameters for the model, which is Logistic Regression
+ Cross-Validation to validate model's performance and store the models that are transformed for each round
+ Dump all models into a pickle file

To train the model, run the training notebook by clicking `run all`



## Inference

The testing notebook contains three parts:
+ Data Loading and Pre-processing
+ Model Loading from the pickle file generated in the training notebook or from the link below
+ Prediction Generation from the average predicted failed probability by all models


To generate the submission file for the Kaggle Competition,  run the inference notebook by clicking `run all`

## Trained Models

The trained model can be downloaded here:
https://drive.google.com/file/d/1wf9DZudaP9dEbCkKXYCwlmGx4ba1L5Kt/view

## Results

The model achieves the following performance on :


| model name  | area under the ROC curve  | 
| ----------- | ------- |
| Logistic Regression | 0.59017 |

