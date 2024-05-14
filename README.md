# Malaria-Image-Classification

The aim of this project is to use a deep learning model to classify bloodslides as either being healthy or infected. The model used is ResNet50, which is known for high performance with medical images.

## Table of Contents
1.	Setup
2.	EDA
3.	Preprocessing
4.	Modelling
5.  Conclusion	

## EDA & Preprocessing

The dataset comprises of 27,000+ Images from the inbuilt Tensorflow Malaria dataset. The dataset is split into train, test and val set in the ratio 80,10,10.

For preprocessing, the images are resized, the labels one hot encoded and batched to make sure they are in the format the ResNet model will accept.

## Modelling. 
The first model has a Resnet50V2 architecture. It performs fairly, with a test loss of.47 and a test accuracy of .78.
The second model is a tuned version of the first model. This has been achieved by augmenting the train data and unfreezing some layers in the model. Although it registers a lower test loss of .15 and higher accuracy of .95, it shows more overfitting. 


## Conclusion
Additional steps could include:

- Experimenting with the layers being frozen and the order of the layers being frozen
- Experimenting with different deep models.
- Using heavier data augmentation

  
## Dependencies
•	Python 3.x
•	TensorFlow
•	Keras
•	Matplotlib
•	NumPy

