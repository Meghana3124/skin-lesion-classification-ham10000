# Skin Lesion Classification Using Deep Learning Models on the HAM10000 Dataset

## 📖 Project Overview

This project presents a deep learning-based approach for automated skin lesion classification using the **HAM10000 dataset**. The objective is to classify dermoscopic skin lesion images into seven diagnostic categories and compare the performance of three deep learning models:

- Convolutional Neural Network (CNN)
- MobileNetV2
- ResNet50

The project also includes image preprocessing, data augmentation, model evaluation, explainability visualization, and error analysis.

---

## 🎯 Objectives

- Develop a CNN model for skin lesion classification.
- Compare CNN with MobileNetV2 and ResNet50.
- Apply preprocessing and data augmentation techniques.
- Evaluate models using multiple performance metrics.
- Analyze model predictions using explainability and error analysis.

---

## 📂 Dataset

**Dataset:** HAM10000 (Human Against Machine with 10000 Training Images)

The dataset contains **10,015 dermoscopic images** belonging to seven skin lesion classes:

| Class | Description |
|-------|-------------|
| akiec | Actinic Keratoses |
| bcc | Basal Cell Carcinoma |
| bkl | Benign Keratosis-like Lesions |
| df | Dermatofibroma |
| mel | Melanoma |
| nv | Melanocytic Nevi |
| vasc | Vascular Lesions |

Dataset Link:
https://www.kaggle.com/datasets/kmader/skin-cancer-mnist-ham10000

---

## 🛠️ Technologies Used

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
├── Report.pdf
├── README.md
├── model_comparison_results.csv
│
├── HAM10000_metadata.csv
├── HAM10000_images_part_1/
└── HAM10000_images_part_2/
```

---

## ⚙️ Methodology

### Data Preprocessing

- Image resizing (128 × 128)
- Image normalization
- Label encoding
- Train/Validation/Test split

### Data Augmentation

- Rotation
- Zoom
- Horizontal Flip

### Deep Learning Models

- Custom CNN
- MobileNetV2
- ResNet50

---

## 🔬 Experimental Setup

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

- CNN achieved the highest classification accuracy.
- Data augmentation improved model robustness.
- Explainability heatmaps helped interpret predictions.
- Dataset imbalance affected minority class performance.

---

## 📈 Outputs

The project generates:

- Class Distribution Graph
- CNN Accuracy Graph
- CNN Loss Graph
- Confusion Matrix
- Classification Report
- Model Comparison Graphs
- Data Augmentation Examples
- Explainability Heatmap
- Error Analysis

---

## 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/your-username/Skin-Lesion-Classification.git
cd Skin-Lesion-Classification
```

Install the required packages:

```bash
pip install tensorflow pandas numpy matplotlib scikit-learn
```

---

## ▶️ Usage

Run the project using:

```bash
python code.py
```

Make sure the HAM10000 dataset is downloaded and the dataset paths are correctly configured before running the script.

---

## 📌 Future Improvements

- Improve performance using EfficientNet
- Address class imbalance
- Implement Grad-CAM for explainability
- Perform hyperparameter tuning
- Deploy the model as a web application

---

## 👩‍💻 Author

**Meghana Nagesh Poojari**

Master's Project – Deep Learning

June 2026

---

## 📚 References

- HAM10000 Dataset
- TensorFlow Documentation
- Keras Documentation
- Scikit-learn Documentation
- Kaggle HAM10000 Dataset

---

## 📄 License

This project is intended for educational and research purposes only.
