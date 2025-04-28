# Image_Resolution_Enhancer
This project implements a Generative Adversarial Network (GAN) to perform image super-resolution — enhancing low-resolution images into high-resolution outputs. It is trained on the CelebA face dataset, where the generator learns to upscale 24×24 pixel images into detailed 96×96 pixel images.

Project Structure
Dataset:

Uses the CelebA dataset (aligned celebrity faces).

Manually loaded and processed into low-resolution (LR) and high-resolution (HR) image pairs.

Model Architecture:

Generator: Upsamples low-resolution images through convolutional layers and upsampling layers to produce high-resolution images.

Discriminator: Classifies real vs generated high-resolution images using convolutional blocks.

Loss Functions:

Pixel-wise Loss (MSE): Ensures the generated images are close to ground-truth images.

Adversarial Loss (Binary Cross Entropy): Helps the generator produce realistic images that can fool the discriminator.

Training Details:

Both models are trained adversarially.


Low-resolution images are progressively enhanced throughout training.

Visualization:

After each epoch, the model visualizes:

LR (Low Resolution Input)

SR (Super Resolved Output)

HR (Ground Truth High Resolution)
