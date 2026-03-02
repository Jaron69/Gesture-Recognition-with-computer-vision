# 🤟 Gesture Recognition with MediaPipe & TensorFlow

Real-time Gesturee recognition system using hand landmark detection and deep learning.

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange.svg)
![MediaPipe](https://img.shields.io/badge/MediaPipe-Hands-green.svg)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-red.svg)

## 📌 Overview

This project recognizes hand signs in real-time using a webcam. It extracts **21 hand landmarks** (42 features: x,y coordinates) using **MediaPipe Hands**, then classifies them.

Webcam → MediaPipe (Hand Detection) → Landmark Extraction → Neural Network → Sign Prediction

## 🎯 Features

- Real-time hand sign detection via webcam  
- Custom dataset creation tool for recording your own signs  
- Lightweight neural network for fast inference  
- Scalable — easily add new signs by recording more data  


### Dependencies

opencv-python  
mediapipe  
tensorflow  
numpy  
pandas  
scikit-learn  

### 1. Collect Data


- Position your hand in front of the webcam  
- Each frame captures 21 hand landmarks (42 values: x,y)  
- Data is saved to dataset.csv  

### 2. Train the Model

### 3. Run Real-Time Recognition

Point your hand at the webcam and the predicted sign will be displayed on screen.


## 📊 How It Works

MediaPipe extracts 21 key points from the hand.  
Each landmark provides (x, y) coordinates → 42 features total.

Example data format:

landmarks (42 values) | sign  
0 0 39 -6 60 -29 ...  | peace  
0 0 35 -23 49 -46 ... | kon  



## 🛠️ Improving Accuracy

- Record more frames per sign  
- Vary hand angles & distances  
- Normalize data (StandardScaler)  
- Keep dataset balanced  


