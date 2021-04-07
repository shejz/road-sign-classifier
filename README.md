# Road Sign Classifier
This project is to classify traffic signs images using Convolutional Neural Networks (CNN).

## **Project structure**

I extracted the dataset into my project directory as you can see here:

- gtsrb-german-traffic-sign/ : **GTSRB** - German Traffic Sign Recognition Dataset.
- output/ : Contains our output model and training history plot generated by **train.py** 
- examples/ : Contains a random sample of 25 annotated images generated by **predict.py** 
- cnn : A module that comprises our RoadSignNet CNN.

    .
    ├── examples [25 entries]
    ├── gtsrb-german-traffic-sign                    
    │   ├── Meta [43 entries]            
    │   ├── Test [12631 entries]             
    │   ├── Train [43 entries]            
    │   ├── meta-1 [43 entries]
    |   ├── test-1 [12631 entries]
    |   ├── train-1 [43 entries]
    |   ├── Meta.csv
    |   ├── Test.csv
    |   ├── Train.csv
    │   └── ...
    ├── output                    
    │   ├── roadsignnet.model           
    │   |   ├── assets           
    │   |   ├── variables            
    │   |   |   ├── variables.data-00000-of-00002
    |   |   |   ├── variables.data-00001-of-00002
    |   |   |   ├── variables.index
    |   |   ├── ├── saved_model.pb
    |   ├── plot.png
    │   └── ...
    ├── cnn
    |   ├── __init__.py
    |   ├──  roadsignnet.py
    ├── train.py
    ├── signnames.csv
    ├── predict.py
    └── ...



 



