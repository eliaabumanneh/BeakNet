# [BeakNet](https://github.com/eliaabumanneh/BeakNet/blob/main/BeakNet_main.ipynb)

Insert Image

# TLDR;

Bird image classification tool built using a trained convoluted neural network. You can view it [here](https://github.com/eliaabumanneh/BeakNet/blob/main/BeakNet_main.ipynb)

# Project Summary

1. A set of bird images were converted into tensors.

![123](https://user-images.githubusercontent.com/59853149/233221779-54fd8cc7-ce8f-4b58-9794-5b45fc630a91.png)

2. A convoluted neural network was created using Keras and Tensorflow. 
![image](https://user-images.githubusercontent.com/59853149/233220928-8a622a17-9e6e-433c-a698-9d59dcd01322.png)

3. The model was trained and used to make predictions. The training was monitored to avoid over-fitting or under-fitting. 

4. The model's performance was evaluated based on the precision, recall, and f1-score
![image](https://user-images.githubusercontent.com/59853149/233221404-641fec2a-b76a-4a00-8710-8c000c4c648e.png)



# Methodology

A set of [guidelines](https://github.com/eliaabumanneh/BeakNet/blob/main/guidelines.txt) were reserached, created and used in the model creation process. Following a carefully design first trial, each subsequent model was adjusted based on its observed behaviour using the guidelines.

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
