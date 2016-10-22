## eignFaces

### Compute a PCA (eigenfaces) on the face dataset
    n_samples: 760
    n_features: 1850
    n_classes: 3

### Extracting the top 150 eigenfaces from 570 faces
    done in 0.157s

### Projecting the input data on the eigenfaces orthonormal basis
    done in 0.017s

### Calculationg PCA components' Variance:
    Variance explained by the first principal component:  0.18954512666
    Variance explained by the second principal component: 0.155786516991

### PCA #components and f1_score relation - classification Report
         
| n_components| -  |  precision |  recall |  f1-score | support
|-----|:------------------:|:------:|:-------:|:-------:|
|  10 | Donald Rumsfeld  | 0.54 | 0.61  |  0.57 | 36
| 15  | Donald Rumsfeld  | 0.69 | 0.56  |  0.62 | 36
| 50  | Donald Rumsfeld  | 0.97 |  0.86 |  0.91 | 36
| 150 | Donald Rumsfeld  | 0.86 |  0.86 |  0.86 | 36
| 250 | Donald Rumsfeld  | 0.83 |  0.83 |  0.83 | 36


* Fitting the classifier to the training set
    done in 3.839s

* Best estimator found by grid search:
    SVC(C=1000.0, cache_size=200, class_weight='balanced', coef0=0.0,
    decision_function_shape=None, degree=3, gamma=0.001, kernel='rbf',
    max_iter=-1, probability=False, random_state=None, shrinking=True,
    tol=0.001, verbose=False)


* Predicting the people names on the testing set
done in 0.010s

* Classification Report
                   precision    recall  f1-score   support

  Donald Rumsfeld       0.91      0.83      0.87        36
    George W Bush       0.91      0.98      0.94       123
Gerhard Schroeder       0.96      0.77      0.86        31

      avg / total       0.92      0.92      0.91       190

* confusion_matrix

[[ 30   6   0]
 [  2 120   1]
 [  1   6  24]]
