# Feedback Convolutional Neural Network for Visual Localization and Segmentation

The code is an implementation of Feedback Convolutional Neural Network for Visual Localization and Segmentation. The code is written in [PyTorch](https://pytorch.org/), very simple to understand.

There is also a Caffe implementation, please check the [Caffe version](https://github.com/caochunshui/FeedbackCNN-demo) if you are interested.

### Requirement:
- Python 3
- Pytorch 0.4.0

### How to run:

open the ipython notebooks with 

`jupyter notebook`

open `vgg_fr.ipynb` or `vgg_fsp.ipynb`, these are the two main files for demonstrate feedback idea.


### How it looks:

If you run vgg_fsp.ipynb without modification of code, you are supposed to see below visualization:

Input image:

<img src="figure/image.png" width="256">

Image gradient with respect to the target label:

<img src="figure/ff.png" width="256">

Image gradient with respect to the target label after 4 iterations of feedback selective pruning:

<img src="figure/fb_1.png" width="256"> <img src="figure/fb_2.png" width="256"> <img src="figure/fb_3.png" width="256"> <img src="figure/fb_4.png" width="256">

### File explanation:

- vgg_fr.ipynb: the main file that defines the vgg feedback network with the feedback recovering mechanism and run a feedback visualization on examplar images.
- vgg_fsp.ipynb: the main file that defines the vgg feedback network with the feedback selective pruning mechanism and run a feedback visualization on  examplar images.
- images: storing exmaplar images
- imagenet1000_clsid_to_human.txt: storing image net 1000 class names, for visualization and understanding purpose
- test/simple_test.ipynb: test for a simple feedback network, using a simple fully connected structure
- test/vgg_test.ipynb: test for the loading of a pretrained vgg network, then check the weights copying from pretrained network to a new defined network interface
