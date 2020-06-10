# DL-fun-summer20
Some one off experiments in deep learning during my summer off

All code was written in python 3.6 with pytorch framework and was developed using Google Colab, which allows for free GPU access (thanks Google!). Here are some brief descriptions of each file. 

* **Doggiest Dog**: Here we explore the idea of what happens when if take pretrained networks and modify an input image to maximize the activation on a certain final layer node (e.g. using the network to create an image that the network itself says is the doggiest dog). This ultimately (inadvertently) became an exercise on generating adversarial examples. View on colab [here.](https://colab.research.google.com/drive/12zs9AXlAOVPCvNCrVV3gVPBAzeNe6VmY?usp=sharing)

* **Doggiest Dog v2**: Adding in a penalty for changing the original image and also experimenting with using feedback from multiple pretrained networks to see if we can make adversarial examples that fool networks they haven't seen before. View on colab [here.](https://colab.research.google.com/drive/12FhCAa5T78EqRGimXxL-6HVo7jgcN5rM?usp=sharing)

* **MNIST GAN**: Just a GAN, largely from the pytorch tutorial. More GAN experiments to come. View on colab [here.](https://colab.research.google.com/drive/1Z3PlGUPkxLVRPeg5Ag8iO_mb-w8GF1_z?usp=sharing)

* **MNIST VAE**: Multiple VAEs for MNIST, as well as some fun with interpolation and varied learning rates of the two loss terms for the VAE. View on colab [here.](https://colab.research.google.com/drive/1KEZB6vre4w-L3gjBDnIT3SVhBHldIOrg?usp=sharing)

* **Backprop Method on MNIST**: Revisiting Doggiest Dog, with the idea that a simpler classifier might have less noisy gradients for generation. We also incorporate the idea of training classifiers to have a 'garbage' class so that classifiers can have a means to handle data that they do not recognize as any of their classes. View on colab [here.](https://colab.research.google.com/drive/1Lag0TbeW6ZzRpuwXlh28SuCKDbe1haIP?usp=sharing)

Note: some outputs are hidden when viewing on github so I added links that allow you to view the files on colab above. Also, I used an image of my dog Rainier in some of the files above. You can just upload your own image instead on colab if you want to recreate these results.
