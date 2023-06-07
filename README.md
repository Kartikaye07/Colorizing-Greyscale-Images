# Colorizing_Images

Built and trained an autoencoder neural network in Keras with TensorFlow as backend. Autoencoder stores the input image representation in the latent space with very few dimensions compared to the input image.

The Decoder block of autoencoder consists of an output layer that gives the reconstructed image and some hidden layers, generally a combination of Convolutional Transpose Layers and Upsampling layers. In the Decoder block, the autoencoder learns the reconstruction of the original image from the previously learned latent space.

In this project, tweaked the Autoencoder Neural Network in such a manner that while training, we input Grayscale Images and set the output as their corresponding color images. In this way, the autoencoder layers would learn how to convert the latent space representation of grayscale images into colored images. For the Encoder, chose a pre-trained VGG16 model trained on ImageNet Dataset to classify 1000 classes. For the decoder part of the autoencoder, to upsample the latent representation up to the size of the original image used UpSampling Layers.

The project performed significantly well on converting grayscale images to colored rgb images. Some of the results can be seen below: 
![test_dog_2](https://github.com/Kartikaye07/Colorizing-Greyscale-Images/assets/106856745/a3ff0c61-b2b9-435c-b760-63209cd7611b)
![test_dog_1](https://github.com/Kartikaye07/Colorizing-Greyscale-Images/assets/106856745/bee49c5e-f97d-42db-b0de-11abc475acab)
![test_person_female](https://github.com/Kartikaye07/Colorizing-Greyscale-Images/assets/106856745/a78fefa8-96db-4b82-b828-223919cbc564)
![test_person_male](https://github.com/Kartikaye07/Colorizing-Greyscale-Images/assets/106856745/e6a77833-671b-46c3-8744-87b96647bd4d)
![test_car](https://github.com/Kartikaye07/Colorizing-Greyscale-Images/assets/106856745/b318a787-6bf6-44c0-b558-90f835def651)
