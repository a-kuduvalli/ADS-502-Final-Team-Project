# Spaceship Titanic: <br>Predicting Alternate Dimension Transportation
This project is a part of the ADS-502 course in the Applied Data Science Program at the University of San Diego.

**Project Status: [Active]**

## Installation
To use this project, first clone the repository on your device using the command below:

```bash
git init
git clone https://github.com/a-kuduvalli/ADS-502-Final-Team-Project.git
```

## Project Intro/Objective
The main purpose of this project is to predict which passengers were transported to an alternate dimension as the *Spaceship Titanic* came into collision with a spacetime anomaly in the year 2912. With records taken from the spaceship's damaged computer system, we will clean and explore the data, and build, validate, and compare multiple classification models that ultimately predict whether a passenger was transported or not. 

In doing so, we seek to build a reliable model that could aid rescue crews in identifying and retrieving the transported passengers. 

### Partners/Contributors

Teammates: Aishwarya Kuduvalli and Brandon Rodriguez-Andrade

Contact:
- akuduvalli@sandiego.edu
- brodriguezandrade@sandiego.edu

### Methods Used
- Data mining
- Data cleaning
- Feature extraction
- Data visualization
- Predictive modeling
- Machine learning
- Programming

### Technologies
- Python
- Jupyter Notebook
- Visual Studio Code
- pandas, numpy, matplotlib, scikit-learn, statsmodels

## Project Description
The dataset is sourced from Kaggle (the Spaceship Titanic competition), containing 8,693 labeled records. There are 13 independent variables, including passenger information (`PassengerID`, `Name`, `Age`, `HomePlanet`, `Destination`), `CryoSleep`, `Cabin`, and voyage spending (`VIP`, `RoomService`, `FoodCourt`, `ShoppingMall`, `Spa`, `VRDeck`). The target variable is the boolean attribute `PassengerId`, indicating whether a passenger was transported or not. 

### Pre-processing
- All passengers with a `CryoSleep` value of 'True' were assigned 0 for all amenities
- All passengers with no spending in amenities were assigned 'True' in `Cryosleep`
- Median (numerical variables) and mode (categorical variables) imputation for the remaining null values
- `Cabin` was split into `Deck`, `CabinNumber`, and `Side`
- Categorical variables were one-hot encoded

### Modelling
- Feature selection done manually, using results from decision-tree based importance bar graph and correlation heatmap
- Classifiers: Decision trees (CART and C5.0), Logistic Regression, Naïve Bayes, Random Forest
- Models evaluated using Accuracy, Error Rate, Sensitivity, Precision, and F1, F2, and F0.5 scores

Challenges faced: Kaggle's original Spaceship Titanic dataset included unlabeled test records and could not be used for model evaluation. For the purpose of this project, the training data (renamed as `spaceship.csv`) was partitioned using a 75/25 train-test split was used. Other challenges included grouping one-hot encoded dummy variables into original features for feature importance bar graph.

## License
[Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)

## Acknowledgements
- Professor An Tran, University of San Diego
- ADS-502: Fundamentals of Data Science, University of San Diego
- Kaggle - Spaceship Titanic competition dataset
