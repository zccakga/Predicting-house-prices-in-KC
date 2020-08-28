# Predicting-house-prices-in-KC

<p>The dataset for this project was obtained from https://www.kaggle.com/harlfoxem/housesalesprediction. It includes prices of the houses sold in King County (U.S.) between May 2014 and May 2015. The columns include features such as number of bedrooms and bathrooms, square foot living, location of the house etc.</p>

<p>There are altogether 18 features in the dataset but some of these are highly correlated, such as the square foot living area of the nearest 15 neighbours and the square foot living area of the house sold, hence 3 variables were dropped. In the dataset there is an entry for a house sold for $640,000 that has 33 bedrooms with only 2 bathrooms, this is most likely a typo and the 33 bedrooms was changed to 3 bedrooms. No other oultiers were found. </p>

<p>The prices of the houses are highly skewed, with the vast majority being sold below 1 million dollars. It is also reasonable to assume that houses over 1 million dollars have a wider range of features and it is harder to predict their value. Therefore, it was decided to only focus on houses below 1 million dollars in this project</p>

<p>K-fold cross validation with XGBoost gave the best result with a root mean square error of $74,000 and an r^2 score of 0.85. Given that the mean house price is $450,000 the model can be used as a reasonable price guide by estate agents and homeowners wanting to sell their house. This model would, however, have to be trained regularly on new data as house prices can fluctuate dramatically.</p>

<p>See the python notebook for this project for more information </p>
