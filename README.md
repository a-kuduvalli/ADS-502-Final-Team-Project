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
- Feature engineering
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
The dataset is sourced from Kaggle (the Spaceship Titanic competition), containing about 8,700 training records and 4,300 training test records. There are 13 independent variables, including passenger information (`PassengerID`, `Name`, `Age`, `HomePlanet`, `Destination`), `CryoSleep`, `Cabin`, and voyage spending (`VIP`, `RoomService`, `FoodCourt`, `ShoppingMall`, `Spa`, `VRDeck`). The target variable is the boolean attribute `PassengerId`, indicating whether a passenger was transported or not. 

### Pre-processing
- Cryosleep status 
- Median (numerical variables) and mode (categorical variables) imputation was used for the remaining null values
- `Cabin` was split into `Deck`, `CabinNumber`, and `Side`
- Categorical variables were one-hot encoded
- StandardScaler used to 
