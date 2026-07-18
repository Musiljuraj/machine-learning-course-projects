# Machine Learning Course Projects

This repository contains two machine-learning projects completed during my studies in Computational and Applied Mathematics at VŠB – Technical University of Ostrava.

The projects demonstrate two complementary areas of machine learning:

* **unsupervised learning** applied to international CO₂-emissions data;
* **supervised classification** applied to customer-churn prediction.

Both projects are implemented as Jupyter notebooks containing data preparation, exploratory analysis, model development, visualizations, evaluation, and interpretation of results.

## Project Overview

| Project                                                                                                            | Learning Type         | Main Methods                                                                                                           | Main Outcome                                                                                                                |
| ------------------------------------------------------------------------------------------------------------------ | --------------------- | ---------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------- |
| [CO₂ emissions clustering and analysis](./01-co2-emissions-clustering-and-analysis/co2-emissions-clustering.ipynb) | Unsupervised learning | Data preprocessing, feature engineering, K-means, hierarchical clustering, PCA, silhouette analysis                    | Identification and interpretation of groups of countries with different economic and emissions characteristics              |
| [Bank customer churn classification](./02-bank-customer-churn-classification/customer-churn-classification.ipynb)  | Supervised learning   | Preprocessing pipelines, stratified cross-validation, Decision Tree, k-NN, Gaussian Naive Bayes, hyperparameter search | Comparison of classification models, with a tuned Decision Tree achieving mean cross-validated recall of approximately 0.91 |

## 1. CO₂ Emissions Clustering and Analysis

[Open the project folder](./01-co2-emissions-clustering-and-analysis)

This project investigates whether countries can be grouped according to their economic structure, energy use, and CO₂-emissions characteristics.

The analysis includes:

* cleaning and merging international emissions data;
* creation and selection of derived indicators;
* exploratory data analysis and correlation analysis;
* data standardization;
* selection of a suitable number of clusters;
* K-means clustering;
* hierarchical agglomerative clustering;
* PCA visualization;
* comparison and interpretation of the resulting country groups;
* analysis of production-based and consumption-based emissions trends.

The project connects machine-learning methods with environmental and economic interpretation. It also discusses the limitations of clustering results and distinguishes descriptive patterns from causal conclusions.

[Open the Jupyter notebook](./01-co2-emissions-clustering-and-analysis/co2-emissions-clustering.ipynb)

## 2. Bank Customer Churn Classification

[Open the project folder](./02-bank-customer-churn-classification)

This project develops and compares classification models for identifying bank customers who are likely to leave.

The workflow includes:

* exploratory analysis of customer data;
* data-quality and duplicate checks;
* removal of unnecessary or potentially misleading variables;
* encoding of categorical features;
* scaling of numerical features;
* preprocessing with `Pipeline` and `ColumnTransformer`;
* stratified ten-fold cross-validation;
* comparison of Decision Tree, k-nearest neighbours, and Gaussian Naive Bayes classifiers;
* treatment of class imbalance;
* hyperparameter tuning with `GridSearchCV`;
* selection of recall as the principal evaluation metric.

The tuned Decision Tree achieved a mean cross-validated recall of approximately **0.91** during hyperparameter selection. This result reflects cross-validation used for model tuning rather than evaluation on a separate independent test set.

[Open the Jupyter notebook](./02-bank-customer-churn-classification/customer-churn-classification.ipynb)

## Skills Demonstrated

* data cleaning and preprocessing;
* exploratory data analysis;
* feature engineering and feature selection;
* handling of numerical and categorical variables;
* unsupervised clustering;
* dimensionality reduction and visualization;
* supervised classification;
* class-imbalance analysis;
* cross-validation;
* hyperparameter optimization;
* selection and interpretation of evaluation metrics;
* critical interpretation of model results and limitations.

## Technologies

* Python
* Jupyter Notebook
* pandas
* NumPy
* Matplotlib
* Seaborn
* scikit-learn

## Repository Structure

```text
machine-learning-course-projects/
├── 01-co2-emissions-clustering-and-analysis/
│   ├── co2-emissions-clustering.ipynb
│   ├── Data.csv
│   └── Regions.xlsx
│
├── 02-bank-customer-churn-classification/
│   ├── customer-churn-classification.ipynb
│   └── BankChurners.csv
│
├── .gitignore
└── README.md
```

Each project is independent and uses its own dataset. The notebooks contain the detailed methodology, source code, visualizations, results, and discussion.

## Academic Context

The projects were completed for the course **Fundamentals of Machine Learning** as part of the **Computational and Applied Mathematics** study programme at **VŠB – Technical University of Ostrava**.

They are presented as academic demonstrations of practical machine-learning workflows and are not intended to represent production-ready systems.
