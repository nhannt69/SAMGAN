# Image-enhanced Generative Models for Industrial Scanning Acoustic Super-resolution (Private)

## Introduction

This project aims to improve the resolution of images obtained from Scanning Acoustic Microscopy (SAM) using Generative Adversarial Networks (GANs). SAM is a non-destructive technique that uses ultrasound waves to investigate the internal properties of a sample. However, SAM images often suffer from low resolution and noise. GANs can help to reconstruct details and enhance the quality of these images.

## Objectives

- Improve the resolution of SAM images.
- Reduce noise and enhance details in the images.
- Generate high-quality images from low-resolution SAM images.

## Method

### Generative Adversarial Networks (GANs)

GANs are a deep learning technique consisting of two models: a Generator and a Discriminator. The Generator creates fake images, while the Discriminator attempts to distinguish between real and fake images. Through training, the Generator learns to produce images that increasingly resemble real images.

### Model Architecture

- **Generator**: Uses a convolutional neural network to enhance the resolution and details of SAM images.
- **Discriminator**: Uses a convolutional neural network to distinguish between original SAM images and enhanced images.

### Training Process

![](https://github.com/NTN-hacker/SAMGAN/blob/main/assets/picture/Image_Release/Image5_TrainingProcess.jpg)

1. **Data Collection**: Use low-resolution SAM images and, if available, corresponding high-resolution images.
2. **Data Preprocessing**: Normalize and break down the images into smaller patches.
3. **Model Training**: Train the Generator and Discriminator simultaneously until the Generator can produce high-quality images from low-resolution images.

## Requirements

- Python 3.9 or higher
- Required libraries: TensorFlow or PyTorch, NumPy, OpenCV, Matplotlib

## Installation

1. **Clone the repository**


2. **Install packages from file**

## Usage
### Training the Model
### Enhancing Images
## Results
Enhanced images will be saved in the output directory. You can compare low-resolution images with the enhanced images to evaluate the model's performance.

<p align="center">
  <img src="https://github.com/NTN-hacker/SAMGAN/blob/main/assets/picture/Github_Result.png" width="350" alt="accessibility text">
</p>

## PSNR Metric Comparison

| Image no. | SRGAN  | Nina-SR | CARN   | RCAN   | EDSR   | ESRGAN | Real-ESRGAN | SAMGAN (Ours) |
|-----------|--------|---------|--------|--------|--------|--------|-------------|---------------|
| 1         | 16.661 | 21.609  | 32.503 | 32.984 | 33.131 | 32.161 | 35.677      | 39.867        |
| 2         | 17.467 | 23.114  | 32.015 | 31.193 | 32.757 | 28.976 | 34.659      | 39.789        |
| 3         | 14.864 | 30.623  | 33.412 | 33.558 | 33.356 | 32.961 | 33.658      | 39.731        |
| 4         | 8.492  | 24.927  | 35.385 | 35.153 | 32.378 | 32.866 | 35.038      | 39.632        |
| 5         | 11.396 | 19.201  | 27.643 | 27.472 | 27.558 | 32.532 | 29.511      | 39.555        |
| ...       | ...    | ...     | ...    | ...    | ...    | ...    | ...         | ...           |
| 123       | 13.858 | 16.123  | 18.622 | 18.114 | 16.650 | 26.533 | 26.197      | 26.813        |
| 124       | 15.345 | 15.386  | 16.006 | 15.769 | 16.693 | 25.940 | 24.801      | 26.804        |
| 125       | 14.760 | 14.857  | 16.663 | 16.068 | 15.272 | 26.165 | 26.325      | 26.725        |
| 126       | 13.600 | 15.258  | 17.073 | 16.578 | 15.418 | 26.346 | 25.720      | 26.645        |
| 127       | 14.478 | 15.925  | 17.195 | 16.602 | 17.115 | 25.911 | 27.107      | 26.349        |
| **Avg**   | 13.717 | 20.284  | 25.230 | 25.976 | 25.934 | 29.414 | 30.630      | 33.978        |

## SSIM Metric Comparison

| Image no. | SRGAN  | Nina-SR | CARN   | RCAN   | EDSR   | ESRGAN | Real-ESRGAN | SAMGAN (Ours) |
|-----------|--------|---------|--------|--------|--------|--------|-------------|---------------|
| 1         | 0.055  | 0.926   | 0.943  | 0.941  | 0.941  | 0.936  | 0.929       | 0.962         |
| 2         | 0.052  | 0.899   | 0.926  | 0.924  | 0.923  | 0.939  | 0.910       | 0.950         |
| 3         | 0.053  | 0.906   | 0.929  | 0.927  | 0.926  | 0.938  | 0.910       | 0.953         |
| 4         | 0.056  | 0.916   | 0.927  | 0.924  | 0.924  | 0.938  | 0.911       | 0.952         |
| 5         | 0.055  | 0.903   | 0.927  | 0.925  | 0.924  | 0.934  | 0.910       | 0.951         |
| ...       | ...    | ...     | ...    | ...    | ...    | ...    | ...         | ...           |
| 123       | 0.085  | 0.718   | 0.752  | 0.745  | 0.733  | 0.803  | 0.750       | 0.834         |
| 124       | 0.094  | 0.756   | 0.767  | 0.760  | 0.744  | 0.793  | 0.753       | 0.838         |
| 125       | 0.083  | 0.704   | 0.723  | 0.713  | 0.701  | 0.799  | 0.719       | 0.816         |
| 126       | 0.100  | 0.711   | 0.738  | 0.732  | 0.720  | 0.792  | 0.748       | 0.841         |
| 127       | 0.088  | 0.743   | 0.758  | 0.753  | 0.732  | 0.784  | 0.749       | 0.836         |
| **Avg**   | 0.102  | 0.832   | 0.852  | 0.851  | 0.849  | 0.862  | 0.842       | 0.906         |


## Deploy


<p align="center">
  <img src="https://github.com/NTN-hacker/SAMGAN/blob/main/assets/picture/Image_Release/Image7_Flowchart_DeployModel.jpg" width="350" alt="accessibility text">
</p>

1. Deploy on Website: [Website] (https://demoai-2024.github.io/ohlabs-ai/) (Public - only demo) and Private to use local
2. Deploy on Software
## Contributing
If you would like to contribute to this project, please fork the repository and submit a pull request. All contributions and suggestions are welcome!

## Acknowledgement
Thanks for all the contributors.

## License
Please see the LICENSE file for more details.

## Contact
If you have any questions, please contact us at nguyennhan8521@gmail.com and doanvuhoangminh@gmail.com
