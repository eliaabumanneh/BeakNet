# [BeakNet](https://github.com/eliaabumanneh/BeakNet/blob/main/BeakNet_main.ipynb)

Insert Image

# TLDR;

Bird image classification tool built using a trained convoluted neural network. You can view it [here](https://github.com/eliaabumanneh/BeakNet/blob/main/BeakNet_main.ipynb)

# Project Walkthrough




# Methodology

The information below was used to guide the model creation process. Following a carefully design first trial, each subsequent model was adjusted based on its observed behaviour using the guidelines below. 

## Layers
* The number of input neurons should be the number of input features (as dummy variables)
* The number of hidden layers will depend on experimentation. Start with at least 2. More hidden layers = more learning. 
* The number of output neurons should be the number of output features (as dummy variables)

## [Optimizer](https://www.youtube.com/watch?v=BheE01CeL8I&ab_channel=M%C4%B1sraTurp)

* Optimizers are used to reduce the network training time

* Optimizers use gradient vectors (think of a 3D topography graph,depending on where your input point starts, 
  it will "fall" based on the gradient at the position to an output value that activates an output neuron path)

* Try the last 4 optimizers on this list, if performance is not good, try Nesterov.

## GD with Momentum:  

* Regular GD updates gradient vector every time without learning from past

* GD with Momentum takes into account previous changes using a momentum variable and a "friction" index

* Almost always faster than GD

* Runs through plateaus faster (as momentum is kept even if gradient is low)

* Fewer oscillations than GD

## Nesterov Accelerated Gradient
* Similar to GD with Momentum but:

* The gradient vector is a derivative of (current location + the current momentum) compared to GD with Momentum which only derives the grad vect from current location

* Generally faster than GD with Momentum

## The 4 below are the "Best ones" (fast, no need for tuning)
* AdaGrad

    Decays the learning rates (slows the learning as epochs increase)
   
    The problem is, it might slow down too early
    
* RMSProp

    Similar to AdaGrad but it decays the rate of decay
    
* Adam

    Combination of (Momentum + RMSProp) - 4 parameters no tuning needed
    
* Nadam:

    Nadam = Nesterov + Adam

    
## Iterations:
* Too many = over-fitting

* We can implement early stopping to determine the optimal number

## Batch Size: 

* Divides the data into parts. Each epoch only looks at a specific batch

* This helps prevent over-fitting

## Hidden Layer
* Each additional hidden layer is similar to another polynomial power

* 0 H Layers: If the function is capable of being represented by separable linear functions

* 1 H Layer: If you need at least one kernel

* 2 H Layer: Capable of representing arbitrary data relationships

# Project Limitations
* Data Limitation: Due to limited computing power, the model was trained on only 15 species of birds. By leverage the power of parallel computing and cloud computing, the same model can be scaled to hundreds of bird species while remaining performant. 

* Modelling Limitation: The keras model created in this project has an overall classification accuracy of 84%. With further optimisation, the model accuracy can theoretically go up to as high as 97%. 

# Data Source(s)
* [Kaggle: BIRDS 515 SPECIES- IMAGE CLASSIFICATION](https://www.kaggle.com/datasets/gpiosenka/100-bird-species)


# Languages Used
* Python

# Software Used
* Visual Code Studio
* GitHub Desktop
* GitHub
* cuDNN

# Python Packages Used
* Pandas
* Numpy
* Scikit-learn
* Scikit-image
* Tensorflow 
* Keras
* Matplotlib
* Pillow


# Legal

This project was created and is intended for educational purposes only. The creator(s) nor any user(s) nor distributor(s) claim legal responsibility for any information, data, claim or prediction infered or supplied by this program whether implicitly or explicitly. The program is not to be sold or resold. The information provided by the program is not to be sold or resold. The project may be used by others for educational and non-commerical purposes.
