# 🛠 Machine Failure Prediction Analysis

This project involves analyzing and modeling a machine failure dataset. We'll be working with a dataset derived from a deep learning model trained on the Machine Failure Predictions dataset. We'll measure our success using the area under the ROC curve, comparing our predicted probabilities to the observed targets.

## 📝 Features Description

Diving into the core of our analysis, we focus on the following features as detailed in the AI4I 2020 Predictive Maintenance Dataset documentation:

- **`id`**: A unique identifier for each data entry in the dataset. While essential for tracking individual data points, it does not play a role in our predictive model.

- **`Product ID`**: Serves as an identifier for specific products or machines, which may reveal patterns in machine reliability or proneness to failure.

- **`Type`**: The type or category of machine, potentially influencing its failure likelihood. Variations across different machine types could yield differing failure rates.

- **`Air temperature [K]`** and **`Process temperature [K]`**: Key indicators of operational conditions, with elevated temperatures often signaling increased risk of machine failure.

- **`Rotational speed [rpm]`**: High operational speeds may augment the risk of failure, making this an important factor to monitor.

- **`Torque [Nm]`**: The torque applied during machine operation can lead to wear and tear, potentially culminating in failure.

- **`Tool wear [min]`**: Reflects the extent of tool use, with increased durations often correlating with heightened failure risk.

- **`Machine failure`**: Our pivotal binary target variable, denoting the occurrence (or absence) of machine failure.

Furthermore, we delve into specific types of failures, each represented as a binary indicator:
- **`TWF`** (Tool Wear Failure),
- **`HDF`** (Heat Dissipation Failure),
- **`PWF`** (Power Failure),
- **`OSF`** (Overstrain Failure),
- **`RNF`** (Random Failure).

If any of these conditions are met, the 'machine failure' flag is raised, signaling the end of functionality.

## 📊 Model Evaluation Metric

The model's performance will be evaluated using area under the ROC curve**.

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

Development and implementation of a **Logistic Regression model** to predict the probability of machine failure.

## Setting Up the Environment

This project uses a Conda environment to manage dependencies. To recreate the environment, make sure you have Anaconda or Miniconda installed, then run the following command in your terminal:

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Marko-zu/tabular-playground/main?labpath=%2Ftabular-playground%2F)


```sh
conda env create -f environment.yml
