# Image Classification using CNN

## Abstract

This project implements a Convolutional Neural Network (CNN) for classifying images into accident and non-accident classes. The CNN model is built using TensorFlow and Keras.

## Dataset

The dataset consists of images collected from various sources, containing both accident and non-accident scenes. The images are preprocessed to ensure uniformity in dimensions and format. Any images not meeting the specified format are removed from the dataset during preprocessing.

## Preprocessing

During preprocessing, the following steps are performed:

1. **Image Format Checking**: Images are checked for their format using the `imghdr` module. Images not in the specified formats (e.g., JPEG, PNG) are removed from the dataset.

2. **Image Resizing**: Images are resized to a uniform size (e.g., 256x256) to ensure consistency in dimensions across the dataset.

## Model Architecture

The CNN model architecture consists of several convolutional layers followed by max-pooling layers for feature extraction. The final layers include fully connected (dense) layers for classification. The summary of the model architecture can be found in the script.

## Model Evaluation

The models are evaluated based on accuracy, confusion matrix, and classification reports. The performance of each model is analyzed to determine its effectiveness in sentiment classification.

## How to Run Locally

1. **Clone the repository:**

```bash
git clone https://github.com/raghulajithn/imageClassification.git
```
2. **Navigate to the project directory:**
```bash

cd imageClassification
```
3. **Install the required libraries:**
```bash
pip install tensorFlow opencv-python matplotlib numpy
```
> Ensure that your dataset is structured properly. It should have separate folders for each class (e.g., accident, non-accident), and each folder should contain the respective images.

> Update the data_dir variable in the script to point to your dataset directory.

4. **Run the Jupyter Notebook or Python script:**
```bash
python imageClassification.py
```

## Result
Upon training and evaluation, the model's performance metrics such as loss, accuracy, precision, and recall are displayed. Additionally, the model can be tested on new images to predict whether they depict accidents or not.
