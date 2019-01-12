# CNN-plant-disease

One Paragraph of project description goes here

## Description
Our architecture is inspired by the Inception-v2 and v3 architectures that bring several upgrades to the initial GoogLeNet architecture
for increasing the accuracy and reducing the computational complexity. Our architecture is a 34 layers deep CNN adding to each 
convolution a batch normalization (BN) operation. BN a has been proven to speed up convergence and limit overfitting. Besides applying 
BN to GoogleNet, the main difference is that the 5x5 convolutional layers are replaced by two consecutive layers of 3x3 convolutions to
improve computational speed like for the Inception-v3 architecture. 

## Dependency
The codes are based on [caffe](http://caffe.berkeleyvision.org/)

## Dataset
* The [PlantVillage dataset](https://github.com/spMohanty/PlantVillage-Dataset) used has has 38 crop-disease pairs, with 26 types of diseases for 14 crop plants.
* In order to train the purely disease classifier with the model using vernacular disease names, the leaf samples of PV dataset are first categorized into 21 classes (20 diseases and one healthy class).
These 21 classes are listed in  ```target_class.txt```

## Installation and Running

1. Users are required to install [Caffe](https://github.com/BVLC/caffe) Library.

2. The train_val.prototxt and solver.prototxt are provided and can be found in the  ```codes``` folder.


## Feedback
Suggestions and opinions of this work (both positive and negative) are greatly welcome. Please contact the authors by sending email to ``` adeline87lee@gmail

## Lisense
BSD-3, see ``` LICENSE ``` file for details.
