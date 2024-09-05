# Enhancing Resolution in Scanning Acoustic Microscopy using GANs

![](https://github.com/NTN-hacker/SAMGAN/blob/main/assets/picture/Image_Release/Image3_Model_Architecture.jpg)

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

## Deploy


<p align="center">
  <img src="https://github.com/NTN-hacker/SAMGAN/blob/main/assets/picture/Image_Release/Image7_Flowchart_DeployModel.jpg" width="350" alt="accessibility text">
</p>

1. Deploy on Website: [Website] (https://demoai-2024.github.io/ohlabs-ai/)
2. Deploy on Software
## Contributing
If you would like to contribute to this project, please fork the repository and submit a pull request. All contributions and suggestions are welcome!

## License
Please see the LICENSE file for more details.

## Contact
If you have any questions, please contact us at nguyennhan8521@gmail.com and doanvuhoangminh@gmail.com
