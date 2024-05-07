# Sign-Language-Detection-Using-LSTM
This project is an implementation of real-time gesture recognition using the MediaPipe library for landmark detection and LSTM (Long Short-Term Memory) neural networks for classification.

# Overview
Gesture recognition is an important area of computer vision and human-computer interaction. This project demonstrates how to build a gesture recognition system using deep learning techniques. The system captures video from a webcam, detects human body landmarks using MediaPipe, and classifies gestures using an LSTM neural network trained on the collected data.

## Features
- Real-time gesture recognition
- Customizable gesture definitions
- Support for multiple gestures
- Integration with MediaPipe for landmark detection

## Installation

1- Create a project directory named "gesture-recognition" and open VS Code

2- Clone the repository:

```bash
  git clone https://github.com/insh-samnani/Sign-Language-Detection-Using-LSTM.git
```

3- Navigate to the project directory:

```bash
  cd gesture-recognition
```

4- Install dependencies:

```bash
  pip install -r requirements.txt
```

5- Install TensorFlow:

```bash
  pip install tensorflow
```

6- Upgrade TensorFlow to the latest version:

```bash
  pip install --upgrade tensorflow
```

## Execution

1- Execute the python file by clicking on green button

2- Collecting the Dataset:
- Record live training data of hand gestures using a webcam or any other camera device.
- Capture various camera angles to enhance the model's robustness and generalization.
- Ensure diverse lighting conditions and backgrounds to make the model more adaptable to real-world scenarios.

3- Preprocessing the Dataset:
- Resize the frames to a consistent size to ensure uniformity across the dataset.
- Normalize the pixel intensities to a common scale (e.g., 0 to 1) to improve convergence during training.
- Split the dataset into training, validation, and testing sets. Typically, a common split ratio is 70% training, 15% validation, and 15% testing.

4- Creating Labels:
- Assign labels to the preprocessed data to represent different hand gestures. For example, labels can include "Quiet," "Hello," "Heart," etc.
- Ensure that the labels are consistent across the dataset and match the gestures recorded during data collection.

5- Building the LSTM Model:
- Define the architecture of the LSTM model. Typically, an LSTM model consists of one or more LSTM layers followed by one or more dense layers for classification.
- Prepare the input data to feed into the LSTM model. This may involve reshaping the data into sequences of fixed length.
- Compile the model with appropriate loss function and optimizer for training. For multi-class classification tasks like gesture recognition, categorical cross-entropy loss is commonly used along with Adam optimizer.
- Train the model on the preprocessed training data using the fit() method. Monitor the model's performance on the validation set to prevent overfitting.
- Evaluate the trained model on the testing set to assess its generalization performance.

## Contributors

- Insha Samnani (20K-0247)
- Ismail Ahmed Ansari (20K-0228)
- Yusra Adam (20K-0207)

## Acknowledgments

- Ms. Sumaiyah Zahid
- MediaPipe
- TensorFlow

## Troubleshooting
If you encounter any issues or have questions, please open an issue in the GitHub repository.
