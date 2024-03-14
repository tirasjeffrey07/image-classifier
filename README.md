## About

---

This is a deep learning model built using CNN.

An image classifier used to classify carrots and apples (a group that possesses a stark difference hence yielding highly accurate results).

This is also my first attempt on working with deep learning models.

Be kind :)

## Libraries and components used

---

1. tensorflow
2. os
3. cv2
4. imghdr
5. matplotlib
6. numpy
7. tensorflow.keras.models - Sequential
8. tensorflow.keras.layers - Conv2D
9. tensorflow.keras.layers - MaxPooling2D
10. tensorflow.keras.layers - Dense
11. tensorflow.keras.layers - Flatten

## Important!

---

Since the system I use couldnt run the notebook in a short span of time, Google Colab was used to run the notebook.

Change all the directories accordingly for proper functioning.

## Clarifications and other necessary information

---

- 70-20-10 rule is used here, 70% of the dataset for training, 20% for validation, 10% for testing

1. Convolution Layers

- The first Conv2D layer has 16 filters of size 3x3, with a ReLU activation function. It's the input layer, taking input images of size 256x256 with 3 channels (RGB)

- The second Conv2D layer has 32 filters of size 3x3 with ReLU activation

- The third Conv2D layer has 16 filters of size 3x3 with ReLU activation.

- Each convolutional layer is followed by a MaxPooling2D layer which reduces the spatial dimensions of the feature maps by taking the maximum value within a specified window (typically 2x2)

2. Flatten layer

- After the convolutional layers, a Flatten layer is added to convert the 3D feature maps into a 1D feature vector, which can be fed into a fully connected layer.

3. Dense Layers

- There is one Dense (fully connected) layer with 256 neurons and ReLU activation.

- The final output layer is also a Dense layer with a single neuron and a sigmoid activation function. This is common for binary classification tasks where the output should be between 0 and 1.

4. Compilation

- The model is compiled using the Adam optimizer and binary cross-entropy loss function, which is suitable for binary classification tasks.

- The metric being tracked during training is accuracy.
