# ISL_gesture_recog
Developed a Convolutional Neural Network (CNN) to classify Indian Sign Language gestures with over 98% accuracy. Collected and preprocessed data using OpenCV, trained the model with Keras, and implemented real-time gesture classification with TensorFlow. Explore this repository for the code, dataset details, and implementation insights.

## Use Case

The Indian Sign Language Gesture Recognition project aims to provide a robust solution for recognizing and classifying hand gestures in real time. This system can be utilized for various applications such as:

- **Accessibility Tools**: Helping individuals with hearing impairments communicate more effectively.
- **Educational Platforms**: Assisting in learning and teaching sign language.
- **Human-Computer Interaction**: Enabling intuitive and gesture-based control for applications and devices.

## Tech Stack

- **Python**: Primary programming language used for developing scripts and models.
- **OpenCV**: Used for capturing and processing video frames.
- **Mediapipe**: Provides tools for efficient hand gesture detection and landmark extraction.
- **TensorFlow**: Framework for training the Convolutional Neural Network (CNN) model.
- **Keras**: High-level API for building and training the CNN model.

## Files

1. **`collectdata.py`**
   - **Description**: Creates directories for storing gesture data. This script sets up the necessary folder structure to organize and store images for different hand gestures.
   - **Usage**: Run this script to initialize the directory structure before starting data collection.
   - **Example**:
     ```bash
     python collectdata.py
     ```

2. **`data.py`**
   - **Description**: Collects gesture data by capturing images from a camera. This script uses OpenCV to capture and save images of hand gestures for training the model.
   - **Usage**: Execute this script to collect and store images for each gesture category.
   - **Example**:
     ```bash
     python data.py
     ```

3. **`function.py`**
   - **Description**: Contains functions for efficiently collecting hand gesture data using Mediapipe. It includes utilities to process and enhance the captured gesture data.
   - **Usage**: This file is used by `data.py` to streamline data collection and improve accuracy.
   - **Example**: Directly imported and utilized in other scripts.

4. **`train.py`**
   - **Description**: Trains a machine learning model to recognize hand gestures. This script trains the model on the collected dataset and saves the trained model for later use.
   - **Usage**: Run this script after collecting gesture data to train the model and save it to a file.
   - **Example**:
     ```bash
     python train.py
     ```

5. **`app.py`**
   - **Description**: Uses the trained model to perform real-time hand gesture detection. This script captures video from the webcam, processes the frames, and predicts gestures using the saved model.
   - **Usage**: Run this script to start real-time gesture recognition using the trained model.
   - **Example**:
     ```bash
     python app.py
     ```

## Setup

1. **Install Dependencies**:
   Ensure you have all the required Python libraries installed. You can install them using pip:
   ```bash
   pip install opencv-python mediapipe tensorflow keras


This README provides a detailed overview of the project, including its use case, tech stack, file descriptions, setup instructions, and notes for users.
