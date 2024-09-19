Sign Language Translator - SignSense
SignSense is a project aimed at bridging the communication gap between the hearing and deaf communities by converting sign language into readable text. This repository contains two versions of the model:

Real-Time Sign Language Translator (using 4 Python scripts)
Static Image Sign Language Translator (Streamlit application using a Keras model)
Table of Contents
Project Overview
Features
Real-Time Model
How It Works

Static Image Model
How It Works

Requirements
Contributors
Project Overview
SignSense uses a machine learning model to recognize hand signs from American Sign Language (ASL) and convert them into readable text. This project promotes inclusivity by enabling easier communication between people who use sign language and those who don't.

Features
Real-Time Translation: Uses your webcam to capture hand signs and converts them to text in real-time.
Static Image Prediction: Allows users to upload images of hand signs and translates them into text.
Alphabet & Common Words Mapping: Maps hand gestures to letters of the alphabet and a few frequently used words.
Streamlit UI: A user-friendly interface to upload images and view results.
Feedback Mechanism: Collects user feedback for further improvements.
Real-Time Model
How It Works
The real-time model captures video from your webcam and processes frames to detect hand landmarks using the Mediapipe library. It then predicts the corresponding letter or word using a RandomForestClassifier trained on hand landmarks data.

The model processes:

Hand detection using Mediapipe’s Hand Landmark Model.
Prediction of hand signs using a RandomForest model.

Static Image Model
How It Works
The static image version uses Keras to load a pre-trained CNN model that predicts the hand sign in uploaded images. The Streamlit app provides an interactive interface for users to upload images of hand gestures, and the model predicts the corresponding letter or word.

OpenCV
Mediapipe
Keras
Numpy
Scikit-learn
Streamlit

Contributors
Aashay Jadhav

With these two variations of the model, SignSense enables both real-time and static image-based sign language translation, making communication easier for all.
