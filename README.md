# Malaria Classification using CNN

This project utilizes a Convolutional Neural Network (CNN) built with TensorFlow to classify cell images as either "parasitized" or "uninfected" using the Malaria dataset.

## Dataset Overview
- **Classes**: 2 (`parasitized`, `uninfected`)
- **Total Images**: 27,558

## Data Preprocessing
- **Train-Test Split**: 80% training, 20% testing
- **Image Preprocessing**: Resized to 200x200 pixels, normalized to `[0, 1]`.

## CNN Model Architecture
- **Layers**: 3 Conv2D, 3 MaxPooling, Flatten, Dense, Dropout
- **Activation**: ReLU for hidden layers, Softmax for output

## Model Training
- **Epochs**: 10
- **Batch Size**: 32
- **Callbacks**:
  - Early stopping with patience of 5 epochs
  - Learning rate reduction on plateau

## Model Performance
- **Accuracy**: Achieved 95.48% on the test set
