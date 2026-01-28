### CIFAR-10 Image Classification with Keras CNN

This notebook demonstrates how to build and train a Convolutional Neural Network (CNN) using Keras for image classification on the CIFAR-10 dataset.

**Contents:**

1.  **Data Loading and Preprocessing:**
    *   Loads the CIFAR-10 dataset.
    *   Normalizes the pixel values of the images to the range [0, 1].

2.  **Model Architecture:**
    *   Defines a sequential CNN model with multiple convolutional layers (`Conv2D`), followed by batch normalization (`BatchNormalization`), max pooling (`MaxPooling2D`), and dropout layers (`Dropout`) to prevent overfitting.
    *   The convolutional blocks are followed by a `Flatten` layer and two `Dense` (fully connected) layers for classification.
    *   The model summary is printed, showing the layers, output shapes, and the number of parameters.

3.  **Model Compilation and Training:**
    *   The model is compiled using `sparse_categorical_crossentropy` as the loss function, the `adam` optimizer, and `accuracy` as the evaluation metric.
    *   The model is trained on the preprocessed training data for 20 epochs, with validation performed on the test data.

4.  **Performance Visualization:**
    *   Plots are generated to visualize the training and validation loss over epochs.
    *   Plots are generated to visualize the training and validation accuracy over epochs.

5.  **Prediction Example:**
    *   Makes predictions on a subset of the test data and displays the predicted labels alongside the true labels.
