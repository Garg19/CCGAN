# CCGAN-CONTINUOUS-CONDITIONAL-GAN
# Introduction
Generative Adversarial Networks (GAN'S) are an approach to generative modeling using deep learning methods, such as convolutional neural networks. GANs are a clever way of training a generative model by framing the problem as a supervised learning problem with two sub-models: the generator model that we train to generate new examples, and the discriminator model that tries to classify examples as either real (from the domain) or fake (generated). The two models are trained together in an adversarial zero-sum game until the discriminator model is fooled about half the time.

Additional information that is correlated with the input images, such as class labels can also be used for the deliberate or targeted generation of images of a given type.CGAN, the conditional GAN is trained to generate images conditioned on labels which are discrete and one hot encoded. We implemented a continuous conditional GAN to generate images conditioned on continuous labels. In this code, we have generated the face images conditioned on age (a continuous variable).

# Input
We have taken the UTKFACE dataset which contains face images with labels consisting of information regarding age and gender. We have divided the dataset into labeled, unlabeled and test set and trained the model on labeled and unlabeled data. We aim to reduce the need of labeled data by introducing comparision data in further improvements.

<p float="left">
  <img src="https://github.com/Garg19/CCGAN/blob/master/UTKFace_input/1_1_0_20170109194032969.jpg.chip.jpg" width="200" />
  <img src="https://github.com/Garg19/CCGAN/blob/master/UTKFace_input/40_0_0_20170117203818313.jpg.chip.jpg" width="200" /> 
  <img src="https://github.com/Garg19/CCGAN/blob/master/UTKFace_input/48_0_3_20170109142337247.jpg.chip.jpg" width="200" /> 
  <img src="https://github.com/Garg19/CCGAN/blob/master/UTKFace_input/67_0_0_20170109002158153.jpg.chip.jpg" width="200" />
</p>

The input images with different age with age increasing from left to right with ages - 1, 40, 48, 67.

# Output
We have uploaded few of the generated face images. The images are conditioned on the age by taking same input vector and different ages with top left corner representing the age 1 year and bottom right representing the age of 60 year. The age is increasing from top left to bottom right. Clearly, we can see the age difference of the images generated by the GAN network.

<p float="left">
  <img src="https://github.com/Garg19/CCGAN/blob/master/outputs/train-0.png" height = "400" width="700" />
</p>

# Conclusion
We can see that the quality of generated images are quite well. The images are conditioned on age and we can see it from the output image generated by taking the same input vector conditioned on different age. We can see the age difference between the top left image and bottom right image and conclude that the generator and discriminator are well trained and generating good quality images conditioned on continuous label - age.
