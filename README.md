# CIFAR-100 Classification with ResNet-50
This project, completed as a homework assignment for the Intelligent Data Processing course at the National Research University Higher School of Economics (HSE), demonstrates image classification on the CIFAR-100 dataset using a pretrained ResNet-50 model.

## Overview
- **Dataset:** CIFAR-100 for training and validation; SVHN for testing.
- **Data Augmentation:** Random cropping, horizontal flipping, normalization.
- **Model:** ResNet-50 pretrained on ImageNet, with the final fully connected layer adjusted for 100 classes.
- **Training:** 15 epochs using Adam optimizer and cross-entropy loss.
- **Evaluation:** Tracks training loss, training accuracy, and validation accuracy.

## Results
- **Training:**  
  - Loss: ~1.27  
  - Accuracy: ~62%
- **Validation:**  
  - Loss: ~1.13  
  - Accuracy: ~66%

## Tech Stack
- PyTorch & torchvision
- Torchvision datasets and transforms
- GPU acceleration (CUDA if available)

## Usage
1. Install dependencies:
```bash
pip install torch torchvision matplotlib tqdm
```
2. Run the training script:
```bash
python train_cifar100.py
```
3. The script automatically downloads the datasets and pretrained model weights.

