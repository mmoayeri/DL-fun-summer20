# DL-fun-summer20
Some one off experiments in deep learning during my summer off

All code was written in python 3.6 with pytorch framework and was developed using Google Colab, which allows for free GPU access (thanks Google!). Here are some brief descriptions of each file. 

* **Doggiest Dog**: Here we explore the idea of what happens when if take pretrained networks and modify an input image to maximize the activation on a certain final layer node (e.g. using the network to create an image that the network itself says is the doggiest dog). This ultimately (inadvertently) became an exercise on generating adversarial examples. 

* **Doggiest Dog v2**: Adding in a penalty for changing the original image and also experimenting with using feedback from multiple pretrained networks to see if we can make adversarial examples that fool networks they haven't seen before.

* **MNIST GAN**: Just a GAN, largely from the pytorch tutorial. More GAN experiments to come. 

* **MNIST VAE**: Multiple VAEs for MNIST, as well as some fun with interpolation and varied learning rates of the two loss terms for the VAE.

* **Backprop Method on MNIST**: Revisiting Doggiest Dog, with the idea that a simpler classifier might have less noisy gradients for generation. We also incorporate the idea of training classifiers to have a 'garbage' class so that classifiers can have a means to handle data that they do not recognize as any of their classes.
