# Image and Video Dehazing Using Deep Learning
## Overview
This project involves the use of deep learning techniques for image and video dehazing. The primary goal is to remove haze from images and videos, thus improving their clarity and visibility. The models used in this project include a U-Net architecture for image dehazing and a GAN-based architecture for video dehazing. We have evaluated the models based on performance metrics like PSNR (Peak Signal-to-Noise Ratio) and SSIM (Structural Similarity Index).

## Table of Contents
Project Structure
Dataset
Methodologies

## Project Structure
├── data/
│   ├── clear/           
│   ├── hazy/           
│   ├── trans/          
├── models/
│   ├── unet/           
│   ├── gan/             
├── scripts/
│   ├── train_unet.py   
│   ├── train_gan.py 
├── results/
│   ├── dehazed_images/  
│   ├── dehazed_videos/ 
└── README.md
## Dataset
The dataset consists of three folders:

clear: Contains clear images/videos that serve as ground truth.
hazy: Contains hazy images/videos used as input to the models.
trans: Contains transmission maps, optionally used for video dehazing.
Data Source:
## Link to dataset 
For images: Use RESIDE dataset.
LINK: https://www.kaggle.com/datasets/balraj98/indoor-training-set-its-residestandard
For videos: Use Real Haze Video Database
LINK: https://jingnantes.github.io/acmmm21-youku-v1k/
## Methodologies
1. Image Dehazing:
Model: U-Net architecture.
Input: Hazy images.
Output: Dehazed images.
Loss Function: Mean Squared Error (MSE).
Evaluation Metrics: PSNR, SSIM.
2. Video Dehazing:
Model: GAN (Generative Adversarial Network).
Input: Hazy video frames.
Output: Dehazed video frames.
Loss Function: Adversarial loss, Reconstruction loss.
Evaluation Metrics: PSNR, SSIM.


Training the Model
1. U-Net for Image Dehazing
To train the U-Net model for image dehazing, run the following script:


2. GAN for Video Dehazing
To train the GAN model for video dehazing, use the following command:


