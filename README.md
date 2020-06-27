# Image-Denoising-Using-Autoencoder
Building and training an image denoising autoencoder using Keras with Tensorflow 2.0 as a backend.

## Overview
- Import Key libraries, dataset and visualize images
- Perform image normalization, pre-processing, and add random noise to images
- Build an Autoencoder using Keras with Tensorflow 2.0 as a backend
- Compile and fit Autoencoder model to training data 
- Assess the performance of trained Autoencoder using various KPIs 

## Prerequisites
- Basic programming experience in python
- Basic understanding of Tensorflow
- Working knowledge of Machine Learning and Deep Learning

## Understanding the theory 
### Autoencoder Intuition
Autoencoders are a type of Artificial Neural Networks that are used to perform a task of data encoding (representation learning).
Autoencoders use same input data for input as well as output, crazy right?

![intuition](/img/AutoencoderDenoising.png?raw=true "Title")

### Code Layer
Autoencoders work by adding a bottleneck in the network.
This bottleneck forces the network to create a compressed (encoded) version of the original input.
Autoencoders work well if correlations exist between input data and (performs poorly if all the input data is independent).

Great reference: “Intro to Autoencoders by Jeremy Jordan”

![Code layer](/img/AutoencoderDenoising2.png)

### Math behind Autoencoder
Encoder: ``` h(x) = sigmoid (W * x + b) ```

Decoder: ``` x̂ = sigmoid (W* * h(x) + c) ```

![math](/img/AutoencoderDenoising3.png)

### Reconstruction Error
Autoencoders objective is to minimize the reconstruction error which is the difference between the input X and the network output X̂. 

![reconstruction](/img/AutoencoderDenoising4.png)



Autoencoders dimensionality reduction (latent space) is quite similar to PCA (Principal Component Analysis) if linear activation functions are used.


## Installing

A step by step series of examples that tell you how to get a development env running

### Step 1
Download the prerequisites from the ``` requirements.txt``` file.

``` pip install -r requirements.txt ```

### Step 2
Open ``` jupyter notebook ``` on your local host or you can use Google Colab too.

### Step 3
Follow the steps in the notebook if you want to train your own or you can simply run the notebook in this repo.

## Output

This is a side-by-side comparison of the input images with added noise and the reconstructed output from the network.

![output](/img/AutoencoderDenoising5.png)


## References to study in detail about related topics
*[Autoencoders](https://towardsdatascience.com/applied-deep-learning-part-3-autoencoders-1c083af4d798)
*[Deep Learning](https://www.datacamp.com/community/tutorials/deep-learning-python)