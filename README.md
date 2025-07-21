CIFAR-10 Image Classification with a Convolutional Neural Network (CNN)
This project demonstrates the implementation and training of a Convolutional Neural Network (CNN) to classify images from the well-known CIFAR-10 dataset. The entire pipeline, from data loading and preprocessing to model training, evaluation, and visualization, is included in the Project_Python.ipynb notebook.

Description
The goal of this project is to build a robust image classifier for the 10 different classes in the CIFAR-10 dataset. The notebook leverages the TensorFlow and Keras libraries to construct, train, and evaluate the CNN model. Techniques like data augmentation, batch normalization, and dropout are employed to improve the model's performance and prevent overfitting.

Dataset
The project uses the CIFAR-10 dataset, which is a standard benchmark for image classification tasks. It consists of:

60,000 total 32x32 color images.

10 different classes, with 6,000 images per class.

A training set of 50,000 images and a test set of 10,000 images.

The 10 classes are:
airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck

Features
Data Preprocessing: Normalizes pixel values to a range of [0, 1] and converts labels to a one-hot encoded format.

Data Augmentation: Applies random horizontal flips, rotations, zooms, and contrast adjustments to the training data to create a more robust model.

CNN Architecture: Implements a sequential CNN model with multiple convolutional blocks, each containing Conv2D, BatchNormalization, MaxPooling2D, and Dropout layers.

Advanced Training: Uses Keras callbacks for efficient training:

EarlyStopping: Halts training if the validation loss does not improve, restoring the best model weights.

ReduceLROnPlateau: Reduces the learning rate when the validation loss plateaus.

ModelCheckpoint: Saves the best-performing model based on validation accuracy.

Comprehensive Evaluation: The model's performance is evaluated using:

Test accuracy and loss metrics.

A detailed classification report showing precision, recall, and F1-score for each class.

Rich Visualization: Includes functions to plot:

Training & Validation Accuracy/Loss curves.

A confusion matrix to analyze class-wise performance.

A sample of test images with their true and predicted labels.

Model Persistence: Saves the final trained model to a file (cifar10_cnn_model.h5) for future use.
