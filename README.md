# MNIST digit classification using CNNs

This repository contains a **Colab notebook** implementing multiple Convolutional Neural Network (CNN) architectures for the [Kaggle MNIST Digit Recognition](https://www.kaggle.com/c/digit-recognizer) competition. The goal is to experiment with different CNN architectures, compare performance, and achieve high accuracy on handwritten digit classification.

---

## Architectures

Implemented models:

- **MLP (Fully Connected Network)** – baseline model  
- **LeNet-5** – classic CNN architecture  
- **VGG-style CNN** – 3 convolutional blocks with increasing filters  
- **Deep CNN** – moderate-depth CNN with 2–4 convolutional blocks  
- **Mini-ResNet** – residual blocks with skip connections

---

## Key Features

- **Data preprocessing:** normalization and reshaping to `(28, 28, 1)`  
- **Data augmentation:** random rotations and contrast adjustments (applied only during training)  
- **Regularization:** Dropout and Batch Normalization  
- **Training techniques:** EarlyStopping to prevent overfitting
  
---

## Results

| Model           | Accuracy |
|-----------------|------------------|
| MLP             | ~95%             | 
| LeNet-5         | ~96%             | 
| Deep CNN        | ~97–98%          | 
| VGG-style CNN   | ~98%             | 
| Mini-ResNet     | ~98–99%          | 

- Mini-Resnet (kaggle) accuracy = 99.1% (Rank 318)
---

## Usage

1. Open the notebook in Google Colab:  

2. Run all cells sequentially to:

   - Load and preprocess MNIST dataset  
   - Train and evaluate different CNN architectures  
   - Generate predictions for Kaggle submission

3. Submit predictions to Kaggle.

---

## Dependencies

- TensorFlow 
- NumPy  
- Pandas  
- Matplotlib  

All dependencies are pre-installed in Google Colab.
