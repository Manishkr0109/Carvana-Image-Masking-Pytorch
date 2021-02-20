# Semantic-Segmentation UNet

## Overview

### Data
The original dataset is from Kaggle Carvana Image Masking Challenge, and I've downloaded it and done the pre-processing.

You can find the dataset at https://www.kaggle.com/c/carvana-image-masking-challenge/data


### Model
<br> 
<br>
<img src="https://github.com/Manishkr0109/Carvana-Image-Masking-Pytorch/blob/main/results/unet.png" title="Anchor_generator" width=90%/>

<br><br>

This deep neural network is implemented with Pytorch functional API, which makes it extremely easy to experiment with different interesting architectures.

Output from the network is a 256*256 which represents mask that should be learned. Sigmoid activation function makes sure that mask pixels are in [0, 1] range.

### Training
The model is trained for 10 epochs.

After 10 epochs, calculated accuracy is about 98.2 %.

Loss function for the training is BCEWithLogitsLoss (Sigmoid layer and the Binary Cross Entropy Loss in one single class).


### Dependencies
This tutorial depends on the following libraries:

* Torch 1.6.0+ 
* torchvision 0.7.0+ 
* PIL 
* matplotlib 
* Python versions 3.5+.

Run Carvana_UNet.ipynb
You will see the predicted results in evaluation section in Carvana_UNet.ipynb

### Results
Use the trained model to do segmentation on test images, the result is statisfactory.
Here are some results:

<br> 
<br>
<img src="https://github.com/Manishkr0109/Carvana-Image-Masking-Pytorch/blob/main/results/1.png" title="Anchor_generator" width=90%/>

<br><br>

<br> 
<br>
<img src="https://github.com/Manishkr0109/Carvana-Image-Masking-Pytorch/blob/main/results/2.png" title="Anchor_generator" width=90%/>

<br><br>

<br> 
<br>
<img src="https://github.com/Manishkr0109/Carvana-Image-Masking-Pytorch/blob/main/results/3.png" title="Anchor_generator" width=90%/>

<br><br>

<br> 
<br>
<img src="https://github.com/Manishkr0109/Carvana-Image-Masking-Pytorch/blob/main/results/4.png" title="Anchor_generator" width=90%/>

<br><br>

<br> 
<br>
<img src="https://github.com/Manishkr0109/Carvana-Image-Masking-Pytorch/blob/main/results/5.png" title="Anchor_generator" width=90%/>

<br><br>

<br> 
<br>
<img src="https://github.com/Manishkr0109/Carvana-Image-Masking-Pytorch/blob/main/results/6.png" title="Anchor_generator" width=90%/>

<br><br>

<br> 
<br>
<img src="https://github.com/Manishkr0109/Carvana-Image-Masking-Pytorch/blob/main/results/7.png" title="Anchor_generator" width=90%/>

<br><br>

