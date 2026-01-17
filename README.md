# Fashion-MNIST-Classification
Deep learning project using TensorFlow/Keras on Fashion MNIST. Achieved ~82% accuracy with visualizations.


# Fashion MNIST Classification – Minor Project

# Overview
This project demonstrates a simple deep learning pipeline using **TensorFlow/Keras** on the **Fashion MNIST dataset**.  
It covers data loading, visualization, model building, training, evaluation, and prediction visualization.

# Dataset
- **Fashion MNIST**: 70,000 grayscale images (28×28 pixels) of 10 clothing categories:
  - T-shirt/top, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag, Ankle boot
- Split into:
  - 60,000 training images
  - 10,000 test images


# Project Workflow
1. **Data Loading**  
   - Imported Fashion MNIST via `keras.datasets.fashion_mnist`

2. **Data Visualization**  
   - Displayed sample images with labels using `matplotlib`

3. **Model Architecture**  
   - Sequential model:
     - Flatten layer (28×28 → 784)
     - Dense layer (128 neurons, ReLU activation)
     - Output Dense layer (10 neurons for 10 classes)

4. **Compilation & Training**  
   - Optimizer: Adam  
   - Loss: SparseCategoricalCrossentropy (from logits)  
   - Metric: Accuracy  
   - Trained for 10 epochs → **~83.5% training accuracy, ~81.7% test accuracy**

5. **Predictions & Evaluation**  
   - Added Softmax layer for probability outputs.  
   - Visualized predictions with probability plots.  
   - Correct predictions shown in **blue**, incorrect in **red**.


# Results
- Achieved ~82% accuracy on test data.
- Clear visualization of predictions and confidence scores.
- Demonstrates the basics of deep learning classification.


# Possible Improvements
- We Can Add **Convolutional Neural Networks (CNNs)** for higher accuracy (~90%+).
- and can Use **Dropout** or **Batch Normalization** for better generalization.
- and also we can Compare performance between dense-only and CNN models.
