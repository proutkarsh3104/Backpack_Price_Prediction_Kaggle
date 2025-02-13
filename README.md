# Backpack Price Prediction - Kaggle Competition

This repository contains the code and documentation for a machine learning project aimed at predicting backpack prices. This project was developed for a Kaggle competition (replace with the actual competition name if applicable).

## Project Overview

The goal of this project is to build a model that accurately predicts the price of a backpack based on various features such as brand, material, size, compartments, and other characteristics. The model is trained using a dataset containing information about backpacks and their corresponding prices.

## Dataset

The dataset consists of two CSV files:

*   `train.csv`: Contains the training data, including backpack features and their prices.
*   `test.csv`: Contains the test data, with backpack features but without prices. The goal is to predict the prices for this dataset.

**Data Dictionary:**

| Feature               | Description                                                                                                                                        | Data Type  |
| --------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- |
| `id`                  | Unique identifier for each backpack.                                                                                                              | Numerical  |
| `Brand`               | The brand of the backpack (e.g., Jansport, Nike, Adidas).                                                                                         | Categorical |
| `Material`            | The primary material of the backpack (e.g., Leather, Canvas, Nylon).                                                                                | Categorical |
| `Size`                | The size of the backpack (e.g., Small, Medium, Large).                                                                                             | Categorical |
| `Compartments`        | The number of compartments in the backpack.                                                                                                        | Numerical  |
| `Laptop Compartment`  | Indicates whether the backpack has a dedicated laptop compartment (Yes/No).                                                                         | Binary     |
| `Waterproof`          | Indicates whether the backpack is waterproof (Yes/No).                                                                                              | Binary     |
| `Style`               | The style of the backpack (e.g., Tote, Messenger, Backpack).                                                                                     | Categorical |
| `Color`               | The color of the backpack.                                                                                                                          | Categorical |
| `Weight Capacity (kg)` | The maximum weight the backpack can carry, in kilograms.                                                                                        | Numerical  |
| `Price`               | The price of the backpack (target variable).                                                                                                    | Numerical  |
| `Material_Style`      | A feature combined from Material and Style.                                                                                               | Categorical |
| `Size_Compartments`| A feature combined from Size and Compartments.                                                                                               | Categorical |

The training dataset has some missing values (around 2-3% for most features, and 0.0385% for Weight Capacity), which are handled during the preprocessing stage.

## Dependencies

This project requires the following Python libraries:

*   pandas
*   numpy
*   scikit-learn
*   matplotlib
*   seaborn
*   xgboost
*   lightgbm
*   catboost

You can install these dependencies using pip:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn xgboost lightgbm catboost
