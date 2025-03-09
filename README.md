# Titanic Survival Prediction 
## Project Overview
This project analyzes the Titanic dataset to explore factors that influenced passenger survival and builds a machine learning model to predict survival outcomes.

## Table of content
- Dataset
- Project Structure
- Requirements
- Result

## Dataset
The dataset contains information about the passanger such as:
- PassengerId
- Survived
- Pclass
- Name
- Sex
- Age
- Sibsp
- Parch
- Ticket
- Fare
- Cabin
- Embarked

## Project Structure
The project is divided into two sub-Tasks:
### Task 1: Exploratory Data Analysis (EDA)
The EDA provides insights into the dataset by:

- Generating basic statistical summaries of the features
- Visualizing key relationships and patterns
- Analyzing specific trends including:
      - Impact of passenger class on survival rates
      - Influence of age and gender on survival chances
      - Effect of port of embarkation on survival
      - Relationship between family size and survival

Key visualizations include:

- Count plots for categorical variables
- Histograms for continuous variables
- Correlation matrix for numerical features
- Survival rate breakdowns by different passenger characteristics
  
### Task 2: Machine Learning Model
The machine learning component includes:
Data Preprocessing
- Handling missing values using median imputation for numerical features and mode imputation for categorical features
- Encoding categorical variables using one-hot encoding
- Scaling numerical features

Model Development
- Base model: Random Forest Classifier
- Enhanced model with feature engineering
- Hyperparameter-tuned model using GridSearchCV

Feature Engineering 
Additional Features created:
- Title extracted from passenger names
- IsAlone flag for solo travelers
- Family size (SibSp + Parch + 1)
- Fare per person
- Deck extracted from cabin information

Hyperparameter Tuning 
Grid search for optimal hyperparameters including:
- Number of estimators
- Maximum depth
- Minimum samples per split
- Minimum samples per leaf

Model Evaluation
Models are evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix
- Classification report
- Feature importance analysis

### Requirements
- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

### Results
The analysis revealed several key insights:

- First-class passengers had significantly higher survival rates
- Women and children were prioritized for survival
- Passengers from Cherbourg had better survival chances
- Family size influenced survival probability, with mid-sized families (2-4 members) showing better outcomes
- Passenger titles (indicating social status) correlated with survival rates
