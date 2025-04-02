

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
    - This project implemented linear regression from scratch on the prostate cancer dataset, employing closed-form solutions along with ridge and lasso regularization to enhance model stability and interpretability. Cross-validation was used to fine-tune hyperparameters, and further feature engineering with polynomial and interaction terms on an additional dataset significantly improved prediction accuracy. Overall, the approach provided robust insights into the impact of regularization on model coefficients.
- **P02.ipynb** - Logistic Regression  
    -  In this project, logistic regression was developed using stochastic gradient descent to analyze heart disease risk on the South African Heart Disease dataset, with comparisons among unregularized, forward stepwise, L1, and L2 regularized models. Hyperparameters were tuned via cross-validation, and the model was extended to multiclass classification using softmax and cross-entropy loss, successfully applied to the Iris dataset. The results demonstrated effective model tuning and clear performance improvements across different regularization te
- **P03.ipynb** - Model Assessment and Validation  
    - This project focused on model validation by implementing a 1-nearest neighbor classifier on synthetic data to illustrate the impact of cross-validation strategies. It contrasted the improper approach of selecting features before cross-validation with the correct within-fold feature selection, clearly demonstrating how these choices affect evaluation outcomes. The study underscored the importance of rigorous validation to reliably assess model performance.
- **P04.ipynb** - Gradient Boosted Trees  
    - This project applied gradient boosting using XGBoost on the California Housing dataset, where grid search was used to optimize hyperparameters and performance was monitored through absolute error metrics and loss curves. Detailed interpretability analyses, including feature importance plots, partial dependence charts, and SHAP visualizations, highlighted the influence of key predictors like median income and geographic factors. The model's robustness was further confirmed through validation on the Breast Cancer dataset.
- **P05.ipynb** - Random Forests  
    - This project compared random forests and gradient boosted trees on the California Housing dataset by tracking test absolute error across varying numbers of trees and visualizing feature importance. The analysis revealed significant differences in predictor influence between the two methods, prompting discussions on the underlying reasons. An extension of the study to the Iris dataset confirmed the consistency of observed performance trends and feature significance across different domains.
- **P06.ipynb** - NMF  
    - In this project, a recommendation system was built using Non-negative Matrix Factorization (NMF) via the Surprise library on an explicit feedback dataset, with cross-validation used to tune latent dimensions and regularization parameters. A custom NMF algorithm was also implemented from scratch to provide deeper insights into model behavior. Additionally, the exploration of implicit feedback data aimed to generate intuitive rating explanations, offering novel perspectives on user-item interactions.
- **P07.ipynb** - Data Mining with Market Basket  
    - This project transformed NYC school performance data into a market basket framework by treating schools as transactions and academic metrics as items, then applied the Apriori algorithm to identify frequent itemsets and mine association rules. Parameter tuning (min_support=0.1, min_confidence=0.7) led to the discovery of significant associations, such as a strong link between attendance and subject proficiency. The analysis provided actionable insights into how key performance indicators interrelate, suggesting targeted strategies to improve academic outcomes.
