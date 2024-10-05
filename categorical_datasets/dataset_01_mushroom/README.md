# Mushroom Dataset - Modified

This folder contains a modified version of the Mushroom dataset from the UCI Machine Learning Repository. The dataset has been modified by:

- Removing records with missing data.
- Adding a new column `is_outlier`, where:
  - `1` indicates the record is an outlier.
  - `0` indicates the record is not an outlier.

## Dataset Information

- **Source**: UCI Machine Learning Repository: [https://doi.org/10.24432/C5959T](https://doi.org/10.24432/C5959T)
- **Modifications**:
  - Removed rows with missing data.
  - Added outlier information 
- **License**: [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/)

## Creation and Purpose

This modified version of the Mushroom dataset draws inspiration from advancements in analytical techniques and research needs within the fields of natural sciences and food safety. The original dataset, which included 8,124 cases and 22 attributes such as cap shape, cap surface, cap color, presence of bruises, odor, etc., classified mushrooms as definitely edible, definitely poisonous, or of undetermined edibility—with the latter treated as definitely poisonous. In this new version, records with missing data were removed, and a `is_outlier` column was introduced to better identify anomalies, which were treated as exceptions in the original data analysis. A significant portion of poisonous mushroom samples was removed, leaving only 42 samples, which constituted 0.988% of all samples, thereby reducing the total number of samples to 4,250. These 42 samples of poisonous mushrooms now represent clearly defined anomalies in the dataset, enabling their realistic and true analysis, unlike previous studies where anomalies were synthetically generated. This modification facilitates more precise predictive modeling and data analysis in a more controlled environment, eliminating the need for data normalization thanks to the application of one-hot encoding.

Furthermore, the dataset named `mushroom_real_with_is_outlier_4250_42.csv` has been divided into a training part and a testing part to facilitate different phases of machine learning experimentation. The dataset is split into `mushroom_real_train_data_with_labels_4250_42_70.csv`, which contains 70% of the data for training purposes, and `mushroom_real_test_data_with_labels_4250_42_30.csv`, which comprises 30% of the data for testing and validation. This separation helps in evaluating the model’s performance on unseen data, ensuring a robust and effective training process.

## How to Use

- Download the `data.csv` file in this folder.
- The `is_outlier` column helps in identifying records that have been classified as outliers.
