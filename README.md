# Image Classification with Convolutional Network

In this project, we are going to do image classification/recognition using Convulotional Neural Network that will classify whether the submitted image is a beach, a forest, or a mountain.Image classification has become one of the most influencial innovations in Computer Vision since the first digital image scanner. Developing models that can classify images has made tremendous advances in the way people interact (social media, search engines & image processing), retail (both in person and online), marketing, theatre & the performing arts, government, survelance, law enforcement, etc. Thanks to image classification algorithms we are able to recieve notifications on social media when someone has posted a picture that may look like us, or object recognition in self driving cars. The idea of a program being able to identify meaningful objects in an image and make a judgement as to what it is, what it’s connected with and where it belongs based on only the information found in an image has endless applications. 



## Dependencies

You need to install the pillow package in your conda environment to manipulate image data. Herewith some library that we used for create model, library `imager` use to load the image from the folder.
 

- Data wrangling - library(tidyverse)
- Image manipulation - library(imager) 
- Deep learning - library(keras)
- Model Evaluation - library(caret)


## Convolutional Neural Network (CNN

A CNN is a class of deep learning neural networks that uses a series of filters to extract features from a particular data set, while keeping parameters relatively low. CNNs analyze pixels in groups with their neighbors by sliding filters (or convolving filters) across the pixels of an image. Each filter’s purpose can be to detect various patterns within images. For example, one filter can contribute to detecting eyes in a facial recognition model; another may be responsible for detecting a nose or a mouth. Each filter essentially executes an operation on pixel data and indicates how strongly a particular feature appears in an image, where it is located and it’s frequency. This process reduces the number of parameters the CNN must learn as compared to an MLP, and does not loose spatial information. Filters change as a response to training and therefore initially begin with arbitrary values. Essentially what is being trained are these filters responsible for identifying unique features for each image or image category. Feature maps for each image are generated for each filter and provided to an activation function at the node which determines if a feature is present in a given location. This process is continued with multiple layers throughout the CNN.

In this case, we will build image classification for helping a stock photo website categorizing their image database based on the thematic location. Why is this an important task? You can check how the unsplash, a photo stock website that use deep learning to organize and create tag for each image in their collection, is a challenge for us who wish to learn more about solving problems with unstructured data from a collection of images. The data consists of images with 3 different labels: “Beach”, “Forest”, or “Mountain”. Data were collected by scraping images directly from Google image search.

## Results

### Accuracy before Improvement
![Accuracy Before](https://github.com/rachmaapriyani/capstone-imageclassificationCNN-usingR/blob/main/before_improvement.PNG)
### Accuracy After Improvement
![Accuracy After](https://github.com/rachmaapriyani/capstone-imageclassificationCNN-usingR/blob/main/after_improvement.PNG)
### Leaderboard Score
![LeaderBoard](https://github.com/rachmaapriyani/capstone-imageclassificationCNN-usingR/blob/main/score.PNG)

## Conclusion

CNN implementation for image classification for arbitrary images of beach, forest and mountain is possible with few lines of code. Keras provides a simple way to implement multiple types of CNN architectures and facilitates easy fine tunning of hyperparameters so that models can be easily optimized. Finally I used model improvement to predit the dataset, and the result better than simple model. The accuracy of the improvement model is significantly increase than the simple model after we adjust the architecture of the model, but it took longer time to train due to I used 100 epoch.This does not tells us whether the model specification is optimal, we can still try in obtaining a better model performance using other method or adjusting the network architecture. Many benefit we can take to use machine learning with convolutional neural networks, from this project case we can implement to classify photo collection in the website, users no longer needed to tag photos with labels like beach, forest, or mountain to categorize image content.
