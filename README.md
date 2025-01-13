# Image Inpainting with U-Net

## Overview

This project implements an image inpainting model using the `U-Net` architecture. The aim of this task is to restore corrupted images by removing random lines drawn on them and recovering the original content. The dataset used consists of 256x256 color images, and the model takes damaged images as input and outputs restored images.

## Dataset

The dataset consists of images of size 256x256x3, split into training (685 images) and validation (170 images) sets. The input images are corrupted by randomly drawn lines, and the target is the original image without any corruption.

## Evaluation Metrics

**Peak Signal-to-Noise Ratio (PSNR)**: Used to measure the quality of the reconstructed image by comparing it to the original image.

## Task

The task is to:

1. **Create a dataset**: Generate input images by applying random lines on the original images. The target images will be the original, undamaged images.

2. **Build U-Net models**:

- Implement a U-Net model without skip connections.
- Implement a U-Net model with skip connections.

3. **Train and Evaluate**: Train and evaluate both models and compare their performance based on the quality of the reconstructed image.

## Usage

1. Clone the repository:

```sh
git clone https://github.com/yourusername/image-inpainting-unet.git
cd image-inpainting-unet
```

2. Open and run the provided `inpainting_image_unet.ipynb` notebook to train, test, and evaluate the model on the dataset.

3. The notebook will allow you to generate the dataset, build and train the models, and visualize the results.

## Result

After training, the notebook will display visualizations comparing the results of the models, including images before and after inpainting.
