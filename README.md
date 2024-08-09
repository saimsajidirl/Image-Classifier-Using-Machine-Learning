# Image-Recognizer-Using-Machine-Learning

Overview

This project demonstrates how to build an image recognition system using a pre-trained neural network model on the CIFAR-10 dataset. The system allows users to upload custom images and predicts their class based on the trained model.

Key Components

Data Loading and Preprocessing:

The CIFAR-10 dataset contains 60,000 32x32 color images across 10 classes (e.g., airplanes, automobiles, birds, cats, etc.).
Images are normalized by dividing pixel values by 255.
Labels are one-hot encoded using to_categorical.

Model Architecture:

A simple neural network is defined using Keras.
The model consists of:
A flattened input layer.
A dense layer with 1000 units and ReLU activation.
An output layer with 10 units (one for each class) and softmax activation.

Model Training:

The model is compiled with categorical cross-entropy loss and the Adam optimizer.
It’s trained on the training data for 10 epochs with a batch size of 64.
Validation data is used during training.

Streamlit Web App:

The Streamlit app provides a user-friendly interface for image recognition.
Users can upload an image.
The app displays the uploaded image and predicts its class using the trained model.
Predicted probabilities for each class are shown in a horizontal bar chart.
Usage
Clone this repository.
Install the required dependencies (tensorflow, numpy, matplotlib, streamlit, and PIL).
Run the Streamlit app using streamlit run app.py.
Upload an image to see the model’s predictions.


Acknowledgments

The CIFAR-10 dataset: CIFAR-10
Streamlit: Streamlit

Overall, this code demonstrates how to build a basic image recognition system using a pre-trained model on the CIFAR-10 dataset. The Streamlit app provides a user-friendly interface for testing the model with custom images. Great job! 😊
