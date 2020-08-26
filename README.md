# Adaline-Madaline-Neural-Nets
Simple Neural Net like Adaline/Madaline codes (Python) similar to what taught in 8th semester the Computer Science Department, NIT Raipur.
# Steps
Just update the input array x, weight array w and target t and get the desired result in the form of dataframe table.
# Assumptions
According to the algorithm in Introduction to Neural Networks Using Matlab 6.0, S. N. Sivanandam, S. N Deepa book
# Theory
**Adaline & Madaline** comes under the supervised learning networks

**ADALINE:**
Known as Adaptive Linear Neuron
Adaline is a network with a single linear unit
The Adaline network is trained using the delta rule

**1.1  Architecture**

As already stated Adaline is a single-unit neuron, which receives input from several units and also from one unit, called bias. An Adeline model consists of trainable weights. The inputs are of two values (+1 or -1) and the weights have signs (positive or negative).

Initially random weights are assigned. The net input calculated is applied to a quantizer transfer function (possibly activation function) that restores the output to +1 or -1. The Adaline model compares the actual output with the target output and with the bias and the adjusts all the weights.

**1.2  Training Algorithm**

The Adaline network training algorithm is as follows:

Step0: weights and bias are to be set to some random values but not zero. Set the learning rate parameter α.

Step1: perform steps 2-6 when stopping condition is false.

Step2: perform steps 3-5 for each bipolar training pair s:t

Step3: set activations foe input units i=1 to n.

Step4: calculate the net input to the output unit.

Step5: update the weight and bias for i=1 to n

Step6: if the highest weight change that occurred during training is smaller than a specified tolerance then stop the training process, else continue. This is the test for the stopping condition of a network.

**1.3  Testing Algorithm**

It is very essential to perform the testing of a network that has been trained. When the training has been completed, the Adaline can be used to classify input patterns. A step function is used to test the performance of the network. The testing procedure for the Adaline network is as follows:

Step0: initialize the weights. (The weights are obtained from the training algorithm.)

Step1: perform steps 2-4 for each bipolar input vector x.

Step2: set the activations of the input units to x.

Step3: calculate the net input to the output units

Step4: apply the activation function over the net input calculated.

**2. Madaline**

![Madaline Image](https://github.com/Duttabhi/Basic-Neural-Nets/blob/master/Madaline.jpg)

Stands for multiple adaptive linear neuron
It consists of many adalines in parallel with a single output unit whose value is based on certain selection rules.
It uses the majority vote rule
On using this rule, the output unit would have an answer either true or false.
On the other hand, if AND rule is used, the output is true if and only if both the inputs are true and so on.
The training process of madaline is similar to that of adaline
2.1 Architecture

It consists of “n” units of input layer and “m” units of adaline layer and “1”

Unit of the Madaline layer

Each neuron in the adaline and madaline layers has a bias of excitation “1”

The Adaline layer is present between the input layer and the madaline layer; the adaline layer is considered as the hidden layer.

**2.2 Uses**

The use of hidden layer gives the net computational capability which is not found in the single-layer nets, but this complicates the training process to some extent.

**2.2 Training Algorithm:**

In this training algorithm, only the weights between the hidden layers are adjusted, and the weights for the output units are fixed. The weights v1, v2………vm and the bias b0 that enter into output unit Y are determined so that the response of unit Y is 1.
