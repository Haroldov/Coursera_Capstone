# <p align="center"> Capstone Project for IBM Data Science Professional Certificate </p>
### <p align="center"> Author: Haroldo Vélez Lora</p>


## 1. Introduction
<p align="justify">Recently, Machine Learning (ML) algorithms are widely used in the study of data instead of traditional statistics. ML algorithms bring advantages because they offer solutions to problems related to the big quantities of data and set fewer constraints than traditional statistics. In particular, unsupervised learning algorithms are used to find patterns in data in terms of similarity between samples. Depending on the pattern within the data, different algorithms are used. For non-convex data it is used Density-Based Spatial Clustering (DBScan). On the other hand, for convex data it is used a well known algorithm as K-Means. </p>

<p align="justify">Foursquare is a website where people comment and rank food sites, coffee sites, malls and parks. For instance, let's think that a Foursquare user had to move from New York city, USA to the city of Toronto, Canada. Foursquare location data along with a clustering algorithm can suggest a neighborhood in order to help this user to live in Toronto in a similar place. The neighborhood that will be suggested, will not be a random suggestion, but instead will be a place for his pleasure. Thus, previous data from New York and Toronto will be used to predict a good living neighborhood for him.</p>

## 2. Data

<p align="justify">For this project the Foursquare API will be used. A list of neighborhoods in New York and Toronto is downloaded and their respective location in longitude and latitude coordinates is obtained. The sources are the following: </p>

* New York neighborhoods: https://ibm.box.com/shared/static/fbpwbovar7lf8p5sgddm06cgipa2rxpe.json
* Toronto neighborhoods: https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M

<p align="justify">The data downloaded are the neighborhoods located in New York and Toronto. Moreover, their specific coordinates are merged. Only Manhattan neighborhoods and boroughs that contain the string "Toronto" are taken into account. A Foursquare API GET request is sent in order to adquire the surrounds venues that are within a radius of 500m. The data is formated using one hot encoding with the categories of each venue. Then, the venues are grouped by neighborhoods computing the mean of each feature.</p>

<p align="justify">The similarities will be determined based on the frequency of the categories found in the neighborhoods. These similarities found are a strong indicator for a user and can help him to decide whether to move in a particular neighborhood near the center of Toronto or not. </p>

## 3. Methodology

### 3.1. Feature Extraction
<p align="justify">For feature extraction One Hot Encoding is used in terms of categories. Therefore, each feature is a category that belongs to a venue. Each feature becomes binary, this means that 1 means this category is found in the venue and 0 means the opposite. Then, all the venues are grouped by the neighborhoods, computing at the same time the mean. This will give us a venue for each row and each column will contain the frequency of occurrence of that particular category.</p>

### 3.2. Unsupervised Learning
<p align="justify">For the purpose of doing unsupervised learning to found similarities between neighborhoods, a clustering algorithm is implemented. In this case K-Means is used due to its simplicity and its similiraty approach to found patterns. </p>

#### * K-Means:

<p align="justify">K-Means is a clustering algorithm. This algorithm search clusters within the data and the main objective function is to minimize the data dispersion for each cluster. Thus, each group found represents a set of data with a pattern inside the muldimensional features. </p>

<p align="justify"> Section which represents the main component of the report where you discuss and describe any exploratory data analysis that you did, any inferential statistical testing that you performed, and what machine learnings were used and why. </p>

## 4. Results

 <p align="justify"> Section where you discuss the results.</p>

## 5. Discussion

<p align="justify"> Section where you discuss any observations you noted and any recommendations you can make based on the results.</p>

## 6. Conclusion 

<p align="justify"> Section where you conclude the report.</p>
