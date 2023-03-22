# Deep-Learning-Projects
A collection of projects &amp; papers that I've in implementing in PyTorch


## Vesuvius Challenge - detecting ink in ancient papyrus scrolls

## Auto-encoder for MNIST
![autoencoder-diagram](/Images/autoencoder-diagram.png)

Result from linear layer autoencoder, composed of Linear, BatchNorm1D and ReLU layers.

Epoch: 240 | Train loss: 1255.1389 | Test loss: 1293.0311 | Time elapsed: 90.7 seconds.

Reconstructions:

![autoencoder-reconstructions-linear](/Images/autoencoder-reconstructions-linear.png)

Modifying architecture to follow a "vgg style", albeit much smaller.

encoder block layers: Conv2d,ReLU,BatchNorm2d,Conv2d,RelU,BatchNorm2d,MaxPool

decoder block layers: UpSample,Conv2d,ReLU,BatchNorm2d,Conv2d,ReLU,BatchNorm

Epoch: 90 | Train loss: 982.5375 | Test loss: 988.5124 | Time elapsed: 196.68 seconds

Reconstructions:
![autoencoder-reconstructions-vgg](/Images/autoencoder-reconstructions-vgg.png)


## GPT

## UNET
