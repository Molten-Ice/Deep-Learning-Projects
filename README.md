# Deep-Learning-Projects
A collection of projects &amp; papers that I've in implementing in PyTorch


## Vesuvius Challenge - detecting ink in ancient papyrus scrolls

## Auto-encoder for MNIST

Condensing information into a 10 node bottleneck, through two different model architectures. This dimensional condensed representations of the input images features is then used for train a side neural network, with the weights for the initial model frozen to get predictions for the MNIST dataset.

### Linear model

![autoencoder-diagram](/Images/autoencoder-diagram.png)

Result from linear layer autoencoder, composed of Linear, BatchNorm1D and ReLU layers.

Epoch: 240 | Train loss: 1255.1389 | Test loss: 1293.0311 | Time elapsed: 90.7 seconds.

Reconstructions:

![autoencoder-reconstructions-linear](/Images/autoencoder-reconstructions-linear.png)

Freezing weights and taking outputs from encoder outcome:

Epochs:10, b:0 |Train loss: 0.3078, acc:87.5000 | Test loss: 0.6531, acc: 85.1562 | lr: 0.1

### VGG style model

Modifying architecture to follow a "vgg style", albeit much smaller.

encoder block layers: Conv2d,ReLU,BatchNorm2d,Conv2d,RelU,BatchNorm2d,MaxPool

decoder block layers: UpSample,Conv2d,ReLU,BatchNorm2d,Conv2d,ReLU,BatchNorm

Epoch: 90 | Train loss: 982.5375 | Test loss: 988.5124 | Time elapsed: 196.68 seconds

Reconstructions:
![autoencoder-reconstructions-vgg](/Images/autoencoder-reconstructions-vgg.png)


Freezing encoder weights, and taking output to feed into side neural network outcome:

E:9, b:15 |Train loss: 0.2056, acc:92.7734 | Test loss: 0.2199, acc: 91.5527 | 

### Conclusion

We can see that the losses for the entire model decreases from ~1250 to <1000 by adapting out model architecture, and the corresponding increase in accuracy was seen from 85% to 91% on the train!


## GPT

## UNET
