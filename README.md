# ROAD Sign Classification with Keras and Deep Learning

Road sign classification is the process of automatically recognizing traffic signs along the road, including speed limit signs, yield signs, merge signs, etc. Being able to automatically recognize traffic signs enables us to build “smarter cars”.

Self-driving cars need traffic sign recognition in order to properly parse and understand the roadway. Similarly, “driver alert” systems inside cars need to understand the roadway around them to help aid and protect drivers.

## **Project structure**
    .
    ├── examples [25 entries]          # Contains a random sample of 25 annotated images generated by predict.py
    ├── gtsrb-german-traffic-sign      # GTSRB - German Traffic Sign Recognition Dataset.              
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
    ├── output                          # Contains our output model and training history plot generated by train.py                 
    │   ├── roadsignnet.model           
    │   |   ├── assets           
    │   |   ├── variables            
    │   |   |   ├── variables.data-00000-of-00002
    |   |   |   ├── variables.data-00001-of-00002
    |   |   |   ├── variables.index
    |   |   ├── ├── saved_model.pb
    |   ├── plot.png
    │   └── ...
    ├── cnn                             # A module that comprises our RoadSignNet CNN.
    |   ├── __init__.py
    |   ├──  roadsignnet.py
    ├── train.py
    ├── signnames.csv
    ├── predict.py
    └── ...



## **GTSRB - German Traffic Sign Recognition Dataset**
The dataset we'll be using to train our own custom traffic sign classifier is the German Traffic Sign Recognition Benchmark (GTSRB).



