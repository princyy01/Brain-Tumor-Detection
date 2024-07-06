This project utilizes deep learning techniques, specifically Convolutional Neural Networks (CNNs), to detect brain tumors from MRI images. 
The model is built using TensorFlow and Keras, and the web application is developed with Flask to allow users to upload MRI images and get predictions.

## Datasets
The dataset consists of MRI images labeled with:
no: MRI images without brain tumors
yes: MRI images with brain tumors

Each image is preprocessed by resizing to 64x64 pixels and normalized for model training.

## Model Architecture
The CNN model architecture consists of:

Three sets of Conv2D and MaxPooling2D layers to extract features from the images.
Flatten layer to convert 2D matrix data to a vector for Dense layer input.
Dense layers with ReLU activation for classification.
Dropout layer for regularization to prevent overfitting.
Output layer with Sigmoid activation for binary classification.

## Web Application
The Flask web application allows users to:

Upload an MRI image via a web interface.
Receive real-time predictions on whether the uploaded image contains a brain tumor.
Uploaded images are saved in the 'uploads' folder within the project directory.
