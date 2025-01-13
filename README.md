# Super Resolution with U-Net

## Overview

This project implements a Super Resolution (SR) model using the `U-Net` architecture to upscale low-resolution images. The aim is to restore high-resolution details from downscaled images, specifically improving image quality after resizing. The task is performed using a dataset where images are resized down by a factor of 4 (from 256x256 to 64x64) and then reconstructed to their original resolution using a `U-Net` model.

## Evaluation Metrics

**Peak Signal-to-Noise Ratio (PSNR)**: Measures the quality of the reconstructed image compared to the original.

## Task

The task is to:

1. **Generate the dataset**: Create input images by resizing the original 256x256 images down to 64x64 and use these as inputs to the model. The original 256x256 images are used as the target output for training.

2. **Implement U-Net**: Build a U-Net model that takes the low-resolution images (64x64) as input and outputs high-resolution images (256x256) without using skip connections.

3. **Compare Models**: Implement two versions of the U-Net:

- One without skip connections.
- One with skip connections, as in the traditional U-Net.

4. **Train & Evaluate**: Train and test the models, compare their results, and measure performance using appropriate metrics.

## Usage

1. Clone the repository.

```sh
git clone https://github.com/linhlinhle997/domain-conversion-unet.git
cd domain-conversion-unet
```

2. Open and run the provided super_resolution_image_unet.ipynb notebook file to train, test, and evaluate the model on the dataset.

## Result

After training, the notebook will display visualizations of the results for both models, comparing their performance.
