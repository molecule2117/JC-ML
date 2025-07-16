# Task 1: Spaceship Titanic
## Objective
The goal of this task is to explore and understand the Spaceship Titanic dataset, identifying patterns and potential features that may influence whether a passenger was "Transported" or not

## EDA
1. Check presence of duplicates
2. Missing value analysis:
   -Handled null values
3. Separated Cabin into deck , side and num
4. Converting categorical data to numerical data:
   -Usage of LabelEncoder on CryoSleep and VIP
   -Usage of OneHotEncoding on deck , side, HomePlanet and Destination
5. Plotted graphs to check for outliers , distribution and relation between different features
6. Created a new feature:
   -Amount = RoomService + FoodCourt + ShoppingMall + Spa + VRDeck.

## Preparing dataset for model application
1. Split the dataset into features and target
2. Train Test Split
3. Using RobustScaler to scale the features and to handle outliers

## Application of different models
1. Logistic Regression
   -Performed GridSearchCV (hyperparameter tuning)
   -Accuracy=80.39%
2. Linear SVC
   -Accuracy=78.26%
3. Naive Baye's
   -Accuracy=71.82%
4. KNN
   -Accuracy=79.3%
5. Decision Tree Classifier
   -Accuracy=76.42%
6. Random Forest Classifier
   -Accuracy=81.65%
7. Gradient Boosting Classifier
   -Accuracy=81.65%
8. AdaBoost Classifier
   -Accuracy=80.79%
9. XGBoost Classifier
   -Accuracy=82.06%

## Hyperparameter Tuning
-Usage of RandomizedSearch CV on Random Forest Classifier and XGBoost
-We get an accuracy of 81.94% and 82.806% respectively

### XG Boost has the best performance

