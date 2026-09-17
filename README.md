# Classification of MNIST Digits with Convolutional Neural Networks

A CNN classifier for MNIST handwritten digits, comparing convolutional feature extraction against the earlier Dense/MLP approach.

> Note: despite this repo's name, the notebook here classifies MNIST digits with a CNN, not CIFAR-10/100.

![CNN model architecture](<https://raw.githubusercontent.com/MikeFerko/Classification-of-CIFAR-10-and-100-with-Convolutional-Neural-Networks/main/Lab%204-MODEL-CNN.JPG>)

- [Notebook](<LAB 4-Classification with CNN.ipynb>)

## Approach

- Built a CNN (Conv2D 8@9x9 to MaxPool to Conv2D 16@5x5 to MaxPool to Flatten to Dense 16 to Dense 10 softmax) trained with Adam and categorical cross-entropy
- Trained for 25 epochs at batch size 128, tracking both loss and accuracy across training and validation
- Visualized low-level and high-level convolutional feature maps for sample digits to see what each layer learns
- Compared parameter count and accuracy against the earlier Dense/MLP classifier from the MNIST classification project
