# What is a Neural Network?

## What is a neural network? (Mathematically)
There are many variants of Neural Networks:

In the first 2 chapters, we will be looking at the **most simplest form of a NN**

### Neural Networks
- inspired by the brain 🧠

Neuron → a thing that holds a number

The network starts with a bunch of neurons corresponding to each of the 28x28 pixels of an input image (784).


Each number (between 0 and 1) represents the grayscale value of said image
- 0 (black pixels)
- 1 (white pixels)

![[Screenshot 2024-11-16 at 6.22.44 PM.png|This is a caption|575]]
- The number inside the neuron is called its "Activation".
- Its like every neuron is lit up when its activation is a high number

**These 784 neurons make up the first layer of our neural network**
![[Screenshot 2024-11-16 at 6.23.55 PM.png|The last layer (highlighted above), represents each digit|575]]


The activation value for each neuron in the last layer represents how much the system thinks that a given image corresponds with a given digit

- for example, if the computer looks at the number 1, but 1 kinda looks like 7, so numbers like 1 and 7 will have higher values than a number like zero

The layers in the middle are the **hidden layers**

**Each layer is supposed to predict or determine the activations of the next layer**
The model above is already trained to recognize digits

If you feed it an image, lighting up the right neurons in the input layer:
- That pattern of activations causes some very specific pattern in the next layer
- and the one after it
- until finally the last layer, where the brightest neuron is the one the computer thinks the number is

Why do layered structures even work?
- because when you think, you think in parts, or by recognizing patterns from memory

Use weights of any number for any range (positive or negative) to determine something transform it into an activation value through the sigmoid function:
![[Screenshot 2024-11-16 at 6.24.55 PM.png|Sigmoid Function]]

Very negative inputs end up close to 0
Very positive inputs end up close to 1

### Weights:
what pixel pattern this neuron in the second layer is picking up on

### Bias:
How high the weight needs to be, before the neuron starts getting meaningfully active
**Learning:** Finding the right Weights and Biases

### Equation for perceptron:
$$
a_{0}^{(1)} = \sigma \Bigg( w_{0,0} \space a_{0}^{(0)} + w_{0,1} \space a_{1}^{(0)} + \dotsb + w_{0,n} \space a_{n}^{(0)} + b_0 \Bigg)
$$
$$\text{where } b_0 \text{ is the bias}$$
![[Screenshot 2024-11-16 at 7.10.27 PM.png|Each neuron as a subject of the function]]

Basically

- every activation from one layer becomes a column as a vector
- every weight from the layer gets added to a matrix
    - each row of the matrix corresponds to a particular neuron in the next layer
- taking the weighted sum of the activations in the first layer, corresponds to one of the terms of the matrix vector product in the next layer:

## ReLU (better than sigmoid)

function where you take a max of 0 and a
$$
\text{ReLU(a)} = \text{max}(0,a)
$$
if it passes a certain threshold its activated, instead of using a function where there is ambiguity as to whether or not a neuron is active.
![[Screenshot 2024-11-16 at 7.19.48 PM.png|ReLU function]]


