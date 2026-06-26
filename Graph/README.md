# Graph Outputs

## Overview

This folder contains all the graphical outputs generated during the implementation of the project **"Skin Lesion Classification Using Deep Learning Models on the HAM10000 Dataset."** These figures are used in the project report to illustrate data distribution, model performance, preprocessing techniques, explainability, and error analysis.

---

## Graph Descriptions

### 1. Class Distribution (`class_distribution.png`)
Displays the distribution of the seven skin lesion classes in the HAM10000 dataset. The graph highlights the dataset imbalance, with the **Melanocytic Nevi (nv)** class having the highest number of images.

---

### 2. CNN Training Accuracy (`cnn_accuracy.png`)
Shows the training and validation accuracy of the Convolutional Neural Network (CNN) over multiple training epochs. It illustrates how the model learns during training.

---

### 3. CNN Training Loss (`cnn_loss.png`)
Displays the training and validation loss of the CNN model across epochs. A decreasing loss indicates improved model learning and convergence.

---

### 4. Confusion Matrix (`confusion_matrix.png`)
Visualizes the classification performance of the CNN model by comparing actual and predicted labels for each skin lesion class. It helps identify correctly classified samples and common misclassifications.

---

### 5. Model Accuracy Comparison (`model_accuracy_comparison.png`)
Compares the classification accuracy of the three evaluated deep learning models:

- CNN
- MobileNetV2
- ResNet50

The CNN achieved the highest classification accuracy.

---

### 6. Model Loss Comparison (`model_loss_comparison.png`)
Compares the loss values of the three models. Lower loss indicates better prediction performance.

---

### 7. Data Augmentation Examples (`augmentation_examples.png`)
Illustrates augmented versions of a sample skin lesion image using preprocessing techniques such as:

- Rotation
- Zoom
- Horizontal Flip

These techniques improve model generalization and reduce overfitting.

---

### 8. Explainability Heatmap (`explainability_heatmap.png`)
Displays a heatmap highlighting image regions that contribute most to the model's prediction. This visualization improves the interpretability of the deep learning model.

---

### 9. Precision by Class (`precision_by_class.png`)
Shows the precision achieved for each skin lesion class, indicating the proportion of correct positive predictions.

---

### 10. Recall by Class (`recall_by_class.png`)
Illustrates the recall values for each class, measuring the model's ability to correctly identify positive samples.

---

### 11. F1-Score by Class (`f1_score_by_class.png`)
Presents the F1-score for each class, providing a balanced measure of precision and recall.

---

## Summary

These graphical outputs support the experimental analysis presented in the project report. They demonstrate dataset characteristics, training performance, model comparison, explainability, and error analysis. Together, they provide visual evidence of the effectiveness of the proposed deep learning approach for skin lesion classification.

---

## Generated Using

- Python
- TensorFlow / Keras
- Matplotlib
- Scikit-learn
- NumPy
- Pandas

---

**Project:** Skin Lesion Classification Using Deep Learning Models on the HAM10000 Dataset

**Author:** Meghana Nagesh Poojari

**Year:** 2026
