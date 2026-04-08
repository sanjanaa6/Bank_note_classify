# Banknote Authentication Classifier

## Overview
This project implements a machine learning model to classify banknotes as authentic or forged using the Banknote Authentication dataset. The model uses a Random Forest Classifier to predict the authenticity based on features extracted from images of banknotes.

## Dataset
The dataset used is the Banknote Authentication dataset, which contains 1372 instances with 4 features:
- Variance of Wavelet Transformed image
- Skewness of Wavelet Transformed image
- Kurtosis of Wavelet Transformed image
- Entropy of image

The target variable is binary: 0 for authentic, 1 for forged.

## Requirements
- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

Install the required packages using:
```
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Usage
1. Ensure the `Banknote_Authentication.csv` file is in the same directory as the notebook.
2. Open the `BNC.ipynb` notebook in Jupyter or VS Code.
3. Run the cells in order to perform exploratory data analysis, train the model, and evaluate its performance.

## Model Performance
The Random Forest model achieves high accuracy on the test set. Key metrics include:
- Accuracy: ~99%
- Precision, Recall, and Specificity are also evaluated.
- ROC-AUC curve and confusion matrix are visualized.

## Features
- Exploratory Data Analysis (EDA) with visualizations
- Feature correlation analysis
- Model training and evaluation
- Performance metrics and plots

## License
This project is for educational purposes.