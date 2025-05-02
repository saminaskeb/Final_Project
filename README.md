![](UTA-DataScience-Logo.png)

# Mushroom Classification

This project focuses on classifying mushrooms as either edible or poisonous using the Mushroom Classification Dataset from [Kaggle](https://www.kaggle.com/datasets/uciml/mushroom-classification). Using machine learning, the goal was to develop an accurate model to classify mushrooms based on their features.

## Overview

The dataset includes 8,124 entries with 22 categorical attributes such as cap color, gill attachment, and odor. The target variable (`class`) indicates if a mushroom is edible (`e`) or poisonous (`p`). Since the dataset is balanced, it's ideal for binary classification tasks.

After experimenting with multiple models, the Random Forest classifier was chosen due to its perfect performance and ability to highlight feature importance.


## Summary of Workdone

## Key Steps

### Exploratory Data Analysis (EDA)

Important findings:
- `veil-type` had no variability and was excluded.
- Missing values in `stalk-root` (represented as `?`) were replaced with a new category called `"unknown"`.

Class distribution appeared nearly even:

![image](https://github.com/user-attachments/assets/9db125c5-56a2-4d08-8672-90d43732e8f0)


### Data Cleaning & Preprocessing

Steps involved:
- All input features were one-hot encoded.
- The target column was mapped to `0` (edible) and `1` (poisonous).

### Visual Analysis

To better understand the dataset, key visualizations were created:

- **Feature Importance:** A Random Forest model helped identify the 15 most influential features, with `odor` and `gill-size` ranking highest.

![Top Features Placeholder](./images/top_feature_importance.png)

- **Odor Analysis:** The `odor` feature displayed a clear distinction between the two mushroom classes.

![Odor Feature Plot Placeholder](./images/odor_feature_plot.png)

### Problem Setup

This task was treated as a standard binary classification problem:
- **Input:** Processed features after encoding
- **Output:** `0` (edible) or `1` (poisonous)

Evaluated models:
- Logistic Regression
- Random Forest
- K-Nearest Neighbors (KNN)
- Support Vector Machines (SVM)

### Model Training & Comparison

Models were trained using 70% of the data, with 15% reserved for validation. Results:

| Model                  | Validation Accuracy | Test Accuracy | Notes                                     |
|------------------------|---------------------|---------------|-------------------------------------------|
| Logistic Regression    | 99.75%              | 99.75%        | Interpretable and efficient               |
| Random Forest          | 100%                | 100%          | Best performance + feature insights       |
| K-Nearest Neighbors    | 100%                | 100%          | Slower with larger datasets               |
| Support Vector Machines| 100%                | 100%          | Accurate, less transparent                |

**Final choice:** Random Forest — for its blend of accuracy and interpretability.

### Final Evaluation

The selected model, Random Forest, achieved flawless accuracy on the test set — confirming its generalization capability.

### Submission Output

The final predictions are stored in `submission.csv`. Sample:

| Index | Prediction |
|-------|------------|
| 0     | 1          |
| 1     | 0          |
| 2     | 1          |
| ...   | ...        |

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







