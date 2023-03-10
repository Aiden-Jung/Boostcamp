# [Day 3] AI Math - Vector & Matrix & Intro to Deep Learning

## 1. Vector
* Vector
  * In mathematics, physics, and engineering, a Euclidean vector or simply a vector is a geometric object that has magnitude (or length) and direction. [1]
* Operation
  * Suppose we have 
    $$ x = \begin{pmatrix} x_1 \\ x_2 \\ \vdots \\ x_d \end{pmatrix} \textmd{ and } y = \begin{pmatrix} y_1 \\ y_2 \\ \vdots \\ y_d \end{pmatrix} $$
  * Addition & Subtraction
    $$ x \pm y = \begin{pmatrix} x_1 \pm y_1 \\ x_2 \pm y_2 \\ \vdots \\ x_d \pm y_d \end{pmatrix} $$
  * Norm
    * L1-norm
      $$ ||x||_1 = \sum^d_{i=1}|x_i| $$
    * L2-norm
      $$ ||x||_2 = \sqrt{\sum^d_{i=1}|x_i|^2} $$
  * Product
    * Inner Product
      $$\langle x, y \rangle = x^Ty $$

      $$ \langle x, y \rangle = ||x||_2||y||_2 \cos \theta $$
    * Outer Product
      $$ x \otimes y = xy^T $$
      $$ x \otimes y = ||x||_2||y||_2 n \sin \theta $$
    * Hadamard product
      $$ x \circ y = \begin{pmatrix} x_1 y_1 \\ x_2 y_2 \\ \vdots \\ x_d y_d \end{pmatrix}$$

## 2. Matrix
* Matrix
  * In mathematics, a matrix (plural matrices) is a rectangular array or table of numbers, symbols, or expressions, arranged in rows and columns, which is used to represent a mathematical object or a property of such an object. [2]
* Operation
  * Suppose we have 
    $$ X = \begin{pmatrix} x_{1,1} & x_{1,2} & \dots & x_{1,m} \\ x_{2,1} & x_{2,2} & \dots & x_{2,m} \\ \vdots & \vdots \\ x_{n, 1} & x_{n,2} & \dots & x_{n,m} \end{pmatrix} \textmd{ and } Y = \begin{pmatrix} y_{1,1} & y_{1,2} & \dots & y_{1,m} \\ y_{2,1} & y_{2,2} & \dots & y_{2,m} \\ \vdots & \vdots \\ y_{n, 1} & y_{n,2} & \dots & y_{n,m} \end{pmatrix} $$
  * Addition & Subtraction
    $$ X \pm Y = \begin{pmatrix} x_{1,1} \pm y_{1,1} & x_{1,2} \pm y_{1,2} & \dots & x_{1,m} \pm y_{1,m} \\ x_{2,1} \pm y_{2,1} & x_{2,2} \pm y_{2,2} & \dots & x_{2,m} \pm y_{2,m} \\ \vdots & \vdots \\ x_{n, 1} \pm y_{n,1} & x_{n,2} \pm y_{n,2} & \dots & x_{n,m} \pm y_{n,m} \end{pmatrix} $$
  * Product
    * Matrix Multiplication
      $$ XY = \left( \sum_k x_{i,k}y_{k,j} \right) $$
    * Hadamard product
      $$ X \circ Y = \begin{pmatrix} x_{1,1} y_{1,1} & x_{1,2} y_{1,2} & \dots & x_{1,m} y_{1,m} \\ x_{2,1} y_{2,1} & x_{2,2} y_{2,2} & \dots & x_{2,m} y_{2,m} \\ \vdots & \vdots \\ x_{n, 1} y_{n,1} & x_{n,2} y_{n,2} & \dots & x_{n,m} y_{n,m} \end{pmatrix} $$
  * numpy.inner (different from mathematical inner product)
* Inverse Matrix
  * If there exists, find it.
  * If not, find a Moore-Penrose inverse matrix

## 3. Intro to Deep Learning
* Neural Network
  * Artificial neural networks (ANNs), usually simply called neural networks (NNs) or neural nets, are computing systems inspired by the biological neural networks that constitute animal brains. [3]
  * It is a combination of a linear model and activation functions
* Function
  * Activation Function
    * Sigmoid
    * ReLU
    * Tanh
    * Softmax (commonly used for the output layer)
  * Optimization Function
    * Gradient Descent
    * Stochastic Gradient Descent(SGD)
    * Adam
    * RMSprop
    * Adagrad
    * Adadelta
  * Loss Function
    * Different depending on situations
  * Update
    * Backpropagation

* Gradient Descent
  * In mathematics, gradient descent (also often called steepest descent) is a first-order iterative optimization algorithm for finding a local minimum of a differentiable function. [4]
  * It is similar as Newton's method, but it does not use the second derivative information.
  * SGD(Stochastic Gradient Descent) can be used to reduce cost.

<!-- Reference -->
[1]: https://en.wikipedia.org/wiki/Euclidean_vector

[2]: https://en.wikipedia.org/wiki/Matrix_(mathematics)

[3]: https://en.wikipedia.org/wiki/Artificial_neural_network

[4]: https://en.wikipedia.org/wiki/Gradient_descent