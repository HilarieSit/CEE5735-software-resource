---
description: >-
  Tensorflow is a popular machine learning framework developed by Google that
  makes implementing optimized deep learning models very simple. It also has
  higher-level APIs: Keras and TF Probability.
---

# Tensorflow

## On this page:

1. [Tensorflow](tensorflow-and-keras.md#tensorflow)
   1. [Tensorboard](tensorflow-and-keras.md#tensorboard)
   2. [Eager Execution](tensorflow-and-keras.md#eager-execution-tf-2-0)
2. [Keras](tensorflow-and-keras.md#keras)
3. [Tensorflow Probability](tensorflow-and-keras.md#tensorflow-probability)

## Tensorflow

Tensorflow is a powerful ML framework that lets us implement models that are computationally optimized with parallel computing and compatibility with different processing units, such as CPUs/GPUs/TPUs. In TF, the _**computational**_ _**graph**_, which maps out operation order and dependencies, is built first, before any computations occur. Because the graph doesn't change, we refer to this type of graph as a _**static graph**_.

![Tensorflow graph visualized using Tensorboard](../.gitbook/assets/image%20%281%29.png)

TF operations closely follow NumPy operations, but the framework also includes more ML specific functions, such as one-hot encoding \(_i.e._ turning classifications into integer representation\). _**Placeholders**_ are TF objects that are given information at the time of computation \(when we "run the _**session**_"\). TF _**variables**_ are the parameters that are evaluated during a session \(_e.g._ the weights and biases in a neural network\).

{% embed url="https://www.tensorflow.org/api\_docs" %}

### Tensorboard

Tensorboard is Tensorflow's visualization tool that allows us to view computational graphs, track variables & performance metrics, etc. 

![](../.gitbook/assets/screen-shot-2020-11-27-at-12.57.06-pm%20%281%29.png)

{% embed url="https://www.tensorflow.org/tensorboard/get\_started" %}

### Eager Execution \(TF 2.0\)

[Top of Page --&gt; ](tensorflow-and-keras.md#on-this-page)

## Keras

Keras is a popular high-level API for building deep neural networks: neural networks can be build by simply specifying prebuilt layers \(_i.e._ dense layers, convolutional layers, etc.\). Keras is great for quickly building regular models, but can't accommodate custom operations. 

{% embed url="https://keras.io" %}

[Top of Page --&gt; ](tensorflow-and-keras.md#on-this-page)

## Tensorflow Probability

Tensorflow Probability is a library for probabilistic models, which include Variational Inference, Bayesian Neural Networks, MCMC, etc.

{% embed url="https://www.tensorflow.org/probability" %}

[Top of Page --&gt; ](tensorflow-and-keras.md#on-this-page)

