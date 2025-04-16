

> This repository contains the code for **ECE 471: Frequentist Machine Learning**, a 3-credit graduate-level course at The Cooper Union for the Advancement of Science and Art, focusing on practical applications of statistical inference and supervised machine learning techniques.

## Frequentist Machine Learning
**Course, Fall 2024**  
**Instructor:** Professor Sam Keene

### Overview

This course provides an applied introduction to frequentist machine learning methods, emphasizing statistical inference, exploratory data analysis, and predictive modeling. Students gain both theoretical insights and practical experience through structured mini-projects covering regression, classification, regularization, feature selection, decision trees, ensemble methods, and data visualization. By engaging in comprehensive hands-on projects, students learn how to select, evaluate, and interpret machine learning models effectively, preparing them for advanced research or industry roles.


### Material

The primary textbook for the course is [*The Elements of Statistical Learning*](https://www.goodreads.com/book/show/148009.The_Elements_of_Statistical_Learning) by Trevor Hastie, Robert Tibshirani, and Jerome Friedman, covering key topics such as:

- Linear regression and regularization techniques (Ridge, LASSO, Elastic Net)
- Classification methods including Logistic Regression and Support Vector Machines (SVM)
- Classification and regression trees, Random Forests, and Extreme Gradient Boosting
- Model selection and cross-validation strategies
- Data visualization and exploratory data analysis



### Repository Structure

```
.
├── P01.ipynb
├── P02.ipynb
├── P03.ipynb
├── P04.ipynb
├── P05.ipynb
├── P06.ipynb
├── P07.ipynb
└── README.md
```

- **`P01.ipynb`** – *Linear Regression*
  - Implements a linear regression model (with ridge and lasso) on the prostate cancer dataset, integrating cross-validation and polynomial/interaction features for enhanced predictions.

- **`P02.ipynb`** – *Logistic Regression*  
  - Uses logistic regression (with various regularization methods) to assess heart disease risk, then extends to multiclass classification via softmax on the Iris dataset.

- **`P03.ipynb`** – *Model Validation*  
  - Showcases a 1-nearest neighbor classifier on synthetic data, illustrating the contrast between pre-selecting features and performing within-fold selection.

- **`P04.ipynb`** – *Gradient Boosted Trees*  
  - Applies gradient boosting (XGBoost) on the California Housing dataset, tuning hyperparameters through grid search and assessing interpretability via feature importance and partial dependence charts.

- **`P05.ipynb`** – *Random Forests*  
  - Compares random forests with boosted trees by examining test error, feature importance, and cross-dataset validity (California Housing and Iris).

- **`P06.ipynb`** – *NMF for Recommendations*  
  - Builds a recommendation system using Non-negative Matrix Factorization with the Surprise library, alongside a custom NMF approach for deeper insight.

- **`P07.ipynb`** – *Market Basket Analysis*  
  - Transforms NYC school data into a transactional format and applies Apriori to identify frequent itemsets and rules, revealing notable academic performance correlations.