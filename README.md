# ResNet-50 on CIFAR-100

This project was completed as a homework assignment for the course **Intelligent Data Processing** at the **National Research University Higher School of Economics (HSE)**. It demonstrates image classification on the **CIFAR-100 dataset** using a pretrained **ResNet-50** model.

## Project Overview

- **Dataset:** CIFAR-100, split into training (80%) and validation (20%) sets.  
  *Note: any mentions of the SVHN dataset in earlier code are artifacts and are not used in this project.*
- **Model:** Pretrained ResNet-50 with the final fully connected layer adapted to 100 classes.
- **Loss Function:** CrossEntropyLoss.
- **Optimizer:** Adam with learning rate 0.001.
- **Training:** 15 epochs with standard data augmentation (random crop, horizontal flip) and normalization.
- **Validation:** Accuracy and loss computed on the validation set.

## Results

After training for 15 epochs, the model achieved:

- **Training Accuracy:** ~62.7%
- **Validation Accuracy:** ~66.7%
- **Validation Loss:** 1.128

The training loss gradually decreases across epochs, demonstrating effective learning.

## Notes

- The project is implemented in PyTorch.
- Uses `torchvision.transforms` for preprocessing and data augmentation.
- Training is performed on GPU if available.
