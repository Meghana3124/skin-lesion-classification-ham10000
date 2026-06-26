# Skin Cancer Detection using Deep Learning

## Project Overview

This project implements a deep learning pipeline for skin lesion classification using the HAM10000 dataset. A Convolutional Neural Network (CNN) is developed to classify dermoscopic images into seven different categories of skin lesions. The project also includes model comparison, data augmentation, explainability visualization, and error analysis.

---

## Dataset

Dataset: HAM10000 (Human Against Machine with 10000 Training Images)

The dataset contains dermoscopic images of seven skin lesion classes:

- akiec – Actinic Keratoses
- bcc – Basal Cell Carcinoma
- bkl – Benign Keratosis-like Lesions
- df – Dermatofibroma
- mel – Melanoma
- nv – Melanocytic Nevi
- vasc – Vascular Lesions

Dataset includes:

- Image files
- Metadata (HAM10000_metadata.csv)

---

## Project Objectives

- Build a CNN model for skin lesion classification.
- Compare CNN with MobileNetV2 and ResNet50.
- Apply image preprocessing and data augmentation.
- Visualize explainability using feature intensity heatmaps.
- Perform classification error analysis.

---

## Technologies Used

- Python
- TensorFlow / Keras
- Scikit-learn
- NumPy
- Pandas
- Matplotlib

---

## Project Structure

```
project/
│
├── code.py
├── HAM10000_metadata.csv
├── HAM10000_images_part_1/
├── HAM10000_images_part_2/
├── model_comparison_results.csv
└── README.md
```

---

## Workflow

### 1. Data Loading

- Load HAM10000 metadata
- Map image IDs to image paths
- Encode lesion labels

---

### 2. Data Preprocessing

- Train/Test split
- Validation split
- Image normalization
- Label encoding

---

### 3. Data Augmentation

Training images are augmented using:

- Rotation
- Zoom
- Horizontal Flip

This improves model generalization.

---

### 4. CNN Architecture

The CNN consists of:

- Conv2D (32 filters)
- MaxPooling
- Conv2D (64 filters)
- MaxPooling
- Conv2D (128 filters)
- MaxPooling
- Flatten
- Dense (256 neurons)
- Dropout (0.5)
- Softmax Output Layer

Optimizer:
- Adam

Loss Function:
- Categorical Crossentropy

Evaluation Metric:
- Accuracy

---

### 5. Model Training

- Image size: 128 × 128
- Batch size: 32
- Epochs: 5

---

### 6. Model Evaluation

Evaluation metrics include:

- Test Accuracy
- Test Loss
- Classification Report
- Confusion Matrix

---

### 7. Model Comparison

Models compared:

| Model | Accuracy | Loss |
|--------|----------|------|
| CNN | 70.53% | 0.7621 |
| MobileNetV2 | 66.93% | 1.1319 |
| ResNet50 | 66.93% | 1.0859 |

CNN achieved the highest accuracy.

---

### 8. Explainability

The project visualizes image feature intensity using a heatmap to highlight regions contributing to model predictions.

---

### 9. Error Analysis

Performance is analyzed using:

- Precision
- Recall
- F1-score
- Best-performing class
- Worst-performing class

---

## Results

CNN Performance

- Test Accuracy: ~70.53%
- Loss: ~0.7621

Observations:

- Excellent performance on the dominant NV class.
- Lower accuracy on minority classes due to dataset imbalance.

---

## Required Libraries

Install dependencies:

```bash
pip install tensorflow
pip install pandas
pip install numpy
pip install matplotlib
pip install scikit-learn
```

---

## Running the Project

```bash
python code.py
```

Ensure the HAM10000 dataset is available and update dataset paths if running outside Kaggle.

---

## Future Improvements

- Train for more epochs
- Apply transfer learning
- Address class imbalance
- Use Grad-CAM for explainability
- Hyperparameter optimization
- Deploy as a web application

---

## Author

Developed as a Deep Learning project for skin cancer image classification using the HAM10000 dataset.

---

## License

This project is intended for educational and research purposes only.
