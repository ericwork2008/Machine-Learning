# Classification with Logistic regression

## Logistic Regression

<figure><img src="../.gitbook/assets/image (6) (1) (1).png" alt=""><figcaption></figcaption></figure>

## Decision Boundary



## Loss Function

* Logistic regression models use [**Log Loss**](https://developers.google.com/machine-learning/glossary#Log_Loss) as the loss function instead of [**squared loss**](https://developers.google.com/machine-learning/glossary#l2-loss).
* Applying [regularization](https://developers.google.com/machine-learning/crash-course/overfitting/regularization) is critical to prevent [**overfitting**](https://developers.google.com/machine-learning/glossary#overfitting).

### Regularization in logistic regression <a href="#regularization_in_logistic_regression" id="regularization_in_logistic_regression"></a>

[**Regularization**](https://developers.google.com/machine-learning/glossary#regularization), a mechanism for penalizing model complexity during training, is extremely important in logistic regression modeling. Without regularization, the asymptotic nature of logistic regression would keep driving loss towards 0 in cases where the model has a large number of features. Consequently, most logistic regression models use one of the following two strategies to decrease model complexity:

* [L2 regularization](https://developers.google.com/machine-learning/crash-course/overfitting/regularization)
* [Early stopping](https://developers.google.com/machine-learning/crash-course/overfitting/regularization#early_stopping_an_alternative_to_complexity-based_regularization): Limiting the number of training steps to halt training while loss is still decreasing.

#### **Regularization to Prevent Overfitting**

(From ChatGPT) Regularization is a technique that introduces a penalty for excessive complexity. It discourages large coefficients (β1,β2,…) in the polynomial equation, making the model simpler and more robust.

**Common Types of Regularization:**

1. **Lasso Regression (L1 Regularization)**:
   * Adds a penalty equal to the absolute value of coefficients (∑∣βi∣).
   * Encourages sparsity, often driving some coefficients to zero (feature selection).
2. **Ridge Regression (L2 Regularization)**:
   * Adds a penalty equal to the square of the coefficients (∑βi^2​).
   * Shrinks coefficients but doesn’t make them zero.
3. **Elastic Net**:
   * Combines L1 and L2 penalties.

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (2) (1) (1).png" alt=""><figcaption></figcaption></figure>

## Gradient Descent

<figure><img src="../.gitbook/assets/image (2) (1) (1) (2) (1).png" alt=""><figcaption></figcaption></figure>

### Confusion matrix <a href="#confusion_matrix" id="confusion_matrix"></a>

<figure><img src="../.gitbook/assets/image (1) (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

**Recall is probability of detection**

<figure><img src="../.gitbook/assets/image (2) (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (3) (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (4) (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (5) (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>
