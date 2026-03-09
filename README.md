# Spaceship Titanic

## Overview

This project explores the Kaggle **Spaceship Titanic** machine learning competition. The goal is to predict whether a passenger was transported to another dimension based on demographic, travel, and onboard spending features.

This repository contains a complete end to end workflow using Python and scikit learn, including data cleaning, feature engineering, model training, model evaluation, and project presentation materials.

## Project Goal

The objective of this project is to build a classification model that predicts the `Transported` outcome for each passenger.

## Dataset

The project uses the Kaggle Spaceship Titanic dataset, which includes features such as:

- HomePlanet
- CryoSleep
- Cabin
- Destination
- Age
- VIP
- RoomService
- FoodCourt
- ShoppingMall
- Spa
- VRDeck

Target variable:

- `Transported`

## Workflow

The notebook follows this machine learning pipeline:

1. Import libraries and load the dataset
2. Clean missing values
3. Split the `Cabin` column into:
   - Deck
   - CabinNum
   - Side
4. Prepare numeric and categorical features
5. Train and validate multiple classification models
6. Compare results using Accuracy and AUC

## Models Used

The following models were tested:

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier

## Results

Validation performance from the notebook:

| Model | Accuracy | AUC |
|-------|----------|-----|
| Logistic Regression | 0.7918 | 0.8815 |
| Decision Tree | 0.7838 | 0.8587 |
| Random Forest | 0.8085 | 0.8931 |

### Best Model
The **Random Forest** model achieved the best overall validation performance in this project.

## Repository Contents

- `Spaceship_Titanic.ipynb`  
  Main notebook containing preprocessing, modeling, and evaluation

- `Spaceship Titanic_Project Slides_Results.pdf`  
  Presentation slides summarizing the project and results

- `README.md`  
  Project documentation

## Tech Stack

- Python
- pandas
- numpy
- matplotlib
- seaborn
- scikit learn
- Jupyter Notebook

## How to Run

1. Clone this repository
2. Install dependencies
3. Open the notebook in Jupyter
4. Update dataset file paths if needed

```bash
pip install pandas numpy matplotlib seaborn scikit-learn notebook
jupyter notebook
```

Notes:
The current notebook uses local file paths for the training and test CSV files. To run this project on another machine, update the file paths to match your local dataset location.

Future Improvements:
Possible next steps for this project include:
Hyperparameter tuning
Cross validation
Additional feature engineering
Kaggle submission optimization
Exporting the final prediction pipeline




