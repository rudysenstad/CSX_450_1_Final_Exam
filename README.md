# CSX_450_1_Final_Exam


Abalone
=====

## Domain

This problem uses measurements of physical properties of abalone (e.g. weight, number of rings, age, sex, etc.). The data was collected for the study "The Population Biology of Abalone (_Haliotis_species) in Tasmania. I. Blacklip Abalone (_H. rubra_) " by Warwick J Nash, Tracy L Sellers, Simon R Talbot, Andrew J Cawthorn and Wes B Ford published in  "North Coast and Islands of Bass Strait", Sea Fisheries Division, Technical Report".


## Problem Statement

Without machine learning, the only way to know the number of rings (a.k.a the age) of an abalone is to cut it open, dye it and count the rings. Given physical properties about abalone, we will use supervised learning to develop a regression model that can predict the number of rings in the abalone so to minimize the physical job of opening the shell and dying.

We examine a number of factors that relate to abalone from Tasmania. In particular, we wish to understand the association between an employee’s `rings` and other physical attributes, namely `height`, `diameter` and `length`.

## Dataset

The abalone dataset from Tasmania (available [here](https://archive.ics.uci.edu/ml/machine-learning-databases/abalone/))

- Number of samples: 4177 
- Number of attributes: 9
- Expected Dataframe Dimensions: 4177 rows x 9 columns
- Column Data Types: 8 columns are float and 1 integer
- Target: n/a
- Theoretical Memory Footprint: 11.5 kB
   - 4177 rows x 7 float columns = 29239
   - 4177 rows x 1 int column = 4177
   - 29239 elements x 8 bytes per float + 4177 elements x 4 bytes per int = 250620 bytes = 245 kB



## Solution Statement

A solution to this problem will be a regression model such as a linear regression, a decision tree regressor, or a support vector regressor. 


## Benchmark Model

Given that we seek a regression model a good naive benchmark would be to use either the mean or the median of the volume of the abalone assuming it's a cylinder shape,  π*r^2*h 


## Performance/Evaluation Metric

Given that this is a regression task, we can measure the success of our model using the R^2 metric, the Mean Absolute Error, or the Mean Square Error.
