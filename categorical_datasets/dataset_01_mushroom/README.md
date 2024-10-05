# Mushroom Dataset - Modified

This folder contains a modified version of the Mushroom dataset from the UCI Machine Learning Repository, tailored to enhance machine learning model performance and anomaly detection in natural sciences and food safety studies. The modifications are designed to facilitate advanced data analysis and training processes.

## Dataset Information

- **Source**: UCI Machine Learning Repository: [https://doi.org/10.24432/C5959T](https://doi.org/10.24432/C5959T)
- **Modifications**:
  - Removed rows with missing data to ensure data quality.
  - Added `is_outlier` column to classify and identify anomalies clearly:
    - `1` indicates the record is an outlier.
    - `0` indicates the record is not an outlier.
- **License**: [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)

## Creation and Purpose

The original dataset featured 8,124 cases and attributes like cap shape, cap surface, cap color, presence of bruises, and odor, categorizing mushrooms based on edibility. This modified version removes records with missing data and introduces an `is_outlier` column. By selectively retaining only 42 samples of poisonous mushrooms, reducing the total sample count to 4,250, this dataset allows for a more accurate and realistic analysis of clearly defined anomalies, thus facilitating robust predictive modeling.

## Dataset Division

The dataset `mushroom_real_with_is_outlier_4250_42.csv` is divided into training and testing parts to support various machine learning phases:
- `mushroom_real_train_data_with_labels_4250_42_70.csv` contains 70% of the data for training.
- `mushroom_real_test_data_with_labels_4250_42_30.csv` contains 30% for testing and validation.

This structured division aids in evaluating model performance on unseen data, ensuring an effective training cycle.

## How to Use

- Download the appropriate dataset files from this folder:
  - `mushroom_real_with_is_outlier_4250_42.csv` is the complete modified dataset, which includes all the samples with the `is_outlier` column indicating whether each record is considered an outlier. This file can be used for comprehensive data analysis or for creating custom splits for training, testing, and validation.
  - `mushroom_real_train_data_with_labels_4250_42_70.csv` should be used for training your models. It contains 70% of the data, specifically selected for training purposes.
  - `mushroom_real_test_data_with_labels_4250_42_30.csv` should be used for testing and validating your models. It contains 30% of the data, specifically selected for testing and validation purposes.

These files are prepared to support various phases of machine learning experimentation, allowing effective training, testing, and validation of models using accurately labeled data. This flexibility facilitates a comprehensive approach to machine learning model development, ensuring that all aspects of the dataset are utilized according to user needs.

- Utilize the `is_outlier` column to identify records classified as outliers, enhancing model training and analysis.
