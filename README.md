# personal_dataset
My personal dataset project for Data Analytics
Data from: https://www.kaggle.com/rashikrahmanpritom/heart-attack-analysis-prediction-dataset?select=heart.csv

Motivation:
The motivation for this project was the thought of being able to predict a heart attack given a couple inputs of data, the question that I wanted to answer was "Does age and chest pain have a good indication of weather or not a person will have heart attack later on?" This may seem like a trivial question but I wanted to be sure, I also checked the correlation of a couple other data entries with the likelihood of a heart attack.

Data Process:
The data cleaning and importing proccess was not all to bad, I found a .csv file off of kaggle that had many many columns of differnt inputs of data, they even provided a heart attack likelihood output which was very helpful in indicating how certain data points would affect a heart attack likelihood. The main cleaning proccess that I did was removing columns that I did not need to be working with and cleaning up some basic things with the .csv file in order to work with them a little more easily. I tried out quite a few methods of analysis to see if there was a correlation betweeen the chestpain, age and whether or not the person is going to have a heart attack or not.To my suprise there was not to much of a correlation, as shown by the graph below.

![image](https://user-images.githubusercontent.com/79605257/113781306-5a348280-96e5-11eb-9dfa-c661920f53e9.png)



This graph reprents the ages of three different groups of people that have different levels of chest pain, the colors separate the likelihood of heart attack.


Analytical Technique:
The data set that I had gotten off of Kaggle was very high dimensional, with about 15 different columns that each represented a different variable some of which were continuous and some discrete. The final column in the dataset was an output column that represented the likelihood of a heart attack for each individual. This setup of high dimensional data and an output that is represented by two diffrent outcomes is perfect for clustering using principal component analysis. I tried out grouping the data quite a few different ways and even trying out grouping with chest pain rather than heart attack outcomes. I was kind of suprised that none of the groupings ended up working out, even after trying a bunch of different combinations of columns and omitting some that did not seem to be effecting much. I am glad I did the PCA, I could tell that using the dimension reduction was a step in the right direction, and while still not having correlation I could tell that the PCA clustering showed more correlation than a matrix of scatterplots did.
