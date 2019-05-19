# GANasso - Generative Adversial neural network Picasso
Pytorch implementation of conditional Generative Adversarial Networks (cDCGAN) and Auxiliary Classifier Generative Adversial Networks (ACGAN) for MNIST and Kaggle dataset

* report folder contains a report of this implementation. Look that if you want to get more deep into details

* We used both cDCGAN and ACDCGAN to create new paintings from total of 4 different labels.

* you can download
  - MNIST dataset: http://yann.lecun.com/exdb/mnist/
  - Kaggle dataset: http://academictorrents.com/details/1d154cde2fab9ec8039becd03d9bb877614d351b
  
## Results

## Resutls
### MNIST and two labels
* Generate using fixed noise (fixed_z_). Epochs for mnist are 10 and for two labels are 80

<table align='center'>
<tr align='center'>
<td> MNIST</td>
<td> Two labels from our dataset <td>
</tr>
<tr>
<td><img src = 'gifs/mnist.gif'>
<td><img src = 'gifs/2labels.gif'>
</tr>
</table>

* MNIST vs Generated images

<table align='center'>
<tr align='center'>
<td> MNIST </td>
<td> cGAN after 50 epochs </td>
<td> cDCGAN after 20 epochs </td>
</tr>
<tr>
<td><img src = 'MNIST_cGAN_results/raw_MNIST.png'>
<td><img src = 'MNIST_cGAN_results/MNIST_cGAN_50.png'>
<td><img src = 'MNIST_cDCGAN_results/MNIST_cDCGAN_20.png'>
</tr>
</table>

* Learning Time
  * MNIST cGAN - Avg. per epoch: 9.13 sec; Total 50 epochs: 937.06 sec
  * MNIST cDCGAN - Avg. per epoch: 47.16 sec; Total 20 epochs: 1024.26 sec

### CelebA
* Generate using fixed noise (fixed_z_; odd line - female (y: 0) & even line - male (y: 1); each two lines have the same style (1-2) & (3-4).)

<table align='center'>
<tr align='center'>
<td> cDCGAN</td>
<td> cDCGAN crop</td>
</tr>
<tr>
<td><img src = 'CelebA_cDCGAN_results/CelebA_cDCGAN_generation_animation.gif'>
<td><img src = 'CelebA_cDCGAN_crop_results/CelebA_cDCGAN_crop_generation_animation.gif'>
</tr>
</table>

* CelebA vs Generated images

<table align='center'>
<tr align='center'>
<td> CelebA </td>
<td> cDCGAN after 20 epochs </td>
<td> cDCGAN crop after 30 epochs </td>
</tr>
<tr>
<td><img src = 'CelebA_cDCGAN_results/raw_CelebA.png'>
<td><img src = 'CelebA_cDCGAN_results/CelebA_cDCGAN_20.png'>
<td><img src = 'CelebA_cDCGAN_crop_results/CelebA_cDCGAN_crop_30.png'>
</tr>
</table>


## Development Environment

* Windows 10
* NVIDIA GTX 1070
* cuda 8.0
* Working environment: misc/environment.yml
