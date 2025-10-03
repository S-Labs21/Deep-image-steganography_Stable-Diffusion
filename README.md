# Deep Image Steganography using Stable Diffusion
An approach to image steganography leveraging Stable Diffusion models to seamlessly hide secret images within cover images while maintaining visual quality.
Overview
This project implements a deep learning-based steganography system that uses Stable Diffusion's latent space manipulation to embed secret images into cover images. The method achieves remarkable imperceptibility with an SSIM score of 0.9982 and MSE of 0.4282, making the hidden content virtually undetectable to the human eye.


## Key Features:

- High Visual Quality: Achieves SSIM ranging from 0.9982 to 0.9644
- Low Distortion: MSE of 0.4282 ensures minimal visible artifacts
- Stable Diffusion Integration: Leverages pre-trained diffusion models for robust embedding
- Reversible Process: Complete recovery of both cover and secret images


## Output
<img width="1768" height="618" alt="Output" src="https://github.com/user-attachments/assets/9b9c4fff-ec4f-441f-a4ff-aba8b2d07a39" />

## Architecture

The system consists of three main components:
1. Encoder Network

Processes cover and secret images through Stable Diffusion's VAE
Manipulates latent representations to embed secret information
Preserves semantic content of the cover image

2. Stable Diffusion Integration

Utilizes pre-trained diffusion model weights
Leverages learned image priors for natural-looking outputs
Maintains consistency with training data distribution

3. Decoder Network

Extracts hidden images from stego images
Reconstructs both cover and secret images with high fidelity
Implements attention mechanisms for precise recovery

### Dataset
Flickr-8k - https://paperswithcode.com/dataset/flickr-8k
