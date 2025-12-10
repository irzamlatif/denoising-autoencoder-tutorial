# Denoising Auto-encoder Complete Tuutorial using Fashion-MNIST Dataset
This repository contain a full tutorial and implementation of a 
**convolutional denoising autoencoder** using **Fashion-MINIST** 
dataset and Keras.
This project illustrate how neural network can reconstruct clean 
and images from noisy inputs by following the denoising autoencoder
which is introduced by Vincent et al. (2008).

---

## project overview
This project aim to teach and how denoising autoencoder can be 
implemented in practice and how it work.
The tutorial explain both the implementation and the theory,
making it easy to unerstand for readers with basic knowledge of neural networks.
The topics this tutorial cover are such as:

- How representation leraning works and what autoencoders are.
- why adding noise improves generalisation and robustness.
- How acn we built a convolutional encoder- decoder architecture with Keras.
- How to interpret training and validation loss and train the model.
- How can we visualise reconstruction quality using images.

This repository also contain a **written PDF tutorial report**

# Repository Contents
- Individual Assignment.ipynb - Notebook containing implementation
- Individual Assignmen.pdf - pdf contain written tutorial
- README.md - Description of the project
- requirements.txt - python dependencies
- LICENCE - MIT licence
- images/ - figures used in the tutorial

## How to Run the code:
1. Install all the required dependencies
2. open the Notebook Individual Assignment.ipynb
3. Run all the cells from top to bottom to get the results.

## This model is a convolutional denoising auto-encoder:
1.Encoder:
- Conv2D (32 filters) + ReLU
- MaxPooling
- Conv2D (64 filters) + ReLU
- MaxPooling
2.Decoder:
- Conv2D (64 filters) + ReLU
- UpSampling
- Conv2D (32 filters) + ReLU
- UpSampling
- Conv2D (1 filter, sigmoid)
3.Loss function used: MSE(MEAN SQUARED ERROR)
4.Optimiser:Adam
5.Training: 20 epochs, batch size: 128

## Results Summary:
The performance this model achieved:
- Model final training loss: 0.0139
- Model final validation loss: 0.0142
- The close distance differnce between training and
  validation loss indicates minimal overfitting and strong generalisation.

## Author:
[Irzam Latif]
Machine learning and Neural Networks
2025
