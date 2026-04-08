# Banknote Authentication Classifier

## Overview
This project implements a machine learning model to classify banknotes as authentic or forged using the Banknote Authentication dataset. The model uses a Random Forest Classifier to predict the authenticity based on features extracted from images of banknotes. This is a binary classification problem where we aim to distinguish between genuine and counterfeit banknotes.

## Dataset
The dataset used is the Banknote Authentication dataset from the UCI Machine Learning Repository. It contains 1372 instances with 5 attributes:
- Variance of Wavelet Transformed image (continuous)
- Skewness of Wavelet Transformed image (continuous)
- Kurtosis of Wavelet Transformed image (continuous)
- Entropy of image (continuous)
- Class (target): 0 for authentic, 1 for forged

The dataset is derived from images that were taken from genuine and forged banknote-like specimens. For digitization, an industrial camera was used, and the images were processed using Wavelet Transform tool to extract features.

### Dataset Source
Download the dataset from: https://archive.ics.uci.edu/ml/machine-learning-databases/00267/data_banknote_authentication.txt

Or use the provided download command:
```
Invoke-WebRequest -Uri "https://archive.ics.uci.edu/ml/machine-learning-databases/00267/data_banknote_authentication.txt" -OutFile "Banknote_Authentication.csv"
```

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

## Installation and Setup
1. Clone or download this repository.
2. Navigate to the project directory.
3. Install the required dependencies as listed above.
4. Download the dataset as described in the Dataset section.

## Usage
1. Ensure the `Banknote_Authentication.csv` file is in the same directory as the notebook.
2. Open the `BNC.ipynb` Jupyter notebook in Jupyter Notebook, JupyterLab, or VS Code.
3. Run the cells sequentially to:
   - Load and explore the data
   - Perform exploratory data analysis (EDA)
   - Train the Random Forest model
   - Evaluate the model's performance

## Data Exploration
The notebook includes comprehensive data exploration:
- Basic statistics and data types
- Class distribution visualization
- Correlation heatmap between features
- Pair plots to visualize feature relationships
- Feature importance analysis

## Model Architecture
- **Algorithm**: Random Forest Classifier
- **Parameters**:
  - n_estimators: 100
  - random_state: 42 (for reproducibility)
- **Training**: 80% of data used for training, 20% for testing
- **Features**: All 4 continuous features are used as input

## Model Performance
The Random Forest model achieves high accuracy on the test set. Key metrics include:
- Accuracy: Approximately 99%
- Precision, Recall, and Specificity are calculated
- ROC-AUC curve and confusion matrix are visualized
- Feature importance is analyzed and plotted

### Evaluation Metrics
- Confusion Matrix
- Classification Report (Precision, Recall, F1-Score)
- ROC Curve and AUC Score
- Feature Importance Plot

## Results
After training and evaluation, the model demonstrates excellent performance in classifying banknotes. The high accuracy indicates that the features extracted from the wavelet transform are effective discriminators between authentic and forged banknotes.

## Features
- Exploratory Data Analysis (EDA) with visualizations
- Feature correlation analysis
- Model training and evaluation
- Performance metrics and plots
- Confusion matrix visualization
- ROC curve analysis
- Feature importance ranking

## Project Structure
- `BNC.ipynb`: Main Jupyter notebook containing the analysis and model
- `README.md`: This file with project documentation
- `Banknote_Authentication.csv`: Dataset file (to be downloaded)

## Contributing
This is an educational project. Feel free to fork and modify for your own learning purposes.

## License
This project is for educational purposes only.

## Author
Sanjana Singh

## Date
April 2026