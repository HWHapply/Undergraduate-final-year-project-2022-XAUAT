# Research on Image Generation Algorithm based on Variational Auto-Encoder

## Abstract:
Variational Auto-Encoder is one of the most widely used generative models in unsupervised
learning, and is a variant of Auto-Encoder. VAE can effectively encode high-dimensional image data
into a distribution of low-dimensional features, then obtain the feature vector by sampling and use it
to generate new samples, which has important application prospects in the fields of image generation
and image denoising.

## Code discription:
Currently, the encoders and decoders of variational self-encoders are mostly implemented using
multi-layer perceptrons. Since the image samples are mostly two-dimensional multi-channel data,
multi-layer perceptrons are often ineffective in mining the deeper features of the image data and using
them to generate new samples of high quality. Therefore, this paper applies a VAE model based on a
convolutional neural network, explores the distribution of data features in the hidden layer using
MNIST data, and investigates the effect of different model parameters on the model generation
capability and the best model training strategy using the CIFAR10 dataset. Finally, to address the
problem that the standard normal distribution is too simple, four samplers including Gaussian mixture
sampler, two-stage VAE sampler, MAF sampler and IAF sampler are applied to the generation stage
of the model in this paper, and new samples are generated and evaluated on MNIST and CelebA
datasets, which finally improve the generation capability of the model effectively.
