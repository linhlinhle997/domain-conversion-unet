# Image Inpainting and Super Resolution with U-Net

This project demonstrates the use of the `U-Net` architecture for two distinct tasks: **Super Resolution** and **Image Inpainting**. The goal is to restore corrupted images by removing random lines and upscale low-resolution images to their high-resolution counterparts.

## Overview

This repository includes two approaches using the U-Net model:

1. **Super Resolution with U-Net**: Upscales low-resolution images (64x64) to high-resolution images (256x256) using the U-Net model. The task focuses on improving image quality after resizing.

2. **Image Inpainting with U-Net**: Aims to restore corrupted images by removing random lines, using the U-Net architecture. The dataset consists of corrupted 256x256 color images, where the model outputs the original, undamaged images.

## Workflow

For each task, the general workflow is as follows:

1. Load and preprocess the dataset containing images.
2. For **Super Resolution**: Resize the images down to 64x64, then train the U-Net model to restore them back to their original 256x256 resolution.
3. For **Image Inpainting**: Corrupt the images by adding random lines, then train the U-Net model to restore the original images.
4. Evaluate both models using Peak Signal-to-Noise Ratio (PSNR) to measure the quality of the reconstructed images.

## How to Use

1. Clone the repository:

```sh
git clone https://github.com/linhlinhle997/domain-conversion-unet.git
cd domain-conversion-unet
```

2. Open the appropriate notebook file for the desired task:

- `inpainting_image_unet.ipynb` for Image Inpainting.
- `super_resolution_image_unet.ipynb` for Super Resolution.

3. Run the provided script in the notebook to install required dependencies, generate the dataset, and train the model.

## Results

After training, the models will display visualizations comparing the original and reconstructed images for both tasks:

- The **Super Resolution with U-Net** will show the comparison between low-resolution inputs and their high-resolution outputs.

- The **Image Inpainting with U-Net** will show images before and after line removal.

These models highlight the effectiveness of U-Net in both image restoration and upscaling tasks, providing valuable insights into the use of deep learning for image processing.
