# credit_risk_evaluator
A machine learning model that attempts to predict whether a loan from LendingClub will become high risk or not.

## Code used:
Python (Jupyter Notebook) - Primary code is called Credit Risk Evaluator.ipynb.

## Libraries used:
- numpy
- pandas
- pathlib
	- Path
- sklearn.preprocessing
	- StandardScaler
	- LabelEncoder
- sklearn.metrics
	- accuracy_score
- sklearn.utils
	- resample
- sklearn.linear_model
	- LogisticRegression
- sklearn.tree
	- DecisionTreeClassifier
- sklearn.ensemble
	- RandomForestClassifier

## Process:
- Using GenerateData.ipynb (located in Resources/Generator folder) pull 2019 data for Q1-Q4 and 2020 data for Q1 then create 2019loans.csv and 2020Q1loans.csv in Resources folder
- Pull in 2019loans.csv data to use as training data and 2020Q1loans.csv as testing data
- Convert categorical data to numeric and separate target feature for training and testing data
- Add missing variables to testing set
- Create and compare a Logistic Regression model and a Random Forest Classifier model for the data
- Scale the data using StandardScaler and create and compare the two models again

## Results:
The scaled data improved the Logistic Regression model and made it the best model when compairing Testing Data Scores. When comparing Training Data Scores, the Random Forest Classifier model was better, and the Random Forest Classifier model had a better Testing Data Score when not scaled compared to the Logistic Regression model when not scaled. If scaling the data and looking toward the Testing Data Scores for 2020, the scaled Logistic Regression model was the best.

## Contact:
Joseph March: josephmarch@gmail.com