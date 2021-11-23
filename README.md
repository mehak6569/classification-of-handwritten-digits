# Classification of the handwritten digits ‘4 and 9’ from the MNIST dataset

## Introduction
The MNIST database of handwritten digits, has a training set of 60,000 examples, and a test set of 10,000 examples. It is a subset of a larger set available from NIST. The digits have been size-normalized and centered in a fixed-size image. 

&nbsp;

## Dataset Description
* There are a total of **60,000 datapoints** (rows in train_data) corresponding to digits ranging from 0 to 9.  
* The **first column** has the label of the datapoint ranging from 0 to 9.
* The **next 784 columns/features** are each a 28 $\times$ 28 grayscale image collapsed into a row. Therefore, the dimension of the data is 784. Each of these values range from 0 to 275 where 0 corresponds to white and 255 corresponds to black.


>An example of a datapoint with label 0.

![Datapoint with label 0](/figures/datapoint_0.png "Label - 0")

&nbsp;

## Problem Statement

![MNIST scatter plot](/figures/mnist_plot.png "MNIST dataset after dimension reduction to 2")

Datapoints corresponding to labels such as **0 and 1 are well separated**, however, ambiguous datapoints such as those **corresponding to 4 and 9 are overlapping**. This makes sense as even when observed by a naked eye 0 and 1 are easily distinguishable however 4 and 9 may not always be as they both have a vertical line towards the bottom and a loop-like structure on top.

Since 4 and 9 are notoriously similar, with a loop on the top and a line on the bottom, this can be corroborated looking at our 2-D t-SNE plot, we see that 0 and 1 are clustered relatively far from each other making them easily distinguishable, however 4 and 9 are overlapping. 

_**The aim is to design Variational Quantum Classifier circuit from Aqua to classify the digits 4 and 9.**_









