# ROAD Sign Classification with Keras and Deep Learning

Road sign classification is the process of automatically recognizing traffic signs along the road, including speed limit signs, yield signs, merge signs, etc. Being able to automatically recognize traffic signs enables us to build “smarter cars”.

Self-driving cars need traffic sign recognition in order to properly parse and understand the roadway. Similarly, “driver alert” systems inside cars need to understand the roadway around them to help aid and protect drivers.


## [GTSRB - German Traffic Sign Recognition Dataset](https://www.kaggle.com/meowmeowmeowmeowmeow/gtsrb-german-traffic-sign)
The GTSRB dataset consists of 43 traffic sign classes and nearly 50,000 images.


## **Challenges with the GTSRB dataset:**
1. Images are low resolution, and worse, have poor contrast images are pixelated, and in some cases, it’s extremely challenging, if not impossible, for the human eye and brain to recognize the sign.
2. The dataset is handling class skew: (Imbalanced dataset)
![](https://i.postimg.cc/yxQWHvpW/imbalanced-dataset.jpg)


## **Build a CNN model**
I'll be using keras package to build CNN model. CNN is best for image classification purposes.

The architecture of our model is:

- 2 Conv2D layer (filter=32, kernel_size=(5,5), activation=”relu”)
- MaxPool2D layer ( pool_size=(2,2))
- Dropout layer (rate=0.25)
- 2 Conv2D layer (filter=64, kernel_size=(3,3), activation=”relu”)
- MaxPool2D layer ( pool_size=(2,2))
- Dropout layer (rate=0.25)
- Flatten layer to squeeze the layers into 1 dimension
- Dense Fully connected layer (256 nodes, activation=”relu”)
- Dropout layer (rate=0.5)
- Dense layer (43 nodes, activation=”softmax”)
