# Predicting Titanic Survival rate using Mean Shift algorithm

Following repo classify into groups and each group is assign survival rate, so that we can study the patern of survival.

# Introduction to Mean Shift algortihm 

First let's see what is K-Mean algortihm, K-mean is unsupurvised clustering algorithm , Where you define K which refer to K centroids. Then we take each feature set and measure it with all centeroid, assign that featureset to its nearest centeroid's cluster. After formation of cluser of all feature sets we then find out the mean of cluster, Make them new cetroids and again repeat the process.

Mean Shift is similar to K Mean just the difference is that we don't define K . Hill Climbing operation is been use. As word state, idea is go up untill there is nothing left ahead, over head hill would nothing but our feature set. After reaching top of hill we find out the mean of the data and that would be our cluster centroid. 
In practise following are the steps we take
1) We take all the feature set as centroids
2) Take mean of all the feature set , setting this as new mean as new centroid
3) Repeat above set till new centroid and old centroid are almost the same.

## Getting Started

We would use MeanShift library from sklearn.
We would be using titanic dataset from kaggle.
https://www.kaggle.com/c/titanic/download/GQf0y8ebHO0C4JXscPPp%2Fversions%2FXkNkvXwqPPVG0Qt3MtQT%2Ffiles%2Ftrain.csv


## Things we did for pre processing our code
* Import the data.
* Drop the column which are not required for insights.
* Handle missing values.
* Replace categories with numeric code.
* Handle dependent variable into seprate variable.

## Insights we got from data

* We find that survival rate for Pclass = 1 has higher survival rate , we can say that Pclass = 3 lower survival rate
* Higher fare has higher survival rate
* Same tickets number would be have same survival output.

## What I interpret from the data

When titanic got started to sink , water would have been started filling from down when pclass = 3 would be staying where as the pclass = 1 would be staying at height in ship and would be having proximity to life boat.
