### Task Overview
The main objective of this task is to develop predictive models for loan approvals based on a large dataset. The task involves preprocessing the data, constructing logistic regression and K-nearest neighbour (KNN) models, and evaluating their performance using accuracy and F1-score metrics.

### Data Used
The dataset contains demographic, credit history, employment, income, debt, and other financial metrics. The target variable is "LoanApproved," with the remaining variables as features. The dataset is a synthetic collection designed to simulate real-world loan approval scenarios.

### Algorithms Applied
Two classification algorithms are applied:
1. **Logistic Regression**: This algorithm models the outcome of a loan approval (with the outcomes being the loan being granted or rejected). RFE is employed to enhance feature selection.
2. **K-Nearest Neighbour (KNN)**: Both 1-NN and KNN models are trained, with grid search and cross-validation used to fine-tune the number of neighbours (K) and analyse the impact of different distance metrics (Euclidean, L1, Cosine).

### Deployment/Execution
The models are implemented in Python. After cleaning the dataset (handling missing values, one-hot encoding), the data is split into 80% training and 20% testing. Model training, validation, and evaluation are performed in a Jupyter notebook. RFE and grid search are utilised for model optimization.

### Key Takeaways
- Logistic regression serves as a baseline model, with RFE identifying the most important features.
- KNN benefits from hyperparameter tuning, with performance varying across different distance metrics.
- The performance is evaluated on both training and test sets, ensuring that the models are not overfitting.
- Visualisations like line charts and bar charts provide insights into performance trends across feature eliminations and hyperparameter selections.
