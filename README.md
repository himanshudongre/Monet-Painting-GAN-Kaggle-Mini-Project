# Monet-Painting-GAN-Kaggle-Mini-Project

# Problem Statement
This project aims to use generative adversarial networks (GANs) to create images in the style of Claude Monet, the renowned impressionist painter. The generated images will be evaluated on their artistic quality using the Memorization-informed Fréchet Inception Distance (MiFID) score, provided by Kaggle.

This solution notebook is available at : https://github.com/himanshudongre/Monet-Painting-GAN-Kaggle-Mini-Project.git

## Objective
Develop a GAN model capable of:
1. Generating Monet-style images based on the provided dataset of Monet paintings and landscape photos.
2. Optimizing the GAN model to minimize the MiFID score, ensuring high-quality image generation.


# Generative Adversarial Networks (GANs)
GANs are a class of generative models comprising two components:
- **Generator**: Creates synthetic data (images) from random noise.
- **Discriminator**: Distinguishes between real and generated images.

The interplay between these two networks enables the generator to improve over time, producing images indistinguishable from real ones.


# Evaluation Metric
The MiFID score incorporates:
- **Fréchet Inception Distance (FID)**: Measures similarity between the feature distributions of real and generated images.
- **Memorization Distance**: Evaluates the minimum cosine distance between generated images and real training samples.

A lower MiFID score indicates better quality and diversity of the generated images.


# Dataset Description
The dataset consists of four directories:
1. **monet_jpg**: 300 Monet paintings in JPEG format, size 256x256.
2. **photo_jpg**: 7028 photos in JPEG format, size 256x256.
3. **monet_tfrec**: TFRecord format of the Monet images.
4. **photo_tfrec**: TFRecord format of the photos.

All images are in RGB format, having three channels (Red, Green, Blue).

The Dataset for this project can be found at : https://www.kaggle.com/competitions/gan-getting-started/data
 
