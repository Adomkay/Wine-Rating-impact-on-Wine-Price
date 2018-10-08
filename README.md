<img src="https://github.com/jarty13/Wine-Rating-impact-on-Wine-Price/blob/master/wine.png" width="250" height="350">

# Project Motivation
* Is there a linear relationship between the price of wine and the wine rating. If a wine has a higher rating, is there opporunity to increase price of the wine to drive more revenue?
* Can wine reviews/descriptions have a relationship to the price category of wine.


# Data Clean-up and  Exploration
* Utlizing the Kaggle Dataset from Wine Enthusiast, analyzed data to see if wine description/rating had an impact on the price of wine that were produced in US, Europe, Australia and Argentina.
* Used Logisitc Regression to see if the wine description could accuratly categorgize if the wine was categorgized as "Cheap"( <$15), "Low"( $15- $40)," Medium"($40-$100), "High"(>$100)
* Data included over 130 wine reviews from wines produced in US, Europe,Australia and Argentina. 
* Reduced deimensionality of our data by categorizing the wines into 19 different categories ranging from dry/sweet reds to drt/sweet white wines.
* Vecotorized wine descriptions using sklearn TfidfVectorizer to get a unqique list of all words mentioned in the wine reviews

<img src="https://github.com/jarty13/Wine-Rating-impact-on-Wine-Price/blob/master/wine%20rating.png" width="650" height="450">

<img src="https://github.com/jarty13/Wine-Rating-impact-on-Wine-Price/blob/master/wine%20price%20distribution.png" width="650" height="450">

<img src="https://github.com/jarty13/Wine-Rating-impact-on-Wine-Price/blob/master/price%20distribtuion%20by%20type%20of%20wine-%20US.png" width="850" height="450">

<img src="https://github.com/jarty13/Wine-Rating-impact-on-Wine-Price/blob/master/price%20distribution%20by%20type%20of%20wine%20-%20other%20countries.png" width="850" height="450">

# Results:
* looking at the relationship to price and rating, we saw that there was small but linear relationship in the price of wine produced in the US, resulting in a R2 of .66. WHile the Wines in Europe, Argentina and Austrlia had less of a linear relationship, since they had higher priced wine ranging above $250 that were reviewing ratings at our mean rate per bottle of wine of 88. 
* running a logistic regression to predict the price of wine off of the words in a wine review resulted in an overall accruacy if 
# Next Step:
- check out my repository predicting the type of wine based off of the words in a wine review multilayer perceptron:
https://github.com/jarty13/Using-MLP-to-categorize-wine-based-off-of-wine-reviews
