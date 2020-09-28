# CCGAN-CONTINUOUS-CONDITIONAL-GAN
# Introduction
Generative Adversarial Networks (GAN'S) are an approach to generative modeling using deep learning methods, such as convolutional neural networks. GANs are a clever way of training a generative model by framing the problem as a supervised learning problem with two sub-models: the generator model that we train to generate new examples, and the discriminator model that tries to classify examples as either real (from the domain) or fake (generated). The two models are trained together in an adversarial zero-sum game until the discriminator model is fooled about half the time.

Additional information that is correlated with the input images, such as class labels can also be used for the deliberate or targeted generation of images of a given type.CGAN, the conditional GAN is trained to generate images conditioned on labels which are discrete and one hot encoded. We implemented a continuous conditional GAN to generate images conditioned on continuous labels. In this code, we have generated the face images conditioned on age (a continuous variable).

# Input
We have taken the UTKFACE dataset which contains face images with labels consisting of information regarding age and gender. We have divided the dataset into labeled, unlabeled and test set and trained the model on labeled and unlabeled data. We aim to reduce the need of labeled data by introducing comparision data in further improvements.

# Output


