# Improving-MNIST-Accuracy-with-Convolutional-Neural-Networks

# Instructions:
Tasks performed in the provided code:

1. **Data Loading**:
   - Load the MNIST dataset, specifically the training images and labels.

2. **Data Preprocessing**:
   - Reshape the images to add an extra dimension to represent the grayscale channel.
   - Normalize the pixel values of the images to the range [0, 1].

3. **Callback Definition**:
   - Define a custom callback class named `myCallback`.
   - Implement the `on_epoch_end` method to monitor the training accuracy at the end of each epoch.
   - If the training accuracy reaches 99.5% or higher, print a message indicating that training will be stopped.

4. **Model Architecture**:
   - Define the convolutional neural network (CNN) model using the `convolutional_model` function.
   - The model includes:
     - One convolutional layer with 32 filters, kernel size of (3, 3), ReLU activation, and input shape of (28, 28, 1).
     - One MaxPooling2D layer with pool size of (2, 2).
     - One Flatten layer to flatten the output of the convolutional layers.
     - One Dense layer with 128 units and ReLU activation.
     - One Dense output layer with 10 units and softmax activation for multi-class classification (MNIST has 10 classes).

5. **Model Compilation and Training**:
   - Compile the model using Adam optimizer and sparse categorical cross-entropy loss.
   - Train the model on the preprocessed training images and labels.
   - Use the custom callback to stop training when the accuracy reaches 99.5%.
   - Limit the training to a maximum of 10 epochs.

6. **Validation**:
   - Verify that the callback stops training once the desired accuracy is reached.

# Problem:
![Screenshot (30)](https://github.com/ArsalMirza007/Improving-MNIST-Accuracy-with-Convolutional-Neural-Networks/assets/121928372/4839e6c0-8f98-4879-8e72-304de8dc7d75)

# Solution:
![Screenshot (31)](https://github.com/ArsalMirza007/Improving-MNIST-Accuracy-with-Convolutional-Neural-Networks/assets/121928372/f04db71f-6325-41f9-9b18-fb082590dd9b)
