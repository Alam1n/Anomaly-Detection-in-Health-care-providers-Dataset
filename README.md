# Anomaly-Detection-in-Health-care-providers-Dataset
This project involves detecting anomalies in healthcare providers' datasets using the Isolation Forest algorithm. The Isolation Forest algorithm is particularly effective for identifying outliers or anomalies in high-dimensional datasets.

Link to the dataset on kaggle: [Healthcare Providers Data For Anomaly Detection](https://www.kaggle.com/datasets/tamilsel/healthcare-providers-data)

### Key Features
* Model: Isolation Forest
* Contamination: 0.01 (Assumed proportion of outliers in the dataset)
* Number of Estimators: 50 (Number of trees in the forest)
* Random State: 42 (Seed for reproducibility)
### Model Architecture
The Isolation Forest algorithm operates on the principle of isolating anomalies rather than profiling normal data. The key components of the architecture are:

* Isolation Forest: An ensemble-based algorithm that isolates observations by randomly selecting a feature and then randomly selecting a split value between the maximum and minimum values of the selected feature. Anomalies are expected to be isolated closer to the root of the tree, requiring fewer splits to isolate them.
Training Process
* Initialization: The Isolation Forest model is initialized with the following parameters:

* contamination: Specifies the proportion of outliers in the dataset.
* n_estimators: The number of trees in the forest.
* random_state: A seed for reproducibility of results.
* Training: The model is trained on the scaled dataset (df_scaled), which has been preprocessed to ensure consistency and comparability of features.

This model is effective for detecting outliers in the dataset by identifying data points that differ significantly from the majority of the data.

