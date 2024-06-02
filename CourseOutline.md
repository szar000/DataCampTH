# Classification with scikit-learn
## Chapter 1: Data Preprocessing and Model Selection
### Lesson 1.1: Dealing with Data Imperfections
- Learner will be comfortable with using `SimpleImputer` and deciding wether to use the mean or the most_frequent category value dependent on type of column data
- Learner will be able to identify standardization issues with `df["column].unique`, such as inconsitent dateformats and solve them using prior Python knowledge
- Learner will be able to detect and discard outliers using `IsolationForest`
- Keywords and new syntax: `SimpleImputer`,`IsolationForest`
### Lesson 1.2: Encoding and Scaling Data
- Learner will be able to correctly assess when to apply `OneHotEncoder` vs. `LabelEncoder`
- Learner will be able to determine which estimators require data sclaing via `StandardScaler`  
- Keywords: `OneHotEncoder`, `LabelEncoder`, `StandardScaler`
### Lesson 1.3: Model Selection
- Learner will consult the machine learning map (https://scikit-learn.org/stable/tutorial/machine_learning_map/index.html) and be able to choose the correct approach
- Keywords: model selection
## Chapter 2: k-Nearest Neighbors  
### Lesson 2.1: Theoretical Foundation
- Learner will understand the motivation behind kNN by interactively visualizing the neighbor parameter at different n, rather than through excessive math notation.
- Keywords: foundation, theory, kNN
### Lesson 2.2: Training / Predicting using kNN
- Learner will be able to instantiate the `KNeighborsClassifier`
- Learner will be able to fit the training data to the estimator using `knn.fit(X_t, y_t)`, where `knn` is the estimator object
- Learner will be able to apply the model to test/unkown data using `knn.predict(X_test)`
- Keywords: train, predict
### Lesson 2.3: The Neighbour Parameter 
- Learner will be able to pick an appropriate value for `n_neighbours`
- Learner will comprehend that the perfromance of kNN is highliy dependent on the `n_neighbours` value
- Keywords: `KNeighborsClassifier`, `n_neighbours`
## Chapter 3: Support Vector Machines
### Lesson 3.1: Theoretical Foundation
- Learner will understands that SVC are based on finding hyperplanes that seperate best seperate data points in to different classes
- Keywords: foundation, theory, SVC
### Lesson 3.2: Training / Predicting using SVC
- Learner will be able to instantiate the `SVC` as `svc`
- Learner will be able to fit the training data to the estimator using `svc.fit(X_t, y_t)`
- Learner will be able to apply the model to test/unkown data using `svc.predict(X_test)`
- Keywords: train, predict
### Lesson 3.3: The Kernel
- Learner will be able to explain the difference between the `linear`, `rbf` and `polynomial`kernels and utilze the correct kernel for the given task
- Learner will confidently apply the `linear` kernel first for a good baseline, unless there is prior data knowledge that the decision boundaries are non-linear
- Keywords: kernel, `linear`, `rbf`, `polynomial`
## Chapter 4: Model Evaluation
### Lesson 4.1: Standard Accurcy metrics
- Learner will be able to use `accuracy_score` and other metrics found in scikit-learn, such as `f1_score`, `recall`
- Learner will be able to produce and analyze the confusion matrix using `confusion_matrix` and assess the models performance
- Keyword: `confusion_matrix`, `accuracy_score` and other metrics discussed
### Lesson 4.2: Validation 
- Learner will be able to perform k-fold-cross-validation using `KFold` and demonstrate why it provides a more robust perfromance evalutation
- Learner will be able to justify why this splitting has to be done for multiple iterations
- Learner will be able to extract an average score from this validation process
Keywords: k-fold-cross-validation
### Lesson 4.3: Hyperparameter Tuning
- Learner will be able to understand that the accurcy scores for initial iterations will be expected to be below the desired range
- Learner will be able to take inital scores as a baseline and apply hyperparameter tuning using `GridSearchCV`
Keywords: hyperparameters, `GridSearchCV`
   


