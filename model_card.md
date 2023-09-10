
# Model Description

Further details can be found in the original Model Card article: [link](https://arxiv.org/pdf/1810.03993.pdf).

## Overview of the Model
The model aims to predict if an individual earns more than $50,000 annually. It employs a GradientBoostingClassifier with specific hyperparameters tailored in scikit-learn. The hyperparameters were fine-tuned using GridSearchCV, with the best configurations being:
- Learning rate: 1.0
- Maximum depth: 5
- Minimum sample splits: 100
- Estimators count: 10

The model's architecture is stored in a pickle format in the designated model directory. 

## Purpose of the Model
This tool has been designed to estimate an individual's income category based on several characteristics. It's primarily intended for educational, academic, or research-related endeavors.

## Source of Training Data
The training data, known as the Census Income Dataset, was sourced from the UCI Machine Learning Repository [link](https://archive.ics.uci.edu/ml/datasets/census+income) in a CSV format. The dataset encompasses 32,561 entries with 15 distinct attributes.