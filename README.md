# Concrete-Image-Classification
This project classifies surface images of concrete as cracked/not cracked using Convolutional Neural Network

The dataset and images are downloaded from Mendeley Data:
Özgenel, Çağlar Fırat (2018), “Concrete Crack Images for Classification”, Mendeley Data, v1 http://dx.doi.org/10.17632/5y9wdsg2zt.1
Dataset: Concrete Crack Images for Classification
File: Concrete Crack Images for Classification
DOI: http://dx.doi.org/10.17632/5y9wdsg2zt.1#file-c0d86f9f-852e-4d00-bf45-9a0e24e3b932

Using the Pytorch, a Convolutional Neural Network model was trained on the scaled down images of concrete labeled as "Positive" or "Negative" for concrete surfaces with/without crack.
The dataset consists of 40000 concrete surface images split in 20000 images labeled "Positive" and 20000 images labeled "Negative". The images have been reduced in size by pre-processing through notebook named image_process.
A convolutional neural network model is used with two fully connected layers. The first convolutional layer has 1 input channels, 6 output channels, a kernel size of 3 (3x3 filter), and a stride length of 1 pixel. The second convolutional layer has 6 input channels, 16 output channels, a kernel size of 3 (3x3 filter), and a stride length of 1 pixel.
The repository consists of three notebooks:
image_process notebook to pre-process the data and reduce the size of images
concrete_classification_pytorch is the main notebook for the CNN model
post_process_pytorch is used to check the cracking condition of any given concrete surface image.
