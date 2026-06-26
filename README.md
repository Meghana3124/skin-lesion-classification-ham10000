# Skin Lesion Classification Using Deep Learning Models on the HAM10000 Dataset

## 📌 Project Overview

Skin cancer is one of the most common types of cancer worldwide. Early diagnosis plays a crucial role in improving treatment outcomes and reducing mortality. This project develops and evaluates deep learning models for the automated classification of skin lesion images using the HAM10000 dataset.

Three deep learning models were implemented and compared:

- 🧠 Convolutional Neural Network (CNN)
- 📱 MobileNetV2
- 🔬 ResNet50

The project includes image preprocessing, data augmentation, model training, performance evaluation, explainability visualization, and error analysis.

---

## 🎯 Objectives

- Develop a CNN model for skin lesion classification.
- Compare CNN with MobileNetV2 and ResNet50.
- Improve model performance using image preprocessing and augmentation.
- Evaluate models using multiple performance metrics.
- Analyze classification results through explainability and error analysis.

---

## 📂 Dataset

**Dataset Name:** HAM10000 (Human Against Machine with 10000 Training Images)

**Source:** https://www.kaggle.com/datasets/kmader/skin-cancer-mnist-ham10000

The dataset contains **10,015 dermoscopic images** classified into seven categories:

| Class | Description |
|-------|-------------|
| akiec | Actinic Keratoses |
| bcc | Basal Cell Carcinoma |
| bkl | Benign Keratosis-like Lesions |
| df | Dermatofibroma |
| mel | Melanoma |
| nv | Melanocytic Nevi |
| vasc | Vascular Lesions |

---

## 🛠 Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Kaggle Notebook

---

## 📁 Project Structure

```
Skin-Lesion-Classification/
│
├── code.py
├── README.md
├── Report.pdf
├── model_comparison_results.csv
├── graphs/
│   ├── class_distribution.png
│   ├── cnn_accuracy.png
│   ├── cnn_loss.png
│   ├── confusion_matrix.png
│   ├── model_accuracy_comparison.png
│   ├── model_loss_comparison.png
│   ├── augmentation_examples.png
│   ├── explainability_heatmap.png
│   ├── precision_by_class.png
│   ├── recall_by_class.png
│   └── f1_score_by_class.png
│
├── dataset/
│   ├── HAM10000_metadata.csv
│   ├── HAM10000_images_part_1/
│   └── HAM10000_images_part_2/
│
└── outputs/
    └── model_comparison_results.csv
```

---

## 🔬 Methodology

### 1. Data Loading
- Load HAM10000 metadata.
- Map image IDs to image paths.

### 2. Data Preprocessing
- Image resizing (128 × 128)
- Label encoding
- Pixel normalization
- Dataset splitting (Training, Validation, Testing)

### 3. Data Augmentation
- Rotation
- Zoom
- Horizontal Flip

### 4. Model Development
- Custom CNN
- MobileNetV2
- ResNet50

### 5. Model Evaluation
- Accuracy
- Loss
- Precision
- Recall
- F1-score
- Confusion Matrix
- Classification Report

### 6. Explainability
- Feature intensity heatmap

### 7. Error Analysis
- Precision by class
- Recall by class
- F1-score by class

---

## ⚙ Experimental Setup

| Parameter | Value |
|-----------|-------|
| Image Size | 128 × 128 |
| Batch Size | 32 |
| Optimizer | Adam |
| Loss Function | Categorical Crossentropy |
| Activation Function | ReLU, Softmax |

### Dataset Split

| Dataset | Images |
|---------|-------:|
| Training | 7010 |
| Validation | 1502 |
| Testing | 1503 |

---

## 📊 Results

| Model | Accuracy | Loss |
|--------|----------|------|
| **CNN** | **70.53%** | **0.7621** |
| MobileNetV2 | 66.93% | 1.1319 |
| ResNet50 | 66.93% | 1.0859 |

### Key Findings

- The CNN model achieved the highest classification accuracy.
- Data augmentation improved model robustness.
- Explainability heatmaps provided insights into model predictions.
- Dataset imbalance affected the classification of minority classes.

---

## 📈 Outputs

The project generates the following outputs:

- Dataset Preview
- Class Distribution Graph
- CNN Accuracy Graph
- CNN Loss Graph
- Confusion Matrix
- Classification Report
- Model Accuracy Comparison
- Model Loss Comparison
- Data Augmentation Examples
- Explainability Heatmap
- Precision by Class
- Recall by Class
- F1-score by Class

---

## 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/your-username/Skin-Lesion-Classification.git
cd Skin-Lesion-Classification
```

Install dependencies:

```bash
pip install tensorflow pandas numpy matplotlib scikit-learn
```

---

## ▶️ Running the Project

1. Download the HAM10000 dataset from Kaggle.
2. Place the dataset in the `dataset/` folder.
3. Update dataset paths in the code if necessary.
4. Run the Python script:

```bash
python code.py
```

---

## 📌 Future Improvements

- Improve classification accuracy using EfficientNet or DenseNet.
- Address class imbalance with weighted loss or oversampling.
- Implement Grad-CAM for advanced explainability.
- Perform hyperparameter tuning.
- Deploy the model as a web application using Flask or Streamlit.

---

## 👩‍💻 Author

**Meghana Nagesh Poojari**

Master's Project – Deep Learning

June 2026

---

## 📚 References

1. Tschandl, P., Rosendahl, C., & Kittler, H. *The HAM10000 Dataset*.
2. TensorFlow Documentation – https://www.tensorflow.org
3. Keras Documentation – https://keras.io
4. Scikit-learn Documentation – https://scikit-learn.org
5. Kaggle HAM10000 Dataset – https://www.kaggle.com/datasets/kmader/skin-cancer-mnist-ham10000

---

## 📄 License

This project is developed for educational and research purposes only.
