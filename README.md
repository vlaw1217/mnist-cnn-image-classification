# CNN MNIST Digit Recognition Lab

## Project Overview

This project builds a Convolutional Neural Network (CNN) to classify handwritten digits from the MNIST dataset.

The goal of this project is to practice deep learning image classification using TensorFlow/Keras and create an interviewer-friendly machine learning project that demonstrates the full model development workflow.

The model classifies grayscale handwritten digit images into one of ten classes:

`0, 1, 2, 3, 4, 5, 6, 7, 8, 9`

---

## Dataset

This project uses the MNIST dataset, which contains handwritten digit images.

The dataset includes:

- 60,000 training images
- 10,000 testing images
- Image size: 28 × 28 pixels
- Image type: grayscale
- Classes: digits 0 to 9

The dataset is loaded directly from TensorFlow/Keras:

```python
keras.datasets.mnist.load_data()
```

No manual dataset download is required.

---
## Project Workflow

The notebook follows these main steps:

1. Import required libraries
2. Load the MNIST dataset
3. Explore the image data and labels
4. Display sample handwritten digit images
5. Normalize pixel values from 0–255 to 0–1
6. Reshape images for CNN input
7. Build a CNN model
8. Compile the model
9. Train the model
10. Plot training and validation accuracy/loss
11. Evaluate the model on test data
12. Generate predictions
13. Review the classification report
14. Display the confusion matrix
15. Visualize sample model predictions
16. Review misclassified images
17. Summarize findings

---

## Tools and Libraries

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## Model Architecture

The CNN model includes the following layers:

| Layer | Purpose |
|---|---|
| Input | Defines the image shape as 28 × 28 × 1 |
| Conv2D | Extracts visual patterns such as edges, curves, and digit shapes |
| MaxPooling2D | Reduces feature map size while keeping important features |
| Conv2D | Learns deeper image patterns |
| MaxPooling2D | Further reduces feature size |
| Flatten | Converts 2D feature maps into a 1D vector |
| Dense | Learns classification patterns |
| Dropout | Reduces overfitting |
| Dense with Softmax | Outputs probabilities for digits 0 to 9 |

---

## Model Evaluation
The model was evaluated using:

- Test accuracy
- Test loss
- Classification report
- Confusion matrix
- Prediction visualization
- Misclassified image review

The CNN model achieved approximately **99% test accuracy** on the MNIST test dataset.

---

## Results Summary

The CNN model achieved approximately 99% test accuracy on the MNIST test dataset.

The classification report and confusion matrix showed strong performance across most digit classes. Most errors occurred when handwritten digits had similar or unclear shapes.

---

## What I Learned

Through this project, I practiced:

- Loading image data using TensorFlow/Keras
- Understanding grayscale image data
- Normalizing pixel values for neural network training
- Reshaping image data for CNN input
- Building a CNN model with convolutional and pooling layers
- Training and validating a deep learning model
- Evaluating model performance using classification metrics
- Interpreting confusion matrices
- Reviewing incorrect predictions for error analysis

---
