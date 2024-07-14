# Digit_Recognizer_CNN_Model

## Project Description: Handwritten Digit Recognition using Convolutional Neural Networks

This project aims to develop a machine learning model capable of recognizing handwritten digits (0-9) from grayscale images. The model uses a Convolutional Neural Network (CNN) to achieve high accuracy in digit classification. The dataset consists of thousands of 28x28 pixel images, each labeled with the correct digit.

### Dataset

**Training Set:** Contains 1,716 images with 785 columns each. The first column is the label, and the remaining 784 columns represent pixel values.
**Test Set:** Contains 1,720 images with 784 columns, representing pixel values.
Preprocessing
**Data Loading:** Loaded training and test datasets from CSV files.
**Data Cleaning:** Removed rows with NaN values to ensure data integrity.
**Normalization:** Pixel values were normalized to a range of 0 to 1.
**Reshaping:** Images were reshaped from a 1D array of 784 values to a 3D array (28x28x1) to be suitable for the CNN input.
**One-Hot Encoding:** Labels were one-hot encoded for the multi-class classification problem.

### Model Architecture
The Convolutional Neural Network (CNN) architecture consists of:

**Convolutional Layer:** 32 filters, 3x3 kernel size, ReLU activation.
**Max Pooling Layer:** 2x2 pool size.
**Dropout Layer:** 25% dropout rate to prevent overfitting.
**Convolutional Layer:** 64 filters, 3x3 kernel size, ReLU activation.
**Max Pooling Layer:** 2x2 pool size.
**Dropout Layer:** 25% dropout rate.
**Flatten Layer:** Converts 2D matrix to 1D array.
**Fully Connected Layer:** 128 units, ReLU activation.
**Dropout Layer:** 50% dropout rate.
**Output Layer:** 10 units (one for each digit), softmax activation.

### Training
The model was trained using the Adam optimizer and categorical cross-entropy loss function. It achieved a validation accuracy of 94.75% after 10 epochs.

### Prediction and Submission
The trained model was used to predict the labels for the test dataset. Predictions were saved in a CSV file in the required submission format.

### Conclusion
This project successfully developed a CNN model that can accurately classify handwritten digits, achieving a high validation accuracy. The techniques and methods used can be applied to other image classification tasks, showcasing the power of deep learning in computer vision.

### Code
The full implementation of the project is included in the provided Python scripts, encompassing data preprocessing, model building, training, and prediction steps.
