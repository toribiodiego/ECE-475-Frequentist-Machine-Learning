

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
    - **Implemented Linear Regression from Scratch:** 
        - Developed a custom model using closed-form solutions on the prostate cancer dataset with a robust train/validation/test split.  
    - **Applied Regularization Techniques:** 
        - Compared hand-coded ridge regression and scikit-learn’s lasso regression with cross-validation to tune hyperparameters and visualize coefficient trends.  
    - **Enhanced Performance with Feature Engineering:** 
        - Extended the analysis to an additional dataset and introduced polynomial and interaction terms, significantly reducing error and refining feature selection.
- **P02.ipynb** - Logistic Regression  
    - **Implemented Logistic Regression with SGD:** 
        - Developed a logistic regression model using stochastic gradient descent, with and without L2 regularization, to replicate the analysis on the South African heart disease dataset.  
    - **Optimized and Compared Models:** 
        - Employed cross-validation and forward stepwise feature selection to tune hyperparameters and compare unregularized, stepwise, L2, and L1 regularized models based on accuracy.  
    - **Extended to Multiclass Classification:** 
        - Expanded the binary model to multinomial logistic regression using the softmax function and cross-entropy loss, and validated the approach on the Iris dataset.
- **P03.ipynb** - Model Assessment and Validation  
    - **Reproduced Cross-Validation Analysis:** 
        - Implemented a 1-nearest neighbor classifier on synthetic data to demonstrate the impact of cross-validation strategy.  
    - **Contrasted Incorrect vs. Correct Methods:** 
        - Highlighted the pitfalls of selecting predictors before cross-validation versus within each fold, emphasizing proper feature selection.  
    - **Evaluated Model Performance:** 
        - Compared average percent error rates to validate and illustrate the benefits of correct cross-validation procedures.
- **P04.ipynb** - Gradient Boosted Trees  
    - **Applied XGBoost for Regression Analysis:** 
        - Tuned an XGBoost model on the California Housing dataset using grid search, and evaluated performance through absolute error metrics and loss curves.
    - **Interpreted Feature Importance:** 
        - Visualized predictor importance and generated partial dependence plots to reveal how key features—such as Median Income and geographic coordinates—influence housing prices.
    - **Enhanced Insights with SHAP:** 
        - Leveraged SHAP to produce global and local interpretability plots (bar, dependence, and beeswarm), and extended the analysis to the Breast Cancer dataset for additional validation.
- **P05.ipynb** - Random Forests  
    - **Compared Ensemble Methods:** 
        - Replicated figure 15.3 by training random forests and gradient boosted trees on the California Housing dataset, evaluating performance through test absolute error as the number of trees increased.  
    - **Analyzed Feature Importances:** 
        - Visualized and contrasted the relative importance of predictors from both models, offering insights into any notable discrepancies.  
    - **Extended Analysis to a New Dataset:** 
        - Repeated the study on the Iris dataset, confirming the consistency of model performance and feature importance trends across different data domains.
- **P06.ipynb** - NMF  
    - **Built a Recommendation System Using Surprise:** Developed a recommendation system on an explicit feedback dataset with the Surprise library, tuning latent dimensions and regularization parameters through cross-validation.  
    - **Implemented Custom NMF (Stretch Goal):** Crafted an NMF algorithm from scratch and optimized it via cross-validation to select the optimal number of latent dimensions and regularization parameter.  
    - **Explored Implicit Feedback for Rating Explanations (Stretch Goal):** Investigated an implicit feedback dataset by implementing a variant of NMF to generate rating explanations, offering innovative insights into recommendation modeling.
- **P07.ipynb** - Data Mining with Market Basket  
    - **Reframed Educational Data as Market Baskets:** Converted NYC school performance metrics into transaction-like records by treating schools as transactions and key academic indicators as items.  
    - **Extracted Frequent Itemsets and Association Rules:** Applied the Apriori algorithm (via mlxtend) with carefully tuned parameters (min_support=0.1, min_confidence=0.7) to identify high-support itemsets and derive meaningful association rules.  
    - **Derived Actionable Insights:** Analyzed the discovered rules to reveal strong interdependencies—such as the link between attendance and subject proficiency—providing valuable recommendations for improving school performance.

