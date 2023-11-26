# Deep Learning Challenge: Charity Funding Predictor

## Overview

Alphabet Soup, a non-profit foundation, initiated the Deep Learning Challenge to develop a predictive algorithm for forecasting the likelihood of success for funding applicants. The task involved leveraging machine learning and neural networks to create a binary classifier capable of predicting the success of organizations funded by Alphabet Soup.

## Results

### Data Preprocessing

- Created a Pandas DataFrame containing the charity_data.csv data.
- Identified target variable(s) as "IS_SUCCESSFUL" and feature variable(s) by dropping irrelevant columns (EIN and NAME).
- Determined the number of unique values in each column.
- Binned "rare" categorical variables together in a new value, "Other," based on a cutoff point.
- Encoded categorical variables using pd.get_dummies().
- Split the preprocessed data into training and testing datasets.
- Scaled the data using StandardScaler.

### Compiling, Training, and Evaluating the Model

- Designed a neural network model with three layers, determining the number of nodes based on features.
- Compiled, trained, and evaluated the model, resulting in an initial accuracy of 52.34%, falling short of the 75% target.

### Optimization

- Explored optimization methods in a new notebook, adjusting the model by introducing the "NAME" column.
- Achieved an improved accuracy of almost 74%, approaching the target performance.

## Summary

Utilizing multiple layers in deep learning models is essential for acquiring the ability to predict and classify information by systematically filtering inputs through various layers of computation.

## Report

For a detailed analysis, refer to the [report](link-to-report) associated with this challenge.

## File Structure

- [deep-learning-challenge](link-to-repository): Main repository for the Deep Learning Challenge.
  - [CharityFundingPredictor.ipynb](link-to-notebook): Notebook for initial model development.
  - [CharityFundingPredictor_Optimization.ipynb](link-to-optimization-notebook): Notebook for model optimization.
  - [AlphabetSoupCharity.h5](link-to-results): HDF5 file containing results of the initial model.
  - [AlphabetSoupCharity_Optimization.h5](link-to-optimized-results): HDF5 file containing results of the optimized model.
  - [README.md](link-to-readme): This README file summarizing the work.

