# ResNet-18 From Scratch on CIFAR-10

This project implements **ResNet-18 from scratch** and trains it on the **CIFAR-10 dataset** using PyTorch.  
The focus is on understanding residual blocks, skip connections, and building a deep convolutional network without relying on pre-trained weights.

---

## Project Overview

**Objective:**  
Train a ResNet-18 network from scratch on CIFAR-10 and achieve high classification accuracy.

**Dataset:**  
- CIFAR-10 (10 classes: plane, car, bird, cat, deer, dog, frog, horse, ship, truck)
- Training: 70% of data  
- Validation: 30% of training data  
- Test: 10,000 images

**Architecture:**  
- **Residual Blocks**: Two convolutional layers with batch normalization and skip connections.  
- **ResNet-18**: Initial 7x7 convolution, 4 stages of residual blocks, final fully connected layer.  

**Training Details:**  
- Optimizer: Adam  
- Loss Function: CrossEntropyLoss  
- Batch Size: 128  
- Learning Rate: 0.001  
- Weight Decay: 1e-4  
- Epochs: 10  
- Learning Rate Scheduler: StepLR (step_size=2, gamma=0.5)

---


## Results

- The model demonstrated good generalization on CIFAR-10.  
- Training and validation accuracy increased steadily, confirming effective learning.  
- Example prediction on a random test image:
