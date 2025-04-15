# AI Interview Training Model - Visual-Feature Detection Module
AI Interview Training System - Visual Feature Detection Model

This module is one part of the AI Interview Training System project. The proposed system (AI Interview Training System) will be able to identify and provide feedback on the user’s behaviour by analyzing the visual and audio features extracted from video data collected during the mock interview to analyse the personality traits of the users.

This part covers the Visual Feature Detection Module. It is a machine learning model trained using the First Impression(FI) Dataset by ChaLearn, which is a large publicly available dataset on the topic, suitable to study apparent personality by deep learning strategies. 

For the visual feature detection module, we will be using Visual Geometry Group-16 (VGG-16) neural network and Long Short-Term Memory (LSTM). VGG-16 is a convolu-tional neural network that is 16 layers deep. The pre-trained version of the network is trained on data from the ImageNet challenge and obtains a 92.7% accuracy when tested on this dataset. LSTM is a variety of recurrent neural networks (RNN) that are capable of learning long-term dependencies, especially in sequence prediction problems. 

In the visual feature detection module, the input to the module is the first impressions data set, which comprises 10000 clips (average duration 15s) extracted from more than 3,000 different YouTube high-definition (HD) videos of people facing and speaking in English to a camera. 

The videos are split into training, validation and test sets with a 3:1:1 ratio. From this video dataset, we extract 15 frames from each video, to be used for the training of the model. These frames are fed into a VGG16 model for model training. In this project, we will be using Transfer Learning on the VGG16 CNN model, to make predictions on our data. The VGG16 model is a CNN architecture that has been pre-trained on the ImageNet dataset. This will enable us to get more accurate results, as well as faster training of our module. 

The output from the VGG16 model will then be fed into a LSTM model to extract the temporal features. Finally, the audio and video model’s output will be combined to output the final personality labels for each video.
