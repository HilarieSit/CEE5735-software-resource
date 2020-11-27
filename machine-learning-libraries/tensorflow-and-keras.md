---
description: >-
  Tensorflow is a popular ML framework developed by Google that makes
  implementing optimized deep learning models very simple. Popular high-level
  APIs include Keras and TF Probability.
---

# Tensorflow

## On this page:

1. [Tensorflow](tensorflow-and-keras.md#tensorflow)
   1. [Version 1.x](tensorflow-and-keras.md#tensorflow-1-x)
   2. [Version 2.x](tensorflow-and-keras.md#tensorflow-2-x-eager-execution)
   3. [Tensorboard](tensorflow-and-keras.md#tensorboard)
2. [Keras](tensorflow-and-keras.md#keras)
3. [Tensorflow Probability](tensorflow-and-keras.md#tensorflow-probability)

## Tensorflow

Tensorflow \(TF\) is a powerful ML framework that lets us develop and train models that are computationally optimized and compatible with different processing units, including CPUs, GPUs, and the more recent TPUs. 

### Tensorflow 1.x

In TF 1.x, the _**computational**_ _**graph**_, which maps out operation order and dependencies, is specified first, before any computations occur. This type of graph is commonly called a _**static graph**_ since it doesn't change during a _**session**_, which is when the graph is executed and values are computed. 

![Tensorflow graph visualized using Tensorboard](../.gitbook/assets/image%20%281%29.png)

A TF computational graph is specified using a combination of these objects and operations: 

* _**TF Placeholders**_ are objects that are given information at the time of computation. Ex: the input layer of a neural network.
* _**TF Variables**_ are the parameters that are evaluated during a session. Ex: weights and biases.
* _**TF operations,**_ which __are performed on placeholders and variables, closely follow NumPy operations. TF also includes more ML specific functions, such as one-hot encoding \(_i.e._ turning classifications into integer representation\) and nonlinear activation functions. 

In addition to the graph, we also need to specify the training method and any functions to execute during training:

* _**Optimizer**_ minimizes the specified loss function to iteratively update the TF variables.
* _**Callback functions**_ are functions that are executed during training after a certain number of iterations. Popular callbacks include early stopping \(_i.e._ determining when to stop training\), using [TensorBoard](tensorflow-and-keras.md#tensorboard-visualization-tool), etc. 

Finally, to perform the computation, we start a TF session _****_and feed the placeholders with our dataset. 

{% embed url="https://www.tensorflow.org/versions/r1.15/api\_docs" %}

### Tensorflow 2.x \(Eager Execution\)

With TF 2.x, there are no longer TF "sessions" and everything is executed eagerly.

{% embed url="https://www.tensorflow.org/api\_docs" %}

### TensorBoard \(Visualization Tool\)

Tensorboard is Tensorflow's visualization tool for viewing computational graphs, tracking variables & performance metrics, etc. Installation of Tensorflow includes TensorBoard. To launch the dashboard, run this on terminal and point the --logdir to the appropriate directory.

```text
tensorboard --logdir=summaries
```

Open the link shown on the terminal \(default: localhost:8888\) on a web browser.

![TensorBoard dashboard](../.gitbook/assets/screen-shot-2020-11-27-at-12.57.06-pm%20%281%29.png)

{% embed url="https://www.tensorflow.org/tensorboard/get\_started" %}

## Keras

Keras is a popular high-level API for building deep neural networks using prebuilt layers \(_i.e._ dense layers, convolutional layers, batch normalization layers, etc.\). Keras is great for quickly building regular models, but can't accommodate custom operations like in Tensorflow/Pytorch.

{% embed url="https://keras.io" %}

Another benefit of Keras is the abundance of [pre-trained model architectures](https://keras.io/api/applications/) that are available for transfer learning.

## Tensorflow Probability

Tensorflow Probability is a library for probabilistic deep learning models and includes useful tools for Variational Inference, Bayesian Neural Networks, MCMC, etc.

{% embed url="https://www.tensorflow.org/probability" %}

