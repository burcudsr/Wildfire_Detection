# Real-Time Wildfire Detection Challenge

This project focuses on identifying wildfires using image classification techniques. It aims to classify images based on the presence of fire using Convolutional Neural Networks (CNN).

### 🚀 Live Demo
You can explore the live demo of the model here: https://huggingface.co/spaces/bdaser/Fire

### 📊 Dataset and Preprocessing
The dataset contains 699 images with and without fire. The processing steps include:
* Image loading and converting from BGR to RGB.
* Resizing images to 128x128.
* Normalization by dividing pixel values by 255.0.

### 🛠️ Model Architecture
The model is built using a Sequential structure containing Conv2D, BatchNormalization, LeakyReLU, MaxPooling2D, and Dropout layers.
* A Sigmoid activation function is used in the output layer.
* The model is compiled using the Adam optimizer and binary_crossentropy loss function.

### 📈 Training and Evaluation
EarlyStopping was utilized to prevent overfitting, with the best model weights restored from epoch 79.
* Accuracy 0.9817, Loss 0.1845, Val_accuracy 0.9643, Val_loss 0.2505.
* A test accuracy of 96.43% was achieved with a threshold of 0.5000.
* The evaluation resulted in 5 incorrect predictions, with an error rate of 3.57%.
