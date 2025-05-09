# California Housing Dataset Analysis

## Binder
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Marko-zu/tabular-playground/163b1db3c2e8ede6307292669139d28fd36d9a96?urlpath=lab%2Ftree%2Fhouse_price_prediction%2Fnotebooks%2Fhouse%20price%20prediction.ipynb)

This project delves into an analysis of a dataset generated by a deep learning model trained on the California housing dataset. While the relationships between variables mirror those of the original dataset, they are not identical. Our exploration spans three distinct datasets:

- **Training dataset**: Includes both predictor and dependent variables.
- **Testing dataset**: Contains only the predictor variables.
- **Original dataset**: Sourced from Scikit-learn, serving as the foundation for both the training and testing datasets.

## 🏠 Predicted Variable

The focus of our analysis is the **Median house value** for California districts, represented in hundreds of thousands of dollars ($100,000).

## 🔍 Independent Variables

We have access to a set of independent variables, including:

- **Median Income (MedInc)**: Median income within each block group.
- **Median House Age (HouseAge)**: Offers insight into the area's housing age distribution.
- **Average Rooms (AveRooms)**: Average number of rooms per household.
- **Average Bedrooms (AveBedrms)**: Average number of bedrooms per household.
- **Population**: Total population within a block group.
- **Average Household Members (AveOccup)**: Average number of individuals per household.
- **Latitude & Longitude**: Geographic coordinates (not used in this analysis).

## 📊 Model Evaluation Metric

The model's performance will be evaluated using the **R^2 metric**.

## 📈 Analysis Phases

### Phase 1: Data Examination

A thorough examination of the dataset, including:

- Identification and treatment of missing values.
- Assessment of feature distribution.
- Detection of outliers.
- Conduct of normality tests.

### Phase 2: Data Correction

Addressing anomalies to enhance the dataset's integrity and prepare for predictive modeling.

### Phase 3: Predictive Modeling

Development and implementation of a **Ridge Regression model** to predict the median house values.

## Setting Up the Environment

This project uses a Conda environment to manage dependencies. To recreate the environment, make sure you have Anaconda or Miniconda installed, then run the following command in your terminal:

```sh
conda env create -f environment.yml
