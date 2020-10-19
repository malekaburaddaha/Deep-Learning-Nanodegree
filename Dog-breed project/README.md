# Dog-Breed-Classifier-Project



In this project, I built a part of a mobile app which classifies dog pictures where it tells you the breed
of the dog when given a dog picture, and tells you which breed does a human look like when given a human picture 

## 1. Domain Background
The field of Image processing is one of the subfields of machine and deep learning, along with signal processing and many others and it is an active area of research.
This field is based on processing the images via mathematical algorithms and uses those algorithms to accomplish many goals like classification, prediction, and even image generation such as using Adversarial Neural Networks (GANs) for that matter.
There are many goals and benefits of this field in healthcare (Radiology, or skin cancer), In security, such as face recognition, in industry like pattern configuration and so on. 

## 2. Problem Statement
One of the main challenges in the field of image processing is to give the ability for a system to recognize how things look like and what are the differences between them.
Here  we are facing this challenge where we are going to build an algorithm that will be able to distinguish between dogs breeds, and overcome the challenge that many the dogs breeds would look very alike, so we have to build the model where it would be powerful enough to distinguish between the pictures of different dogs, in addition to that we will train it to be able to tell us what breed a human looks like given an image of a human being. 


## 3. Datasets And inputs
The project dataset and input provided by Udacity, and they contain images of dogs
breed and humans, in separate folders , one contains 13233 images of humans , and the
other with 8351 images of dogs .
The dog’s folder divided into folders of validation , test , and train data, each folder
contains images for 133 breeds of dogs, separated into folders using breed name, and
Each breed has a huge number of images.
There are 835 images in the validation set and, 6680 dog images in the training set, And
836 images in the test set.


## 4. Solution statement
We are going to build a model to classify dogs' breed and distinguish the different kinds using a Convolutional Neural Network (CNN) which is the best for image classification and processing. We have two main goals here: the first one is to classify the dog breeds and the second one is to tell what a human image looks like compared with the dog breeds.
In this model we will use the Haar Cascades classifier from the OpenCV library to give the ability of the model to distinguish between a human and a dog and tell which breed does the human look like given an image of a human. On the other hand we are going to use transfer learning technique to build another classifier to distinguish between the dog breeds and I am going to use the VGG16 trained model for this goal. At the end of the project we will have a part of an image app that can distinguish between the dogs and humans, tell the dogs breed, and tell which dog’s breed does a certain human look like. 


## 5. Benchmark Model
We are building two models in two different ways:
● Building a model from scratch that should exceed 10% accuracy, this is a challenging task due to the fact that the images processing models need many iterations and epochs which take a long time to finish training
● The second approach will be to build a model using a pre-trained model which, this model should achieve more than 60%, and it should not be very hard since we are using a pre-trained model which has been trained with more many epochs with a massive amount of data for a long time. 


## 6. Evaluation Metrics
The project evaluation metric for this project is the accuracy. Based on the accuracy we will be able to determine the level proficiency for the model performance on classifying the pictures.
The accuracy will be determined as follows:
Accuracy = ( The number of correctly classified images / The total number of images ) x 100


## 7. Project Design
The design steps of this project are as follows: 
1. Importing Datasets as provided by Udacity
2. Detecting Humans: by using OpenCV’s implementation of Haar feature-based cascade
classifiers.
3. Detecting Dogs: by using pre-trained models (VGG-16 ) from the Image Net competition.
4. Classifying dog breeds: via preprocessing our images  (rotating, resizing, cropping, etc...) and training the model for a sufficient number of epochs to obtain the desired results.
5. The last step will be to test a few images (dogs and human pictures) of our own choice and see how the model will perform. 



## Suggested Improvement

This project can be improved as follow:
1. Considering training the model with more number of epochs which could make an
improvement.
2. Considering more image augmentation that would make an improvement.
3. Considering more improvement of the accuracy of the model by adding more layers
or editing any of the model’s parameters such as the learning rate, optimizing function.
