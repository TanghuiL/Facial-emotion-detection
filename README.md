
Facial expression analysis 

Emotions are the essence of what makes us human. They impact every aspect of our daily life, including attention, perception, memory, decision making and social interaction. Facial expression is usually the foremost display of our emotional state. 

Through evolution, humans become extremely adept in reading faces. In fact, facial recognition is so crucial to human's survial that the human brain has specilized a region called fusiform face area (FFA) for it. In this specialized area, emotional expressions evoke a differential response. 

This near effortless process in humans has been found difficult in computers untill recent progress in computer vision and computational algorithms, which made it possible to mimic the facial recognition skills of humans by closely tracking of the subtle changes in facial features on a moment-by-moment basis. This real time tracking of facial features is considered facial expression analysis (FEA).  


Facial emotion detection system 
This system conducts the facial expression analysis of images through two main steps: 
1. Face detection using a feature-based cascade classifier. 
   >> This classifier is real time and faster in comparison to most face detector. 
   >> Implemented using openCV

2. Emotion detection using Xception CNN model
    >> This CNN model is implemented with Keras


Dataset 
The dataset use here can be download the facial expression recognition (FER) data-set from Kaggle challenge (https://www.kaggle.com/c/challenges-in-representation-learning-facial-expression-recognition-challenge/data). 

The data consists of 48x48 pixel grayscale images of faces. The faces have been automatically registered so that the face is more or less centered and occupies about the same amount of space in each image. The task is to categorize each face based on the emotion shown in the facial expression in to one of seven categories (0=Angry, 1=Disgust, 2=Fear, 3=Happy, 4=Sad, 5=Surprise, 6=Neutral).

The dataset contains two columns, "emotion" and "pixels". The "emotion" column contains a numeric code ranging from 0 to 6, inclusive, for the emotion that is present in the image. The "pixels" column contains a string surrounded in quotes for each image. The contents of this string a space-separated pixel values in row major order. The training set consists of 28,709 examples. The dataset only contains the training set from the original dataset provided by Kaggle. 

(Note: The dataset was prepared by Pierre-Luc Carrier and Aaron Courville)

