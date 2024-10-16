Driver Drowsiness Detection System
==================================

Overview
--------
The Driver Drowsiness Detection System is designed to detect signs of drowsiness in drivers and prevent accidents by issuing an alert when the driver is detected to be drowsy. The system analyzes a video stream from a camera, detecting closed eyes and other signs of drowsiness. Upon detection, an audio alarm is triggered to wake the driver up.

Features
--------
Real-time face detection and monitoring using a webcam.
Detection of eye closure over time to assess drowsiness.
Triggering of an alarm when the driver shows signs of fatigue or drowsiness.
Uses machine learning for drowsiness classification based on facial landmarks.

Project Structure
-----------------
alarm.wav: A sound file used for the alarm.
drowsiness_detection.py: The main script for the drowsiness detection system.
model.py: Pre-trained machine learning model for detecting drowsiness.
README.txt: This file.

System Requirements
-------------------
Python 3.x
OpenCV (for computer vision tasks)
dlib (for facial landmark detection)
TensorFlow/Keras (for machine learning model)
NumPy

Installation
------------
1. Clone the repository:
https://github.com/naman1824/Driver-Drowsiness


2. Install the required dependencies:
pip install opencv-python dlib tensorflow keras numpy


3. Ensure that your webcam is connected and properly functioning.

How to Use
----------
1. Run the main script to start the detection system:
python drowsiness_detection.py


2. The program will start capturing video from your webcam and monitor your face for signs of drowsiness.

3. If the system detects that your eyes have been closed for a certain period, it will trigger an alarm using the `alarm.wav` file.

Algorithm Explanation
---------------------
The system uses a combination of computer vision and machine learning to detect drowsiness:

1. Face Detection: The program captures real-time video and detects the driver's face.

2. Eye Closure Detection: Using facial landmarks, the system detects the position of the eyes. If the eyes remain closed for longer than a threshold duration, the driver is considered drowsy.

3. Alarm Trigger: If drowsiness is detected, an alarm sound (`alarm.wav`) is played to alert the driver.

Customization
-------------
Adjusting Drowsiness Threshold: You can change the sensitivity of drowsiness detection by adjusting the threshold values in the `drowsiness_detection.py` file.

Custom Alarm: To use a different alarm sound, simply replace the `alarm.wav` file with another audio file, ensuring the file is in the correct format.

