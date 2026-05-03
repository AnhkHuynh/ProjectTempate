![](UTA-DataScience-Logo.png)

# Project Title

* **One Sentence Summary**: This repository applies machine learning models to classify mushrooms as edible or poisonous using the Kaggle Mushroom Classification dataset.
* https://www.kaggle.com/datasets/uciml/mushroom-classification

## Overview

* This section could contain a short paragraph which include the following:
  * **Definition of the tasks / challenge**  Ex: The task, as defined by the Kaggle challenge is to use a time series of 12 features, sampled daily for 1 month, to predict the next day's price of a stock.
  * **Your approach** Ex: The approach taken in this project includes: Cleaning and preprocessing categorical data, performing exploratory data analysis (EDA), training machine learning models including Logistic Regression and Decision Tree.
  * **Summary of the performance achieved** Ex: Both models achieved 100% validation accuracy, indicating that the dataset contains strong patterns that clearly separate edible and poisonous mushrooms.

## Summary of Workdone

Include only the sections that are relevant an appropriate.

### Data

* Data:
  * Type:         Input: CSV file containing categorical mushroom features (cap shape, odor, gill color, etc.)
    * Output: Binary classification label (0 = edible, 1 = poisonous)
  * Size: 8,124 samples, 23 features
  * Instances (Train, Test, Validation Split): how many data points? Ex:         Training: 5,686 samples (70%)
    * Validation: 1,219 samples (15%)
    * Test: 1,219 samples (15%)

#### Preprocessing / Clean up

*  Replaced "?" values in the stalk-root column with "missing"
* Converted all categorical features into numerical format using one-hot encoding (pd.get_dummies)
* Verified that there are no missing values in the dataset
#### Data Visualization

Show a few visualization of the data and say a few words about what you see.

* Created bar charts comparing feature categories against mushroom class
* Observed strong relationships between features and class
* Features like odor were highly predictive of whether a mushroom is poisonous or edible

### Problem Formulation

* Define:
  * Input / Output
  * * Input: Encoded mushroom features
* Output: Binary label (0 = edible, 1 = poisonous)
  
  * Models
    * Describe the different models you tried and why.
     Logistic Regression (baseline model)
  Decision Tree Classifier
  * Loss, Optimizer, other Hyperparameters.
 Accuracy
 Log Loss
### Training

* Describe the training:
 * Models were trained using scikit-learn
* Training performed on a local machine (CPU)
* Logistic Regression used max_iter=1000 to ensure convergence
* Dataset required minimal preprocessing due to its clean structure
* No major training difficulties encountered

### Performance Comparison

* Clearly define the key performance metric(s).
* Show/compare results in one table.
* Logistic Regression Log Loss: 0.0064

Both models achieved perfect accuracy, showing that the dataset is highly separable.

### Conclusions

* The dataset contains strong predictive features that clearly distinguish edible and poisonous mushrooms
* Both models performed perfectly, indicating the problem is easy to classify
* Features such as odor play a major role in classification

### Future Work

* Try more advanced models (Random Forest, SVM, Gradient Boosting)
* Perform feature importance analysis
* Test the model on new or real-world datasets
* Reduce features to evaluate model robustness
## How to reproduce results

* In this section, provide instructions at least one of the following:
   git clone https://github.com/yourusername/mushroom-classification.git
cd mushroom-classification
   pip install pandas numpy scikit-learn matplotlib
  Run notebook

Open the .ipynb file in Jupyter Notebook or Google Colab and run all cells.

### Overview of files in repository

* mushroom_classification.ipynb → Main notebook (EDA, preprocessing, modeling, evaluation)
* README.md → Project documentation

  
### Software Setup
Required packages:

* pandas
* numpy
* scikit-learn
* matplotlib

### Data

Dataset available here:
https://www.kaggle.com/datasets/uciml/mushroom-classification

Download the dataset and place mushrooms.csv in the project directory before running the notebook.

### Training

Run all cells in the notebook to:

* Load data
* Preprocess features
* Train models
* Evaluate performance

#### Performance Evaluation

* Accuracy is calculated using accuracy_score
* Log loss is calculated using log_loss
* Results are printed directly in the notebook


## Citations

* Kaggle Mushroom Classification Dataset






