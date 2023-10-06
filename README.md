# driver_drowsiness_detection_system

This facial recognition and detection system can detect whether a driver is drowsy and feeling sleepy while driving a vehicle, or not. The objective of this python project is to build a drowsiness detection system that can detect that a person’s eyes are closed for a few seconds. This system will alert the driver when drowsiness is detected.

In this Python project, we've used OpenCV for gathering the images from webcam and feed them into a Deep Learning model which will classify whether the person’s eyes are ‘Open’ or ‘Closed’. The approach for making this project is as follows :

Step 1 – Take image as input from a camera.
Step 2 – Detect the face in the image and create a Region of Interest (ROI).
Step 3 – Detect the eyes from ROI and feed it to the classifier.
Step 4 – Classifier will categorize whether eyes are open or closed.
Step 5 – Calculate score to check whether the person is drowsy.

The model we used is built with Keras using Convolutional Neural Networks (CNN).
The CNN model architecture consists of the following layers:
Convolutional layer; 32 nodes, kernel size 3
Convolutional layer; 32 nodes, kernel size 3
Convolutional layer; 64 nodes, kernel size 3
Fully connected layer; 128 nodes
The final layer is also a fully connected layer with 2 nodes. A Relu activation function is used in all the layers except the output layer in which we used Softmax.

We've used:
OpenCV – pip install opencv-python (face and eye detection).
TensorFlow – pip install tensorflow (keras uses TensorFlow as backend).
Keras – pip install keras (to build our classification model).
Pygame – pip install pygame (to play alarm sound).
