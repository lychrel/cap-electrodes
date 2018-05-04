# Capacitive Electrodes: Signal Collection & Analysis

---

### Arduino Control

rtbt.ino

![Press Down Key](img/down-arrow.png)

+++



---

### Softmax Implementation

![Softmax](img/s1.png)

![Press Down Key](img/down-arrow.png)

+++

### equation form
![Softmax (equation form)](img/s1_eqns.png)

![Press Down Key](img/down-arrow.png)

+++

### matrix form
![Softmax (matrix form)](img/s1_matrices.png)

![Press Down Key](img/down-arrow.png)

+++

### defining the model 

```python
x = tf.placeholder(tf.float32, [None, 784])
W = tf.Variable(tf.zeros([784, 10]))
b = tf.Variable(tf.zeros([10]))
y = tf.nn.softmax(tf.matmul(x, W) + b)
```

---

## MNIST with SoftMax

![Press Down Key](img/down-arrow.png)

+++?code=mnist_softmax.py&lang=python

@[16-20](tutorial source)
@[21-27](various imports)
@[28-29](load MNIST data)
@[30](load TensorFlow API)
@[32](FLAGS)
@[35-37](import the (one-hot encoded) MNIST data)
@[40-42](create variables, weights, and biases)
@[43](matrix multiplication)
@[46](output layer (predicted probabilities))
@[57-58](define the loss function (measurement of incorrectness))
@[59](define how we want to reduce loss (incorrectness) over time (stochastic gradient descent))
@[61-62](start a session in TensorFlow)
@[64-66](train network using above parameters on 10 sets of 100 images)
@[69-71](check accuracy of predictions)
@[74-79](run session)
