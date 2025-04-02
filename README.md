

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

Each notebook is self-contained and focuses on a specific project, such as Linear Regression, Linear Classification, Cross-Validation, and more.


### Projects

- **P01.ipynb** - Linear Regression  
    This project implemented linear regression from scratch on the prostate cancer dataset, using closed-form solutions enhanced with ridge and lasso regularization. Cross-validation was applied to fine-tune hyperparameters, and additional feature engineering with polynomial and interaction terms significantly boosted prediction accuracy.  

    - Developed a linear regression model from scratch.
    - Incorporated ridge and lasso regularization for stability.
    - Used cross-validation for hyperparameter tuning.
    - Enhanced predictions with polynomial and interaction features.

- **P02.ipynb** - Logistic Regression  
    This project developed logistic regression using stochastic gradient descent to assess heart disease risk on the South African Heart Disease dataset. It compared unregularized, forward stepwise, L1, and L2 regularized models, and extended the approach to multiclass classification on the Iris dataset using softmax and cross-entropy loss.  

    - Built logistic regression with SGD.
    - Compared multiple regularization techniques.
    - Tuned hyperparameters via cross-validation.
    - Extended the model to multiclass classification.

- **P03.ipynb** - Model Assessment and Validation  
    This project examined model validation by implementing a 1-nearest neighbor classifier on synthetic data, contrasting the improper approach of pre-selecting features with the correct within-fold feature selection. The analysis clearly demonstrated how validation strategies impact evaluation outcomes.  

    - Implemented a 1-nearest neighbor classifier.
    - Compared pre-selection vs. within-fold feature selection.
    - Highlighted the importance of proper cross-validation.
    - Emphasized rigorous validation for reliable evaluation.

- **P04.ipynb** - Gradient Boosted Trees  
    This project applied gradient boosting using XGBoost on the California Housing dataset, optimizing hyperparameters through grid search and monitoring performance via loss curves and absolute error metrics. Interpretability analyses—featuring feature importance plots, partial dependence charts, and SHAP visualizations—highlighted key predictors, with further validation on the Breast Cancer dataset confirming robustness.  

    - Used XGBoost with grid search for optimization.
    - Monitored performance using loss curves and error metrics.
    - Conducted detailed interpretability analyses (feature importance, partial dependence, SHAP).
    - Validated model robustness on an additional dataset.

- **P05.ipynb** - Random Forests  
    This project compared random forests and gradient boosted trees on the California Housing dataset by tracking test error trends as the number of trees increased, and by visualizing feature importance differences. The study was extended to the Iris dataset to verify the consistency of performance and predictor significance across domains.  

    - Compared random forests with gradient boosted trees.
    - Analyzed test error trends with increasing tree counts.
    - Visualized and compared feature importances.
    - Extended analysis to a different dataset for validation.

- **P06.ipynb** - NMF  
    In this project, a recommendation system was built using Non-negative Matrix Factorization (NMF) with the Surprise library on an explicit feedback dataset, with cross-validation tuning for latent dimensions and regularization parameters. Additionally, a custom NMF algorithm was implemented to gain deeper insights, and exploration of implicit feedback data provided intuitive rating explanations.  

    - Developed a recommendation system using NMF.
    - Tuned latent dimensions and regularization via cross-validation.
    - Implemented a custom NMF algorithm for deeper insights.
    - Explored implicit feedback for intuitive rating explanations.

- **P07.ipynb** - Data Mining with Market Basket  
    This project transformed NYC school performance data into a market basket framework by treating schools as transactions and academic metrics as items. The Apriori algorithm was then applied to extract frequent itemsets and association rules, with parameter tuning revealing significant associations—such as the strong link between attendance and subject proficiency—that offer actionable insights.  

    - Converted school performance data into market basket format.
    - Applied the Apriori algorithm to mine frequent itemsets and association rules.
    - Tuned parameters to uncover significant associations.
    - Derived actionable insights for improving academic outcomes.