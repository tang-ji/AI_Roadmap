

# Training

## score

### Diagnosing Model

- [x] Variance Bias

### Confusion Matrix

 **true positive (TP)**   **true negative (TN)**   

**false positive (FP)**  - false alarm, Type I error  

**false negative (FN)**  - miss, Type II error

- [ ] AUC ROC

- [x] Accuracy

  $\mathrm {ACC}={\frac {\mathrm {TP} +\mathrm {TN} }{\mathrm {P} +\mathrm {N} }}=\frac {\mathrm {T} }{\mathrm {T} +\mathrm {F}}$

- [x] Precision - Positive Predictive Value

  $\mathrm {PPV}=\frac {\mathrm {TP} }{\mathrm {TP} + \mathrm {FP}}$

- [x] Recall - True Positive Rate

  $\mathrm {TPR}=\frac {\mathrm {TP} }{\mathrm {TP} + \mathrm {FN}}$

- [x] F1 score

  $\mathrm {F} _{1}=2\cdot {\frac {\mathrm {PPV} \cdot \mathrm {TPR} }{\mathrm {PPV} +\mathrm {TPR} }}$

- [x] Type 1, 2 Error

  Type I error: False positive

  Type II error: False negative

- [ ] K-fold cross validation

## Data Splitting

- [x] Training
- [x] Validation
- [x] Test

# Dimensionality Reduction

## Eigen Decomposition

### Matrix Property

### Eigen Value

### Eigen Vector

- [ ] PCA SVD

  Principal Component Analysis

  Singular Value Decomposition

   We name the eigenvectors for *$AA^T$* as *$u_i$* and *$A^TA$* as *$v_i$* here and call these sets of eigenvectors *u* and *v* the **singular vectors** of *A*. The square roots of these eigenvalues are called **singular values**. 

- [ ] Kernel PCA

  K is an N-by-N kernel: $K = k(x,y)=\Phi(x)^T\Phi(y)$

  Then we centralize K to become K': $K'=K-1_{\mathbf{N}}K-K1_{\mathbf{N}}+1_{\mathbf{N}}K1_{\mathbf{N}}$

  Finally we solve the eigenvector equation: $N\lambda a=K'a$

   where N is the number of data points in the set, and $\lambda$ and $\mathbf {a} $ are the eigenvalues and eigen vectors of $K'$. 

# Ensemble

- [ ] Bagging

   It also reduces variance and helps to avoid overfitting.  Given a standard training set $D$ of size *n*, bagging generates *m* new training sets $D_{i}$, each of size *n′*, by sampling from *D* uniformly and with replacement. 

- [ ] AdaBoost

- [ ] Random Forest 

# Clustering

- [ ] Hierarchical
- [ ] K-means

# Non-Probabilistic

- [ ] Kernel SVM
- [ ] Kernel Trick
- [ ] C-SVM
- [ ] KKT Condition
- [ ] Lagrangian approach

# Regularization

- [ ] Early Stopping
- [ ] Weight Decay
- [ ] Dropout

### Normalization

- [ ] Layer normalization

  ![img](https://i1.wp.com/mlexplained.com/wp-content/uploads/2018/01/%E3%82%B9%E3%82%AF%E3%83%AA%E3%83%BC%E3%83%B3%E3%82%B7%E3%83%A7%E3%83%83%E3%83%88-2018-01-11-11.48.12.png?resize=628%2C366)

- [ ] Batch normalization

  We want to use the global mean and variance to normalize the inputs to a layer, but it costs too much after each update of the network. Smaller mini-batch sizes increase the variance.

  Hard to apply on recurrent connections.

  Add some stochastic noise to the activations. (has a regularization effect in some applications but can be potentially harmful in some noise sensitive domains)

- [ ] Weight normalization

  computationally cheaper compared to batch normalization

# Logistic Regression

## Activation Function

- [ ] Sigmoid

  ![img](https://pic4.zhimg.com/80/v2-208a4aa5dc657fe86919f3549d853793_hd.jpg)

  the max derivative is smaller than 0.25 -> gradient vanishing

- [ ] tanh

  ![[公式]](https://www.zhihu.com/equation?tex=%5Ctanh+%28x%29%3D%5Cfrac%7Be%5E%7Bx%7D-e%5E%7B-x%7D%7D%7Be%5E%7Bx%7D%2Be%5E%7B-x%7D%7D%5C%5C)

  ![img](https://pic4.zhimg.com/80/v2-66a7e4fcf11a2d85c15e7bf7b88b2d1b_hd.jpg)

  better than sigmoid but the derivative is still smaller than 1

- [ ] ReLU

  the derivative is always 1, solve gradient vanishing/ gradient exploding, facilate computation and training.

  input smaller than 0 always output 0, the derivative isn't continue around 0

- [ ] Leakly ReLU

  ![img](https://pic4.zhimg.com/80/v2-3ab1bd8fb85542a0c85eb907b73fa327_hd.jpg)

  solve the segment smaller than 0

- [ ] PReLU

- [ ] ELU

  solve the continuity of derivative around 0

- [ ] Maxout

# Linear Regression