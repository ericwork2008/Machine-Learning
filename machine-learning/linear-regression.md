# Linear Regression

## Fomular

<figure><img src="../.gitbook/assets/image (4) (1).png" alt=""><figcaption></figcaption></figure>

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

<figure><img src="../.gitbook/assets/image (34).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (2) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

## Gradient descent

Gradient descent is an algorithm for finding values of parameters w and b that minimize the cost function J. [**Gradient descent**](https://developers.google.com/machine-learning/glossary#gradient-descent) is a mathematical technique that iteratively finds the weights and bias that produce the model with the lowest loss. Gradient descent finds the best weight and bias by repeating the following process for a number of user-defined iterations.

Alpha is the learning rate

<figure><img src="../.gitbook/assets/image (3) (1) (1).png" alt=""><figcaption></figcaption></figure>

\


<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

* Batch: each step of gradient descent uses all the training examples.

## Adam (Adaptive Moment estimation) Algorithm

learning alpha isn't a fix value.

<figure><img src="../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>
