# GAN vs VAE on MNIST dataset
## CAP6610 Machine Learning - Final Project

## GAN
Generative adversarial networks were proposed in a 2014 paper by Ian Goodfellow et al., and although the idea got researchers excited almost instantly, it took a few years to overcome some of the difficulties of training GANs. Like many great ideas, it seems simple in hindsight: make neural networks compete against each other in the hope that this competition will push them to excel. GAN is composed of two neural networks:
### Generator
Takes a random distribution as input (typically Gaussian) and outputs some data — typically, an image. You can think of the random inputs as the latent representations (i.e., codings) of the image to be generated. So, as you can see, the generator offers the same functionality as a decoder in a variational autoencoder, and it can be used in the same way to generate new images (just feed it some Gaussian noise, and it outputs a brand-new image). However, it is trained very differently, as we will soon see.
### Discriminator
Takes either a fake image from the generator or a real image from the training set as input, and must guess whether the input image is fake or real.

## VAE
Another important category of autoencoders was introduced in 2013 by Diederik Kingma and Max Welling and quickly became one of the most popular types of autoencoders: variational autoencoders.
They are quite different from all the autoencoders we have discussed so far, in these particular ways:
 - They are probabilistic autoencoders, meaning that their outputs are partly deter‐ mined by chance, even after training (as opposed to denoising autoencoders, which use randomness only during training).
 - Most importantly, they are generative autoencoders, meaning that they can generate new instances that look like they were sampled from the training set.

## Details about Files
* Autoencoder.ipynb - Variational AutoEncoder
* GAN.ipynb - Generative Adversarial Network

## Instruction for Running
I ran the code on Google Colaboratory due to lack of GPU support on my personal system. To check, the two files can be downloaded, and tested individually by simply running them in Google Colabs at separate instances. They do not require any additional dependencies on the host machine like python, tensorflow or other libraries as these are already installed in Colabs.
