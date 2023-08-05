# Changelog

A summary of changes for project-vinho

## 08.05.23

### Updates:

- Change of project description to match the work done with unsupervised learning
- Addition of changelog.md to report changes made to the project

## 08.03.23

### Updates:

- Deletion of supervised learning notebook. Deemed unnecessary after unsupervised learning deemed successful
- Upload WineQuality.csv to postgres. Create table and sql statement to store data. Upload sql file to repository
- Add sqlalchemy to unsupervised notebook. change from reading in csv to reading in database
- Fill spaces in column headers with underscores. {"volatile acidity": "volatile_acidity}

## 08.01.23

### Updates:

- Use of PCA to find if something in the data causes changes to other things. PCA1 longer than PCA2
- upload PCA scatter plot to output folder
- Plot quality against features of wine using seaborn
- Find alcohol content and citric acid are more commonly grouped in higher quality wines
- Find volatile acidity and chlorides are more commonly found in lower quality wines
- Drop all columns except alcohol, citric acid, volatile acidity, chlorides, and quality for another round of unsupervised learning
- Plot clusters, which are more obviously grouped than before data exploration, possibly signifying that these features indeed do effect quality
- Upload all charts to output folder

## 07.31.23

### Update:

- Create notebook for supervised learning work

## 07.28.23

### Updates:

- Clean data by changing "Unnamed: 0" to wine_data and making it the index
- Scale and transform dataframe for unsupervised learning using KMeans
- Use get_dummies to change "white wine" and "red wine" to 1 and 0
- Create elbow plot to find how many clusters to use.
- Create scatter plots after unsupervised learning. Will attempt to find which columns aren't as important

## 07.27.23

### Initial commit:

- Upload resource folder containing wine data
- Initial data exploration in notebook, including adding it to a dataframe