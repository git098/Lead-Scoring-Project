# Lead Scoring Project

## Overview

This project aims to build a lead scoring system to identify potential customers who are most likely to convert into paying customers. The project analyzes lead data from various sources to predict the likelihood of conversion and help the marketing team prioritize leads effectively.

## Functionality

The project performs the following steps:

1.  **Data Loading and Cleaning:** Loads the lead data from a CSV file (`Lead_Data.csv`), handles missing values, and removes duplicate entries.
2.  **Exploratory Data Analysis (EDA):**
    *   Performs univariate and bivariate analysis to understand the distribution of variables and their relationship with the target variable (Converted).
    *   Identifies key factors that influence lead conversion.
3.  **Data Preparation:**
    *   Creates dummy variables for categorical features.
    *   Splits the data into training and testing sets.
    *   Scales numerical features using MinMaxScaler.
4.  **Model Building:**
    *   Uses Logistic Regression as the classification model.
    *   Employs Recursive Feature Elimination (RFE) to select the most relevant features.
    *   Uses Statsmodels to build and analyze the logistic regression model.
    *   Calculates Variance Inflation Factor (VIF) to check for multicollinearity.
5.  **Model Evaluation:**
    *   Evaluates the model's performance on the training and testing sets using metrics such as accuracy, sensitivity, and specificity.
    *   Plots the ROC curve to visualize the trade-off between sensitivity and specificity.
    *   Determines the optimal cutoff point for conversion probability.
6.  **Lead Scoring:**
    *   Assigns lead scores based on the predicted conversion probabilities.

## Installation

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/git098/Lead-Scoring-Project.git
    cd Lead-Scoring-Project
    ```

2.  **Install the dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

## Usage

1.  **Download the Lead Data dataset:**

    *   Download the `Lead_Data.csv` dataset and place it in the same directory as the notebook.
2.  **Run the Jupyter Notebook:**

    *   Open `Lead_Scoring_Project.ipynb` using Jupyter Notebook or JupyterLab.
    *   Run the cells in the notebook to perform the lead scoring analysis and build the prediction model.

## Requirements

*   Python 3.6+
*   `pandas`
*   `numpy`
*   `matplotlib`
*   `seaborn`
*   `scikit-learn`
*   `statsmodels`

## License

This project is licensed under the MIT License - see the `LICENSE` file for details.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.
