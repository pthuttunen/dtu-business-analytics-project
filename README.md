# dtu-business-analytics-project
Final project for DTU course Introduction to Business Analytics. The project was done in collaboration with two other students. My responsibility was the predictive notebook, in addition to descriptive statistics and helping with the other parts.

## Introduction
The challenge relates to the housing market in the Santiago de Chile area. A relevant dataset was provided and used to perform different analyses on. The challenge is split into three components: a prediction challenge, an exploratory component and the report notebooks. To address the different components of the challenge the final handin contains four notebooks that should be read in the following order:

1. Descriptive Statistics Notebook
2. Additional Dataset Notebook
3. Exploratory Notebook
4. Predictive Notebook

## The dataset
The dataset that was provided for the challenge contains a few details about different house transactions, such as the latitude/longitude coordinates, the transport accessibility context of the area and some characteristics of the household that bought the house. The data was examined in the Descriptive Statistics Notebook. In addition to the given dataset, our group used point of interest -data for the Santiage de Chile area. This dataset was examined in the Additional Dataset Notebook

## Exploratory work
The following questions were addressed in the Exploratory Notebook:
- How is accessibility distributed across space?
- Are there particular areas that somehow relate to together?
- Can we explain why?

The __main idea__ to approach these questions is the following:
1. __Clustering__ household data according to their accessibility (using all the features from the "accessibility" group, see descriptive statistics notebook)
2. __Visualizing__ accessibility for every data point in a map (using a colour scale)
3. __Identifying__ areas with high and low accessibility
4. __Finding explanations__ for the (un)evenly distributed accessibility across space by visualizing information from an __external data set__:
   - location of __points of transport__, such as roads, metro lines and bus stations
   - location of __points of interest__, such as supermarkets, schools and restaurants

## Predictive models
The Predictive Notebook aims to predict the CLASE variable, which is a categorical variable with three different categories related to the extent of education in each household. It was instructed to use specific testing and training datasets based on the latitude and longitude of houses. Due to the high number of variables, PCA was first used for dimension reduction. The following models were tested for the prediction task:
- Logistic regression (baseline)
- Logistic regression with l1 regulizer
- Support Vector Machines
- KNeighbors classifier
- Random forest
- Simple neural network with l2 regulizers
