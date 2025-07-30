### Predicting House Prices in the United States

**Uday Mukkavilli**

#### Summary
House prices in the U.S. are a constant source of worry and anxiety. Whether you're in the market for a new home, or looking to sell one, you no doubt are concerned with the factors that influence the price of a house. 

This project poses a simple question: what drives the price of a house in the U.S.? In order to answer it, a linear regression model will be used to predict the price of a house given a set of features. It will incorporate features which have a positive correlation with the price of a house, and use those features to predict the price of a house in the US.

The dataset used for this project is Housing.csv, a dataset of more than 21,000 properties listed for sale across the U.S from 2014-2015. The dataset is sourced from Kaggle: https://www.kaggle.com/datasets/sukhmandeepsinghbrar/housing-price-dataset/data

For this portion of the project, preliminary data preparation and exploratory data analysis was performed, as well as the creation of a baseline linear regression model.

#### Results
Explorator Data Analysis was conducted to identify five features which exhibit a strong positive correlation with price. It was also determined to drop the date, lat, and long columns from the dataset for the purpose of modeling, as these features were determined to be either unnecessary for the model, or not easily quantifiable. 

From this, a baseline linear regression model using a single feature, sqft_living (the living area size in square feet), was created. This model was used to predict the price of a house with 49% accuracy, according to the R^2 value of the model. 

#### Next steps
To improve the accuracy of the model, two approaches can be considered. The first is to include more features. We only looked at sqft_living, but as highlighted by our exploratory data analysis process, four other features exhibited a strong positive correlation with price. Including too many features does run the risk of overfitting the data by increasing model complexity, but a baseline model like this needs to be made more complex if our goal is to maximize predictive accuracy.

Furthermore, re-introducing the locational features (zipcode, lat, long) may help to increase the accuracy of the model. It may suffice to just include the zipcode, and to map these zipcodes to their respective locations in the U.S. This will introduce a categorical feature into our model, therefore increasing model complexity--but possibly helping us to arrive at a highly accurate model for predicting a house's price.

#### Outline of project

- Jupyter Notebook: https://github.com/udaymukkavilli/Capstone_InitialReportAndEDA/blob/main/Housing_EDA.ipynb


##### Contact and Further Information
Uday Mukkavilli

mukkavilliu@gmail.com

https://www.linkedin.com/in/umukkavilli/
