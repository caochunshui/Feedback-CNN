# feedbacknet

The code is written in PyTorch, very simple to understand.

Currently, there are still bugs in the feedback part.

- images: storing exmaplar images
- imagenet1000_clsid_to_human.txt: storing image net 1000 class names, for visualization and human understanding purpose
- map_clsloc.txt: did not really use
- simple_test.ipynb: a simple test ipython file to test feedback idea, using a simple fully connected layer
- vgg.ipynb: a test ipython file to test pretrained vgg network and a redefinition vgg network, then check the weights copying from pretrained network to the new defined network
- vgg_feedback.ipynb: the main file, define the vgg feedback network and run a feedback visualization on an examplar image.
