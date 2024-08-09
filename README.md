# Image-Recognizer-Using-Machine-Learning

Data Loading and Preprocessing:
 
You’re using the CIFAR-10 dataset, which contains 60,000 32x32 color images in 10 different classes (e.g., airplanes, automobiles, birds, cats, etc.).
The dataset is split into training and test sets (X_train, y_train, X_test, y_test).
Images are normalized by dividing pixel values by 255.
Labels are one-hot encoded using to_categorical.

Model Architecture:

You’ve defined a simple neural network using Keras.
The model consists of a flattened input layer followed by a dense layer with 1000 units and ReLU activation.
The output layer has 10 units (one for each class) with softmax activation.

Model Compilation and Training:

The model is compiled with categorical cross-entropy loss and the Adam optimizer.
It’s trained on the training data for 10 epochs with a batch size of 64.
Validation data is provided during training.

Image Recognition Web App:

You’ve created a Streamlit web app for image recognition.
Users can upload an image, and the app will display the image and predict its class using the trained model.
The predicted probabilities for each class are shown in a horizontal bar chart.

Overall, this code demonstrates how to build a basic image recognition system using a pre-trained model on the CIFAR-10 dataset. The Streamlit app provides a user-friendly interface for testing the model with custom images. Great job! 😊
