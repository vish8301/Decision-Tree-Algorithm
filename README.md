# Decision Tree Classification Algorithm
This project was an assignment in one of my ML classes.

## Introduction
This project involves the development and evaluation of a Decision Tree Classifier to predict income levels based on census data. Using data from the Census Bureau, which includes seven demographic variables, we aim to classify individuals into two income categories: ">50K" and "<=50K". This notebook guides you through data preparation, analysis, building decision tree models, performance evaluation, tuning, and visualization.

## Data Source
The dataset is hosted on GitHub and can be directly accessed through this link: <br>
https://github.com/ArinB/MSBA-CA-03-Decision-Trees/blob/master/census_data.csv?raw=true <br>
It features demographic information across 48,842 instances and is pre-split into training and testing datasets.
- Number of target classes: 2: '>50K' and '<=50K' (labels: 1, 0)
- Number of attributes (Columns): 7
- Number of instances (Rows): 48,842


## Installation and Setup
- Clone or download this project repository to your local machine.
- Ensure Python and pip are installed.
- Create and activate a virtual environment: python -m venv venv
  - Windows: venv\Scripts\activate
  - macOS/Linux: source venv/bin/activate
- Install the following packages:
```bash
pip install pandas scikit-learn matplotlib numpy graphviz
```

### Project Tasks
- Data Quality Analysis: Identification and correction of data quality issues.
- Decision Tree Modeling: Utilize DecisionTreeClassifier from scikit-learn to create models.
- Performance Evaluation: Compute metrics like accuracy, precision, recall, and F1 score.
- Hyperparameter Tuning: Experiment with different settings to find the most effective decision tree configuration.
- Visualization: Use GraphViz to visualize the optimal decision tree.


### Conclusion and Analysis
The best model had the following hyperparameters:
- Split Criteria: ‘Gini Impurity’
- Minimum Sample Leaf: 20
- Maximum Features: None
- Maximum Depth: 10

Accuracy of the best model: 0.8460 (84.60%)

The decision tree is fully grown and is pretty complex. There is a chance of overfitting.
