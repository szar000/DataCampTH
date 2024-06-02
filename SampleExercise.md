# Examining the impact of the k neighbours value  
This excersise aims to put your classification skills to the test and showcase the influence of the k parameter on the final predictions using a real life exmaple.
To accomplish this, you're are going to fit two kNN estimators with iris data, where both estimators will have different k values.
The iris dataset has been pre-split for you into `X_train`,`X_test`,`y_train`, `y_test`.



# Code
```python 
from sklearn.neighbors import KNeighborsClassifier
from sklearn.model_selection import train_test_split

X_train, X_test, y_train, y_test = train_test_split(iris['data'], iris['target'],test_size=0.3, random_state=42)

# Instantiate both estimator objects
knn_1 = ______(_____=__)
knn_2 = ______(__=__)

# Fit the classifiers
knn_1.__(___, ___)
knn_2.__(___, ___)
# Use the fitted classfiers to predict the test data
y_pred_1 = knn_1.___(___)
y_pred_2 = knn_2.___(___)
# Compare the results by printing the predictions
print(f"Results of the first classfier:{y_pred_1})
print(f"Results of the second classfier:{y_pred_2})
```
