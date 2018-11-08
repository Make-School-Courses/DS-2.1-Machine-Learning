# Principal Component Analysis

## What is principal component analysis? (5 min)

- PCA is a mathematical technique to reduce redundancy in the data
- PCA is one of the well-known algorithm for Dimensionality Reduction


## PCA Visualization (15 min)
- http://setosa.io/ev/principal-component-analysis/
- https://www.youtube.com/watch?v=5HNr_j6LmPc&t=264s

## Activity: are the countries in great UK different in terms of food? (20 min)
- In the table is the average consumption of 17 types of food in grams per person per week for every country in the UK
- It would be great if we represent difference among UK countries based on the food they eat visually
- Write a Python code that visualize the PCA component for the dataset

## The mathematics for eigenvalue and eigenvector (20 min)
- http://www.math.harvard.edu/archive/20_spring_05/handouts/ch05_notes.pdf


## Activity: write a Python code to return PCA (30 min)
1- Subtract column mean from feature matrix

2- Calculate the covariance of centered matrix

3- Calculate the eigenvalue and eigenvector of covariance matrix

4- Return the first K (two for example) column of matrix multiplication of centered matrix with eigenvector matrix

- Compare the result of custom function with PCA in sklearn

- Calculate the correlation of the first two principle component

- How much of the dataset information is preserved in the first two components?

- Hint: use `pca.explained_variance_ratio_`
