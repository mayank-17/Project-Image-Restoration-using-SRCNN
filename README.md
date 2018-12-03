# Project-Image-Restoration-using-SRCNN

The goal of super-resolution (SR) is to recover a high resolution image from a low resolution input.

To accomplish this goal, I will be deploying the super-resolution convolution neural network (SRCNN) using Keras. This network was published in the paper, "Image Super-Resolution Using Deep Convolutional Networks" by Chao Dong, et al. in 2014. You can read the full paper at https://arxiv.org/abs/1501.00092.

As the title suggests, the SRCNN is a deep convolutional neural network that learns end-to-end mapping of low resolution to high resolution images.  As a result, I will be using it to improve the image quality of low resolution images. To evaluate the performance of this network, I will be using three image quality metrics: peak signal to noise ratio (PSNR), mean squared error (MSE), and the structural similarity (SSIM) index.  

Furthermore, I will be using OpenCV, the Open Source Computer Vision Library. OpenCV was originally developed by Intel and is used for many real-time computer vision applications.  In this particular project, I will be using it to pre and post process our images. As we will frequently be converting our images back and forth between the RGB, BGR, and YCrCb color spaces. This is necessary because the SRCNN network was trained on the luminance (Y) channel in the YCrCb color space.  

During this project, following steps were taken: 

* use the PSNR, MSE, and SSIM image quality metrics,
* process images using OpenCV,
* convert between the RGB, BGR, and YCrCb color spaces,
* build deep neural networks in Keras,
* deploy and evaluate the SRCNN network
