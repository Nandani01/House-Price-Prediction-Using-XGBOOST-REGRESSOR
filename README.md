California Housing Price Prediction using XGBoost
Project Overview
This project demonstrates how to build a regression model using XGBoost to predict California housing prices based on the California Housing dataset.
The process involves data loading, exploration, preprocessing, model training, and evaluation.

Dataset
The dataset used is the California Housing dataset, available through sklearn.datasets.fetch_california_housing. It contains 20,640 instances with 8 numerical features and a target variable (median house value).

Attribute Information:

MedInc: Median income in block group
HouseAge: Median house age in block group
AveRooms: Average number of rooms per household
AveBedrms: Average number of bedrooms per household
Population: Block group population
AveOccup: Average number of household members
Latitude: Block group latitude
Longitude: Block group longitude
The target variable, MedHouseVal, is the median house value for California districts, expressed in hundreds of thousands of dollars ($100,000).

Dependencies
The following libraries are used in this project:

numpy
pandas
matplotlib
seaborn
sklearn
xgboost

Project Steps
1. Importing Dependencies: Import necessary libraries for data manipulation, visualization, and model building.
2. Loading the Dataset: Load the California Housing dataset using fetch_california_housing.
3. Loading to Pandas DataFrame: Convert the dataset into a pandas DataFrame for easier manipulation and analysis. The target variable (MedHouseVal) is added as a new column named House_price.
4. Data Exploration:
Display the first 5 rows of the DataFrame to get a glimpse of the data.
Check the shape of the DataFrame to understand the number of rows and columns.
Check for any missing values in the dataset.
Generate statistical measures of the dataset to understand the distribution and characteristics of the features.
Correlation Analysis: Calculate and visualize the correlation matrix of the features and the target variable using a heatmap to understand the relationships between them.
Splitting Data: Separate the features (X) and the target variable (Y). Split the data into training and testing sets (80% for training, 20% for testing) using train_test_split.

6. Model Training:
   
Load the XGBoost Regressor model.
Train the model using the training data (X_train and Y_train).

6. Model Evaluation:
Prediction on Training Data: Make predictions on the training data using the trained model.
Evaluate the model's performance on the training data using R-squared error and Mean Absolute Error.
Visualize the actual prices versus predicted prices for the training data using a scatter plot.
Prediction on Test Data: Make predictions on the unseen test data using the trained model.
Evaluate the model's performance on the test data using R-squared error and Mean Absolute Error.
Visualize the actual prices versus predicted prices for the test data using a scatter plot.
Single Data Point Prediction: Demonstrate how to make a prediction on a single data point from the test set and compare the predicted price with the actual price.

7. Results
The model's performance is evaluated using R-squared error and Mean Absolute Error on both the training and test datasets. The scatter plots visualize how well the predicted prices align with the actual prices. The prediction on a single test data point provides a concrete example of the model's output.

8. Conclusion
This project successfully demonstrates the process of building a house price prediction model using XGBoost on the California Housing dataset. The evaluation metrics and visualizations provide insights into the model's accuracy and performance.
