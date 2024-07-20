# Image-to-Image Translation with cGAN

This repository contains a project demonstrating image-to-image translation using Conditional Generative Adversarial Networks (cGANs) with TensorFlow. The implementation focuses on translating images from night to day using the `night2day` dataset, but it can be adapted to other datasets as well.

## Description

Image-to-image translation involves converting one type of image to another, such as transforming night scenes into day scenes. This project uses a cGAN, where a generator network learns to create realistic day images from night images, and a discriminator network learns to distinguish between real and generated day images.

### Key Features:

- **Dataset Handling**: Automatically downloads and extracts the `night2day` dataset from the Pix2Pix dataset collection.
- **Image Preprocessing**: Includes functions for resizing, cropping, normalizing, and applying random jitter to enhance the training data.
- **Generator and Discriminator**: Implements a U-Net based generator for high-quality image generation and a PatchGAN discriminator for evaluating the generated images.
- **Training Loop**: Custom training loop with logging and checkpointing to save model progress and visualize training performance.
- **Visualization**: Functions to display input images, target images, and generated images to visually compare the results of the model.

### Workflow:

1. **Data Preparation**: The dataset is automatically downloaded and extracted. Images are preprocessed to prepare them for training.
2. **Model Architecture**: The generator and discriminator networks are defined, with the generator using a U-Net architecture and the discriminator using a PatchGAN architecture.
3. **Training**: The model is trained using a custom training loop, with periodic visualization of the input, target, and generated images to monitor the training progress.
4. **Testing and Visualization**: After training, the model can be tested on new images, and the results can be visualized to assess the performance of the image translation.

### Results

The generated images are compared with the ground truth images to evaluate the effectiveness of the model. The visualizations show the model's ability to translate night images into realistic day images.

