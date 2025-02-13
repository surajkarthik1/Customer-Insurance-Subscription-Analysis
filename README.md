# Vehicle-Insurance-Subscription-Analysis

### Project Overview:

This project aims to predict car insurance subscription likelihood from initial quote data using various machine learning models. Utilizing a comprehensive dataset including features like quote date, vehicle make, and model, this analysis involves rigorous data preprocessing, feature engineering, and model evaluation to enhance prediction accuracy.

### Data Description:

The dataset encompasses numerous features such as vehicle make, model, quote date, and personal details provided during the insurance quotation. The primary objective is to use this data to predict whether customers will purchase insurance post-quote.

## Data Preprocessing and Feature Engineering:

### Data Cleaning:

* Consistency Adjustment: We standardized vehicle make and model names using a dictionary for mapping, correcting various spelling errors and inconsistencies.
* Handling Missing Values: Missing values in categorical and numeric fields were imputed with 'Unknown' or central tendency measures (mean/median) based on the distribution of the data.

### Feature Selection and Engineering:

* Feature Reduction: Used Chi-squared tests to reduce dimensionality, selecting 296 significant features out of the initial set for model building.
* Encoding: Applied one-hot encoding to transform categorical variables into a numerical format, facilitating their use in machine learning models.

### Modeling and Evaluation:

* Initial Models: Evaluated Logistic Regression and two types of Naive Bayes (Categorical and Bernoulli).
* Optimization: Tuned Bernoulli Naive Bayes through iterations of alpha and binarize values, which showed promising results.
* Model Comparison: The ROC curve and AUC metrics were utilized to compare models. Bernoulli Naive Bayes outperformed others with better precision and accuracy.

## Results:

Final Choice: Bernoulli Naive Bayes was selected based on its superior performance in our tests, achieving a prediction accuracy of 78% on the test set.

## Conclusion:

The project demonstrates the effectiveness of detailed data preprocessing and feature selection in improving the accuracy of predictive models. Bernoulli Naive Bayes, with its focus on binary features, proved optimal for our needs, underscoring the importance of model selection based on specific project goals and data characteristics. The study reinforces the necessity of using advanced statistical techniques and machine learning to refine insurance marketing strategies and customer understanding.
