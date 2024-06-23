# Image-compression_using_neural_networks
This project focuses on converting images to a lower number of neurons and then regenerating the images from these neurons using an AutoEncoder neural network architecture. An AutoEncoder consists of two main components: an Encoder and a Decoder. Below is a detailed overview of the architecture and methodology used in this project.

# Project Overview
The primary goal of this project is to compress images and then accurately reconstruct them. The dataset used for this project is the MNIST dataset, which contains images of handwritten digits. Two neural network architectures were utilized for this compression and reconstruction process:
# 1. Using Feedforward neural networks:
  + Compression: The images are first flattened and then compressed in the Encoder. The images are compressed to 25% of their original size.
  + Reconstruction: The compressed images are then regenerated through the Decoder. 
  + Results: Below, you can see a comparison of the original images and their regenerated versions.

    ![github_pic1](https://github.com/algezoly7/Image-compression_using_neural_networks/assets/63818969/4160dcf7-8da2-42ba-8c5d-7bdad073b53d)

# 2. Using CNNS:
  + Compression: The Encoder uses a Convolutional Neural Network with max-pooling to initially compress the images. This architecture is then flattened into a feedforward neural network to achieve maximum compression. The middle hidden layer between the Encoder and the Decoder is called the latent space, which consists of neurons that represent and store the image's features.
  + Reconstruction: The Decoder reverses the process, regenerating the images from the compressed representation.
  + Results: Below, you can see a comparison of the original images and their regenerated versions using the CNN architecture. 

# Applications:
  This project can be particularly useful in areas with poor internet connections. The sender can use the Encoder to compress the image and send it to the receiver. The receiver can then decompress the images using the Decoder they have. This method significantly reduces the size of the data being transmitted, making it ideal for low-bandwidth scenarios.
