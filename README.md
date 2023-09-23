# Avatar-Generation-from-Real-Images
This repository is made up of GAN(Generative Adversarial Networks) which consists of Generator and Discriminator. They create new data instances that resemble your training data. Similarly
here the real images gets trained and the avatar images gets generated. This repository contains a PyTorch implementation of a Generative Adversarial Network (GAN) for generating images from random noise.

Code: https://github.com/akxhbaby2506/Avatar-Generation-from-Real-Images   [Run the code here]

# Overview

This GAN consists of two main components:
1. **Generator**: A neural network that generates fake images from random noise.
2. **Discriminator**: A neural network that distinguishes between real and fake images.

The generator and discriminator are trained simultaneously in a adversarial manner, with the goal of the generator generating increasingly realistic images over time.

## Prerequisites

Before running the code, make sure you have the following prerequisites installed:

- Python 3.x
- PyTorch
- NumPy
- Matplotlib
- torchvision

You can install these dependencies using pip:
pip install torch numpy matplotlib torchvision

Train the GAN by running the following command:

generator.py
This will train the GAN for a specified number of epochs and save the trained generator model to generator.pth.

Generate a sample image using the trained generator:
python convertor.py
This will generate and display a sample image created by the trained generator and save it as sample_generated_image.png.

Generate and save avatar images:

python avatar.py
This script loads the trained generator and generates multiple avatar images, saving them to the generated_images directory.

## Project Structure
train.py: The main script for training the GAN.
generate_sample.py: Script to generate a sample image using the trained generator.
generate_avatars.py: Script to generate and save multiple avatar images.
generator.pth: Trained generator model.
generated_images/: Directory to store generated images.
RandomNoiseDataset: Custom dataset class for generating random noise as input.

## Customization
You can customize the GAN's hyperparameters, architecture, and dataset by modifying the code in realImg.py and other relevant files. Additionally, you can replace the Random-Noise-Dataset with your own dataset for more specific image generation tasks.
