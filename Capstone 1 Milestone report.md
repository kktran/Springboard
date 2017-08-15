## Problem and Client

This project aims to predict whether an individual earns over $50,000 a year based on demographic attributes from the 1994 census. A project of this nature could provide significant value to a variety of clients. For instance, in the absence of information about the annual income of a potential customer, a business could attempt to predict the income bracket of an individual and target the segment that would want the product most. From a large database of potential customers, the most likely customers could be contacted to increase the efficiency and rate of customer acquisition. 

## Data Set Information and Cleaning

The data used for this project was obtained from the 1994 Census and hosted in the UCI Machine Learning Repository (link: http://archive.ics.uci.edu/ml/datasets/Adult). Other census data from other uses could similarly be used for this analysis. The data set consits of 32,561 records each representing a single individual. The following attributes are provided: age, workclass, fnlwgt, education, education-num, marital-status, occupation, relationship, race, sex, capital-gain, capital-loss, hours-per-week, native-country. The final column describes whether the individual earned over or under $50,000 a year in 1994. Records with missing information (represented with '?') were removed from the data set. 

In the cleaning process, non-numeric variables were reduced into fewer categories to simplify analysis. All self-employed work class individuals were grouped together. For education, all individuals under high school graduate education were grouped and all associate degree graduates were grouped. Individuals with some college education but without a degree were grouped with high school graduates. For marital status, "divorced", "married-spouse-absent", "separated", and "not-married" individuals were grouped, and all other married individuals were grouped as "married". The columns fnlwgt and education-num were dropped (for irrelevance and overlap with education level, respectively).

## Initial Findings

Before undertaking the machine learning prediction component of the project, the data set was explored through simple visualization and  hypothesis testing. 75.1% of individuals in the data set earned under $50,000 a year. Particularly insightful attributes for predicting an individual's income level were education level, marital status, sex, age, and occupation. Chi square and z-score tests were used to verify that these attributes were significant factors in income at a significance level <10^-100. 
