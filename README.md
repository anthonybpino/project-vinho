## Project -4 Wine Quality Analysis



## Group- 3 Members:
Purnima Pathak, 
Anthony Pino, 
Emily Washburn, 
Sergio Roberto de Souza Junior 



## Background


Tasty Wine manufacturing company wants to enhance their taste of wine and supply it to European countries to expand their business. They sought the help of Team-3 Agency to analyze the dataset of wine quality that has 6449 wine Ids. Based on the quality ratings in the dataset, Team-3 Agency’s task is to provide Tasty Wine with the hidden trends and patterns in what makes a good wine based on its ingredients so that they can manufacture quality wine for export. The Agency is using Unsupervised Machine Learning to find what ingredients affect the quality of wine.

## Cleaning And Exploring
The first thing we did was to clean the data. We used SQL Alchemy, created an engine that can connect to the database and queried the data and created a data frame. We dropped duplicate items and dropped unwanted columns. Then started the data exploration where we started the comparison between density and other wine ingredients like- fixed acidity, citric acid, chlorides, total sulfur dioxide, ph. value, alcohol content, volatile acidity, free sulfur dioxide, residual sugar, sulphates and quality.

![bar_charts](https://github.com/anthonybpino/project-vinho/assets/125159045/72e2d3b4-3327-482f-b106-a7dec8f0af61)


Through our data exploration we found 4 areas that affected quality-
The lower the volatile acid the higher the wine quality. 
The lower the chlorides the higher the wine quality.
The higher the citric acid, the higher the wine quality.
The higher the alcohol content, the higher the wine quality.

![barchart](https://github.com/anthonybpino/project-vinho/assets/125159045/440e7039-6a91-4c29-938b-31c265a8a383)


## PCA Method (Unsupervised Machine Learning)

We went for PCA Method to do the unsupervised machine learning with our dataset.
We checked the variation of wine density which came out to be 0.05187. The variation in wine density is very small and most likely it does not have any effect on the quality of wine, so we dropped the density column. The variation in alcohol content came out to be 6.9, so we are keeping it. 
We used pd.get_dummies on types which were red wine and white wine to turn it from categorical values to numerical values and we appended it to the main data frame and then dropped the type column. Fit transform method was used through scikit-learn library before using the machine learning algorithms to reduce noise, remove redundant features so that computational efficiency can be improved. We used Kmeans clustering algorithm and got the elbow curve and predicted and plotted the model.
![PCA_elbow](https://github.com/anthonybpino/project-vinho/assets/125159045/e11572d2-6fb6-488c-ba6b-9885dd874ca9)

![model](https://github.com/anthonybpino/project-vinho/assets/125159045/061278fb-23a9-45a3-9710-afd3cc701a3f)
![plot 1](https://github.com/anthonybpino/project-vinho/assets/125159045/ff18898e-c015-4da5-8f86-9dc67e1148df)



Dataset Source-
https://www.kaggle.com/datasets/subhajournal/wine-quality-data-combined
Documentations-
https://seaborn.pydata.org/archive/0.11/generated/seaborn.distplot.html
https://faculty.washington.edu/yenchic/18W_425/Lec6_hist_KDE.pdf





