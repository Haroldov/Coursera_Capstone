# <p align="center"> Capstone Project for IBM Data Science Professional Certificate </p>
### <p align="center"> Author: Haroldo Vélez Lora</p>


## 1. Introduction
<p align="justify">Recently, Machine Learning (ML) algorithms are widely used in the study of data instead of traditional statistics. ML algorithms bring advantages because they offer solutions to problems related to the big quantities of data and set fewer constraints than traditional statistics. In particular, unsupervised learning algorithms are used to find patterns in data in terms of similarity between samples. Depending on the pattern within the data, different algorithms are used. For non-convex data it is used Density-Based Spatial Clustering (DBScan). On the other hand, for convex data it is used a well known algorithm as K-Means. </p>

<p align="justify">Foursquare is a website where people comment and rank food sites, coffee sites, malls and parks. For instance, let's think that a Foursquare user had to move from New York city, USA to the city of Toronto, Canada. Foursquare location data along with a clustering algorithm can suggest a neighborhood in order to help this user to live in Toronto in a similar place. The neighborhood that will be suggested, will not be a random suggestion, but instead will be a place for his pleasure. Thus, previous data from New York and Toronto will be used to predict a good living neighborhood for him.</p>

## 2. Data

<p align="justify">For this project the Foursquare API will be used. A list of neighborhoods in New York and Toronto is downloaded and their respective location in longitude and latitude coordinates is obtained. The sources are the following: </p>

* New York neighborhoods: https://ibm.box.com/shared/static/fbpwbovar7lf8p5sgddm06cgipa2rxpe.json
* Toronto neighborhoods: https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M

<p align="justify">The similarities will be determined based on the frequency of the categories found in the neighborhoods. Therefore, the avenues near from those neighborhoods will be downloaded from the Foursquare API and the categories of each avenue will be extracted. Finally, these similarities found are a strong indicator for a user and can help him to decide whether to move in a particular neighborhood near the center of Toronto or not. </p>

## 3. Methodology

<p align="justify"> Section which represents the main component of the report where you discuss and describe any exploratory data analysis that you did, any inferential statistical testing that you performed, and what machine learnings were used and why. </p>

## 4. Results

 <p align="justify"> Section where you discuss the results.</p>

## 5. Discussion

<p align="justify"> Section where you discuss any observations you noted and any recommendations you can make based on the results.</p>

## 6. Conclusion 

<p align="justify"> Section where you conclude the report.</p>
