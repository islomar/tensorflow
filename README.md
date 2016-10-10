# Tensorflow
Playground for learning about Tensorflow

https://www.tensorflow.org/


**Tutorials:** 
* https://codelabs.developers.google.com/codelabs/tensorflow-for-poets/index.html
* https://www.tensorflow.org/versions/r0.11/get_started/index.html

http://playground.tensorflow.org/

https://github.com/tensorflow/


**Inception** is a huge image classification model with millions of parameters that can differentiate a large number of kinds of images. We're only training the final layer of that network, so training will end in a reasonable amount of time.

Deep learning is a branch of Machine Learning inspired by how the brain works.

TensorFlow™ is an open source software library for numerical computation using data flow graphs. 

**What is a Data Flow Graph?**
Data flow graphs describe mathematical computation with a directed graph of nodes & edges. Nodes typically implement mathematical operations, but can also represent endpoints to feed in data, push out results, or read/write persistent variables. Edges describe the input/output relationships between nodes. These data edges carry dynamically-sized multidimensional data arrays, or tensors. The flow of tensors through the graph is where TensorFlow gets its name. Nodes are assigned to computational devices and execute asynchronously and in parallel once all the tensors on their incoming edges becomes available.

A **Bottleneck** then, is an informal term we often use for the layer just before the final output layer that actually does the classification.

**Going deeper with convolutions**
http://www.cs.unc.edu/~wliu/papers/GoogLeNet.pdf


* The **training accuracy** shows the percentage of the images used in the current training batch that were labeled with the correct class.
* **Validation accuracy**: The validation accuracy is the precision (percentage of correctly-labelled images) on a randomly-selected group of images from a different set.
* **Cross entropy** is a loss function that gives a glimpse into how well the learning process is progressing. (Lower numbers are better here.)

A true measure of the performance of the network is to measure its performance on a data set that is not in the training data. This performance is measured using the validation accuracy. If the training accuracy is high but the validation accuracy remains low, that means the network is overfitting, and the network is memorizing particular features in the training images that don't help it classify images more generally.

The training's objective is to make the cross entropy as small as possible, so you can tell if the learning is working by keeping an eye on whether the loss keeps trending downwards, ignoring the short-term noise.

`docker run -it gcr.io/tensorflow/tensorflow:latest-devel`

```
# docker run -it -v ~/workspace/tensorflow/tf_files:/tf_files  gcr.io/tensorflow/tensorflow:latest-devel
# ls /tf_files/
# cd /tensorflow
# git pull
# ls /tensorflow/tensorflow/examples/image_retraining/
```


##Neural networks and deep learning
http://neuralnetworksanddeeplearning.com/index.html



##Glossary
* **Convolution**
In mathematics (and, in particular, functional analysis) convolution is a mathematical operation on two functions (f and g); it produces a third function, that is typically viewed as a modified version of one of the original functions, giving the integral of the pointwise multiplication of the two functions as a function of the amount that one of the original functions is translated.