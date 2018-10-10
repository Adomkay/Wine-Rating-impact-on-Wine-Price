<img src="https://github.com/jarty13/Wine-Rating-impact-on-Wine-Price/blob/master/wine.png" width="250" height="350">

# Project Motivation
* Is there a linear relationship between the price of wine and the wine rating. If the relationship is linear,  if the wine has a higher rating, is there opportunity to increase price of the wine to drive more revenue?
* Can wine reviews/descriptions predict the price category of the of the wine.

# Data Clean-up and Exploration
*  Utilizing the Wine Enthusiast dataset from Kaggle, analyzed the wine reviews/descriptions to see if had an impact on the price of wine that were produced in US, Europe, Australia and Argentina.
* Implemented Logistic Regression Classifier  to see if the wine description could accurately categorize if the wine was categorized as "Cheap"( <$15), "Low"( $15- $40)," Medium"($40-$100), "High"(>$100)
* Data included over 130K wine reviews from wines produced in US, Europe,Australia and Argentina 
* Reduced dimensionality of the data by categorizing the wines into 19 different categories ranging from dry/sweet reds to dry/sweet white wines.
* Vectorized wine descriptions using sklearn TfidfVectorizer to get a unique list of all words mentioned in the wine reviews

<img src="https://github.com/jarty13/Wine-Rating-impact-on-Wine-Price/blob/master/images/wine%20rating.png" width="650" height="450">

<img src="https://github.com/jarty13/Wine-Rating-impact-on-Wine-Price/blob/master/images/wine%20price%20distribution.png" width="650" height="450">

<img src="https://github.com/jarty13/Wine-Rating-impact-on-Wine-Price/blob/master/images/price%20distribtuion%20by%20type%20of%20wine-%20US.png" width="850" height="450">

<img src="https://github.com/jarty13/Wine-Rating-impact-on-Wine-Price/blob/master/images/price%20distribution%20by%20type%20of%20wine%20-%20other%20countries.png" width="850" height="450">

# Results:
*  In regards to the the relationship to price and rating, we saw that there was small but linear relationship in the price of wine produced in the US, resulting in a R-Square of 66%. While the Wines in Europe, Argentina and Australia had no linear relationship , since they had higher priced wine ranging above $250 that were reviewing ratings at our mean rate per bottle of wine of 88.
* Running a logistic regression to predict the price of wine off of the words in a wine review resulted in an overall accuracy if 66%.
* To improve accuracy will be to run a grid search, categorize the wines into more defined wine priced categories and running additional classifiers on our train and test data. 
* overall there is opporunity to increase prices on certain wines if their reviews are over 88pts with the price point in the low range, in order to increase revenue. 
 
# Next Step:
- Check out my repository classifying the type of wine from 19 different categories based off of the words in a wine review using a multilayer perceptron. I was experimenting with 4 different regularizaiton methods (Early Stopping, L1, L2 and Dropout) to see which ones would get me the best results. 
https://github.com/jarty13/Using-MLP-to-categorize-wine-based-off-of-wine-reviews
