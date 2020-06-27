# Image-Denoising-Using-Autoencoder
Building and training an image denoising autoencoder using Keras with Tensorflow 2.0 as a backend.

## Overview
- Import Key libraries, dataset and visualize images
- Perform image normalization, pre-processing, and add random noise to images
- Build an Autoencoder using Keras with Tensorflow 2.0 as a backend
- Compile and fit Autoencoder model to training data 
- Assess the performance of trained Autoencoder using various KPIs 

## Understanding the theory 
### Autoencoder Intuition
Autoencoders are a type of Artificial Neural Networks that are used to perform a task of data encoding (representation learning).
Autoencoders use same input data for input as well as output, crazy right?

![GitHub Logo](/img/Autoencoder Denoising.png)

### Code Layer
Autoencoders work by adding a bottleneck in the network.
This bottleneck forces the network to create a compressed (encoded) version of the original input.
Autoencoders work well if correlations exist between input data and (performs poorly if all the input data is independent).

Great reference: “Intro to Autoencoders by Jeremy Jordan”

![GitHub Logo](/img/Autoencoder Denoising2.png)

### Math behind Autoencoder
Encoder: h(x) = ``` sigmoid (W * x + b) ```

Decoder: ``` x̂ = sigmoid (W* * h(x) + c) ```

![GitHub Logo](/img/Autoencoder Denoising3.png)

### Reconstruction Error
Autoencoders objective is to minimize the reconstruction error which is the difference between the input X and the network output X̂. 

![GitHub Logo](/img/Autoencoder Denoising4.png)



Autoencoders dimensionality reduction (latent space) is quite similar to PCA (Principal Component Analysis) if linear activation functions are used.




