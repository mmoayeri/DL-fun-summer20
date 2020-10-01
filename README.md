# DL-fun-summer20
Some one off experiments in deep learning during my summer off

All code was written in python 3.6 with pytorch framework and was developed using Google Colab, which allows for free GPU access (thanks Google!). Here are some brief descriptions of each file. 

* **Doggiest Dog**: Here we explore the idea of what happens when if take pretrained networks and modify an input image to maximize the activation on a certain final layer node (e.g. using the network to create an image that the network itself says is the doggiest dog). This ultimately (inadvertently) became an exercise on generating adversarial examples. View on colab [here.](https://colab.research.google.com/drive/12zs9AXlAOVPCvNCrVV3gVPBAzeNe6VmY?usp=sharing)

* **Doggiest Dog v2**: Adding in a penalty for changing the original image and also experimenting with using feedback from multiple pretrained networks to see if we can make adversarial examples that fool networks they haven't seen before. View on colab [here.](https://colab.research.google.com/drive/12FhCAa5T78EqRGimXxL-6HVo7jgcN5rM?usp=sharing)

* **MNIST GAN**: Just a GAN, largely from the pytorch tutorial. More GAN experiments to come. View on colab [here.](https://colab.research.google.com/drive/1Z3PlGUPkxLVRPeg5Ag8iO_mb-w8GF1_z?usp=sharing)

* **MNIST VAE**: Multiple VAEs for MNIST, as well as some fun with interpolation and varied learning rates of the two loss terms for the VAE. View on colab [here.](https://colab.research.google.com/drive/1KEZB6vre4w-L3gjBDnIT3SVhBHldIOrg?usp=sharing)

* **CIFAR GANs**: These files were too big for me to post :/ but in short, I looked at DCGANs, GANs based on MLPs, and Wasserstein GANs. Surprisingly, the MLP based GANs did the best. Take a look for your self on colab [here.](https://colab.research.google.com/drive/1Zle4KCFe5vtpetyp0W3MzzwG7PUTXujL?usp=sharing)

* **Backprop Method on MNIST**: Revisiting Doggiest Dog, with the idea that a simpler classifier might have less noisy gradients for generation. We also incorporate the idea of training classifiers to have a 'garbage' class so that classifiers can have a means to handle data that they do not recognize as any of their classes. View on colab [here.](https://colab.research.google.com/drive/1Lag0TbeW6ZzRpuwXlh28SuCKDbe1haIP?usp=sharing)

* **Bach Harmonizer**: Hadjeres et al had a very cool paper on automatically generating Bach chorales. I attempt to create a harmonizer, that fills in a missing vocal trac (provided the other three). Multiple architectures attempted. Also lots of useful code for processing symbolic music. View on colab [here.] (https://colab.research.google.com/drive/1NJhDO9xuxn6MG3jx_gVNv8k9dpDFaQKg?usp=sharing)

* **Deterministic AE**: A recent ICLR paper suggested removing the KLD loss and turning VAEs into deterministic AEs does not compromise performance (if a regularizer is used). Deterministic AEs would be great for the motif detection I will pursue later so I experimented with a number of variants on autoencoder structures and losses. View on colab [here.] (https://colab.research.google.com/drive/1kBh3ipmtdowT6UCYDi3uvXHAoqqlKNS5?usp=sharing)

* **Modeling functions with small NNs**: Quick experiment to investigate how width and depth effect ability of a NN to model different functions from R to R. Also looks at generalizability by means of visualizing results. View on colab [here.] (https://colab.research.google.com/drive/111ysDskEkSTE-t_WUi3HG_q3sIxp_M2S?usp=sharing)

* **Bottleneck MLP**: For simple classification tasks, visualizes representations of inputs at various levels of depth in the network. The visualization was facilitated by having interspersed layers with only two nodes. The observed result was that inputs from the same class become progressively more and more separable as training progresses. Separability is also higher in deeper layers. View on colab [here.] (https://colab.research.google.com/drive/1G7GJQDUDLlv7Fsv1CuGKgXnLCdkoZp0L?usp=sharing

* **Distance b/w Feature Maps** : Investigating how information propagates through networks, in particular looking to see if items in the same class end up closer to one another as we get deeper into the network. Inspired by results of BottleneckMLP and also previous work in neural perceptual distance (LPIPS, Perceptual Threat Model). View on colab [here.] (https://colab.research.google.com/drive/1WUJ4sdKI37yqhT6VELbitZNG4eg8Cq3n?usp=sharing)



Note: some outputs are hidden when viewing on github so I added links that allow you to view the files on colab above. Also, I used an image of my dog Rainier in some of the files above. You can just upload your own image instead on colab if you want to recreate these results.
