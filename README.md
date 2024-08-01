# Edith--chatbot-with-emotional-intelligence

## Overview

This project demonstrates an advanced chatbot that uses real-time emotion detection through a camera to enhance interactions with humans. The chatbot observes and detects emotions and suggests tasks accordingly, leveraging state-of-the-art deep learning techniques and the MobileNet architecture for emotion recognition.

## Features

- **Real-Time Emotion Detection**: Utilizes the camera to detect user emotions in real-time.
- **Emotion-Aware Responses**: The chatbot tailors its responses and task suggestions based on detected emotions.
- **Deep Learning Model**: Employs MobileNet for accurate and efficient emotion recognition.

## Dataset

The dataset used for emotion recognition is downloaded from a Dropbox link and consists of labeled images for various emotions. The images are organized in a directory structure compatible with Keras's `ImageDataGenerator`.

## Model Architecture

The model architecture includes:

- MobileNet as the base model with pre-trained weights.
- A Flatten layer.
- A Dense layer with a softmax activation function for multi-class emotion classification.

## Training

The model is compiled using the Adam optimizer and categorical cross-entropy loss. It is trained with data augmentation techniques such as zoom, shear, and horizontal flip to enhance generalization.

## Evaluation

The model is evaluated using validation data, and the best model is saved based on validation accuracy. Early stopping and model checkpointing are utilized to prevent overfitting and save the best model, respectively.

## Usage

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/your-repository-name.git
    cd your-repository-name
    ```

2. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

3. Download and unzip the dataset using the provided Dropbox link:
    ```bash
    wget https://www.dropbox.com/s/w3zlhing4dkgeyb/train.zip?dl=0 -O train.zip
    unzip train.zip -d data
    ```

4. Run the Jupyter notebook to train and evaluate the model:
    ```bash
    jupyter notebook emotion_aware_chatbot.ipynb
    ```

5. Use the trained model for real-time emotion detection and chatbot interactions:
    - Ensure you have a camera connected.
    - Run the script for real-time emotion detection and chatbot interaction.

## Dependencies

- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- OpenCV (for real-time camera input)

## publication 

published this project in a journal https://www.ijitee.org/portfolio-item/c98120311422/
