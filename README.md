# GANasso - Generative Adversial neural network Picasso
Pytorch implementation of conditional Generative Adversarial Networks (cDCGAN) and Auxiliary Classifier Generative Adversial Networks (ACDCGAN) for MNIST [2] and Kaggle dataset

* The network architecture (number of layer, layer size and activation function etc.) of this code differs from the paper.

* CelebA dataset used gender lable as condition.

* If you want to train using cropped CelebA dataset, you have to change isCrop = False to isCrop = True.

* you can download
  - MNIST dataset: http://yann.lecun.com/exdb/mnist/
  - Kaggle dataset
  
## Development Environment

* Windows 10
* NVIDIA GTX 1070
* cuda 8.0
* Python 3.5.6
* pytorch 0.1.12
* torchvision 0.1.8
