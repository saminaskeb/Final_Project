![](UTA-DataScience-Logo.png)

# Mushroom Classification

This project focuses on classifying mushrooms as either edible or poisonous using the Mushroom Classification Dataset from [Kaggle](https://www.kaggle.com/datasets/uciml/mushroom-classification). Using machine learning, the goal was to develop an accurate model to classify mushrooms based on their features.

## Overview

The dataset includes 8,124 entries with 22 categorical attributes such as cap color, gill attachment, and odor. The target variable (`class`) indicates if a mushroom is edible (`e`) or poisonous (`p`). Since the dataset is balanced, it's ideal for binary classification tasks.

After experimenting with multiple models, the Random Forest classifier was chosen due to its perfect performance and ability to highlight feature importance.


## Summary of Workdone

Include only the sections that are relevant an appropriate.

### Data

* Data:
  * Type: For example
    * Input: medical images (1000x1000 pixel jpegs), CSV file: image filename -> diagnosis
    * Input: CSV file of features, output: signal/background flag in 1st column.
  * Size: How much data?
  * Instances (Train, Test, Validation Split): how many data points? Ex: 1000 patients for training, 200 for testing, none for validation

#### Preprocessing / Clean up

* Describe any manipulations you performed to the data.

#### Data Visualization

Show a few visualization of the data and say a few words about what you see.

### Problem Formulation

* Define:
  * Input / Output
  * Models
    * Describe the different models you tried and why.
  * Loss, Optimizer, other Hyperparameters.

### Training

* Describe the training:
  * How you trained: software and hardware.
  * How did training take.
  * Training curves (loss vs epoch for test/train).
  * How did you decide to stop training.
  * Any difficulties? How did you resolve them?

### Performance Comparison

* Clearly define the key performance metric(s).
* Show/compare results in one table.
* Show one (or few) visualization(s) of results, for example ROC curves.

### Conclusions

This project demonstrates the effectiveness of ensemble methods like Random Forest in handling classification tasks with categorical data. The success came from:
- Careful data preparation
- Visualization-driven insights
- Rigorous model testing

### Future Work
Ideas for further development:
- Fine-tune hyperparameters for better generalization
- Apply workflow to similar biological datasets

## How to reproduce results

1. Run `Project_Code.ipynb` for data preparation and model training.
2. Follow notebook cells for model comparisons and evaluations.
3. Use `submission.csv` for result review or external validation.

### Overview of files in repository

- `Project_Code.ipynb`: Full workflow
- `submission.csv`: Prediction file
- `README.md`: Documentation 

### Software Setup
Required Packages:
- pandas
- scikit-learn
- matplotlib
- 
## Citations

- Mushroom Classification Dataset: [Kaggle](https://www.kaggle.com/datasets/uciml/mushroom-classification).







