Project Title:

CIFAR10 data using Pytorch with 70% acuuracy.

About:

The model used is LeNet with 3 convolutions layer and 2 fully connected layer with padding equals 1 for all the CNN layers.
The learning rate has been adjusted to 0.001 which gives about 72% of validation accuracy and 68.5% of training accuracy.


Dataset used:

The Dataset is used here is the CIFAR10 which essentialy has 10 different classes to predict namely:
'plane', 'car', 'bird', 'cat', 'deer', 'dog', 'frog', 'horse', 'ship', 'truck'. There are 50000 data with the dimension
3 x 32 x 32 which has been further augmented using torchvision's 'transforms' module. The augmentation done here are :

transforms.RandomHorizontalFlip()
transforms.RandomRotation(10)
transforms.RandomAffine(0, shear = 10 , scale=(0.8,1.2))
transforms.ColorJitter(brightness = 0.2, contrast = 0.2, saturation = 0.2)
transforms.ToTensor()
transforms.Normalize((0.5,0.5,0.5),(0.5,0.5,0.5))

Library used:

Torch
Numpy
matplotlib.pyplot
torch.nn
sklearn
torchvision
PIL.ImageOps