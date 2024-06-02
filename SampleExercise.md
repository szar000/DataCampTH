# Examining the impact of the k neighbours value  
This excersise aims to put your classification skills to the test and showcase the influence of the k parameter on the final predictions using a real life exmaple.
To accomplish this, you're are going to fit two kNN estimators with iris data, where both estimators will have different k values.
The iris dataset has been pre-split for you into `X_train`,`X_test`,`y_train`, `y_test`.

# Instructions
- Instantiate two kNN estimator objects, `knn_1` and `knn_2` with different `n_neighbors` values. Please make sure that the values are at least 5 apart.
- Fit the training data to the classfiers with the `.fit()` method using the appropriate variable. Due to the specifics on how the data is strucutred, the slicing has been done for you. 
- Try predicting the test traget data by using the `.predict` method on both estimators using the appropriate variable. Due to the specifics on how the data is strucutred, the slicing has been done for you. 
- Take a moment to examine `y_pred_1` and `y_pred_2`. Do they match? Are they what you expect based on the previous theory?    

# Code
```python 
from sklearn.neighbors import KNeighborsClassifier
from sklearn.model_selection import train_test_split

X_train, X_test, y_train, y_test = train_test_split(iris['data'], iris['target'],test_size=0.3, random_state=42)

# Instantiate both estimator objects
knn_1 = ______(_____=__)
knn_2 = ______(__=__)

# Fit the classifiers
knn_1.__(___[:, 2:], ___)
knn_2.__(___[:, 2:], ___)
# Use the fitted classfiers to predict the test data
y_pred_1 = knn_1.___(___[:, 2:])
y_pred_2 = knn_2.___(___[:, 2:])
# Compare the results by printing the predictions
print(f"Results of the first classfier:{y_pred_1})
print(f"Results of the second classfier:{y_pred_2})
```
# Solution Code 
```python
from sklearn.neighbors import KNeighborsClassifier
from sklearn.model_selection import train_test_split

X_train, X_test, y_train, y_test = train_test_split(iris['data'], iris['target'],test_size=0.3, random_state=42)

# Your k values don't necessarly have to match
knn_1 = KNeighborsClassifier(n_neighbors=1)
knn_2 = KNeighborsClassifier(n_neighbors=6)

# Fit the classifiers with X_train and y_train
knn_1.fit(X_train[:, 2:], y_train)
knn_2.fit(X_train[:, 2:], y_train)
# Use the fitted classfiers to predict the test data using X_test
y_pred_1 = knn_1.predict(X_test[:, 2:])
y_pred_2 = knn_2.predict(X_test[:, 2:])
# Compare the results by printing the predictions
print(f"Results of the first classfier:{y_pred_1})
print(f"Results of the second classfier:{y_pred_2})
```
