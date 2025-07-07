# Linear Regression

## Refresh

<figure><img src="../../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>

## Fomular

<figure><img src="../../.gitbook/assets/image (4) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

```
a = np.array([1, 2, 3, 4])
b = np.array([-1, 4, 3, 2])
c = np.dot(a, b)

//create a 1*5 matrix
a = np.zeros((1, 5))    
a = [[0. 0. 0. 0. 0.]]

a = np.arange(6).reshape(-1, 2)   #reshape is a convenient way to create matrices
a= [[0 1]
 [2 3]
 [4 5]]
 
//slicing (start:stop:step)
a[0, 2:7:1]
```

## Linear Regression

From [https://developers.google.com/machine-learning/crash-course/linear-regression/loss](https://developers.google.com/machine-learning/crash-course/linear-regression/loss)

<figure><img src="../../.gitbook/assets/image (34).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (2) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

## Gradient descent

Gradient descent is an algorithm for finding values of parameters w and b that minimize the cost function J. [**Gradient descent**](https://developers.google.com/machine-learning/glossary#gradient-descent) is a mathematical technique that iteratively finds the weights and bias that produce the model with the lowest loss. Gradient descent finds the best weight and bias by repeating the following process for a number of user-defined iterations.

Alpha is the learning rate

<figure><img src="../../.gitbook/assets/image (3) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

\


<figure><img src="../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

* Batch: batch refers to running all the examples in one iteration.



## Adam (Adaptive Moment estimation) Algorithm

learning alpha isn't a fix value.

<figure><img src="../../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>

## Feature scale

* to change feature in \[0,1].
* mean normalization.  mean
* z-normalization  =  (x-mean)/standard deviation

<figure><img src="../../.gitbook/assets/image (35).png" alt=""><figcaption></figcaption></figure>

Scikit-learn has a gradient descent regression model [sklearn.linear\_model.SGDRegressor](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.SGDRegressor.html#examples-using-sklearn-linear-model-sgdregressor). Like your previous implementation of gradient descent, this model performs best with normalized inputs. [sklearn.preprocessing.StandardScaler](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.StandardScaler.html#sklearn.preprocessing.StandardScaler) will perform z-score normalization as in a previous lab. Here it is referred to as 'standard score'.

## Learning rate

## Hyperparameters

[**Hyperparameters**](https://developers.google.com/machine-learning/glossary#hyperparameter) are variables that control different aspects of training. Three common hyperparameters are:

* [**Learning rate**](https://developers.google.com/machine-learning/glossary#learning-rate)
* [**Batch size**](https://developers.google.com/machine-learning/glossary#batch-size)
* [**Epochs**](https://developers.google.com/machine-learning/glossary#epoch)
