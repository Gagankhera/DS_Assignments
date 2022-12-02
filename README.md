# DS_Assignments
Tasks for Data Scientist role

Completed the following 2 tasks as part of Shack Labs DS role Assignment:

House Price Prediction 
Matching of Amazon and Flipkart Products

Libraries & Frameworks Used
For Task 1: House Price Prediction
Numpy
Pandas
Matplotlib
Seaborn
Scikit-learn
Scipy

For Task 2: Product Matching
Pandas
Numpy

Machine Learning Models Performance Comparison for Task 1: House Price Prediction
Drawbacks related to Underlying Assumptions of Machine Learning Algorithms

The assumptions associated with regression modeling and machine learning in general are as follows:

Homoscedasticity: The variance of residual should be the same for any value of X.
Observations are assumed to be independent of each other.
For most of the machine learning algorithms such as Linear Regression and many clustering algorithms, normal distribution is necessary for producing better outcomes.
Unstability: Tree-based models are relatively unstable. A small change in the data can cause a large change in the structure of the decision tree causing instability.
Non-scalability: Several boosting models such as XGBoost and Gradient Boosting models are very sensitive to outliers since every classifier is forced to fix the errors in the predecessor learners. The overall method is hardly scalable. Moreover, they don't perform well enough on sparse and unstructured data due to their internal working and underlying assumptions.

Model	R2 Score (%)\
Linear Regression	78.85\
Lasso Regression 78.83\
Ridge Regression 78.52\
Random Forest Regressor 84.27\
Gradient Boosting Regressor 83.49\
BaggingRegressor 79.02

Hyperparameter Tuning
GridSearchCV(RandomForestRegressor(),parameters,cv=5)
R2_Score: 84.75

Installation of Scikit-learn
scikit-learn requires:

Python (>= |PythonMinVersion|)
NumPy (>= |NumPyMinVersion|)
SciPy (>= |SciPyMinVersion|)
joblib (>= |JoblibMinVersion|)
threadpoolctl (>= |ThreadpoolctlMinVersion|)
Scikit-learn 0.20 was the last version to support Python 2.7 and Python 3.4. scikit-learn 1.0 and later require Python 3.7 or newer. scikit-learn 1.1 and later require Python 3.8 or newer.

Scikit-learn plotting capabilities (i.e., functions start with plot_ and classes end with "Display") require Matplotlib (>= |MatplotlibMinVersion|). For running the examples Matplotlib >= |MatplotlibMinVersion| is required. A few examples require scikit-image >= |Scikit-ImageMinVersion|, a few examples require pandas >= |PandasMinVersion|, some examples require seaborn >= |SeabornMinVersion| and plotly >= |PlotlyMinVersion|.

User installation
If you already have a working installation of numpy and scipy, the easiest way to install scikit-learn is using pip:

pip install -U scikit-learn
or conda:

conda install -c conda-forge scikit-learn
The documentation includes more detailed `installation instructions `_.
