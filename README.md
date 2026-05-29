[README(1).md](https://github.com/user-attachments/files/28385036/README.1.md)
# Dissertation Project – Deep Learning Image Classification

## Overview
This project was developed as part of the CMP600 Dissertation module for the BSc (Hons) Computing programme.

The dissertation focuses on using Deep Learning and Transfer Learning techniques for image classification. The project compares the performance of two popular convolutional neural network (CNN) architectures:

- MobileNetV2
- ResNet50

The system was designed and tested using TensorFlow and Keras in a Google Colab environment.

---

# Project Objectives

The main objectives of this project are:

- Build an image classification system using deep learning.
- Apply transfer learning using pre-trained CNN models.
- Compare the performance of MobileNetV2 and ResNet50.
- Evaluate classification accuracy using confusion matrices and classification reports.
- Investigate the effectiveness of data augmentation in improving model performance.

---

# Technologies Used

| Technology | Purpose |
|---|---|
| Python | Programming language |
| TensorFlow / Keras | Deep learning framework |
| NumPy | Numerical operations |
| Matplotlib | Data visualisation |
| Scikit-learn | Model evaluation |
| Seaborn | Confusion matrix visualisation |
| Google Colab | Development environment |

---

# Project Structure

```text
.
├── README.md
├── M420CQ.ipynb
├── m420cq.py
├── Dissertation-Proposal.pdf
├── Dissertation friday - Copy.pdf
└── CMP600-IT dissertation 1.pdf
```

---

# Dataset

The project uses an image classification dataset organised into training and testing folders.

Expected dataset structure:

```text
classification_task/
├── train/
│   ├── class_1/
│   ├── class_2/
│   ├── class_3/
│   └── class_4/
└── test/
    ├── class_1/
    ├── class_2/
    ├── class_3/
    └── class_4/
```

The dataset is loaded from a ZIP file and extracted automatically.

---

# Features

## Data Preprocessing

The project applies:

- Image resizing
- Rescaling
- Data augmentation
- Batch generation

Image augmentation includes:

- Rotation
- Zooming
- Horizontal flipping

---

# Models Implemented

## 1. MobileNetV2

MobileNetV2 is a lightweight convolutional neural network architecture optimised for performance and efficiency.

### Configuration

- Pre-trained on ImageNet
- Frozen convolutional base
- GlobalAveragePooling2D layer
- Dense layer with ReLU activation
- Dropout regularisation
- Softmax output layer

---

## 2. ResNet50

ResNet50 is a deeper residual neural network architecture designed to improve feature extraction and classification accuracy.

### Configuration

- Pre-trained on ImageNet
- Frozen convolutional base
- GlobalAveragePooling2D layer
- Dense layer with ReLU activation
- Dropout regularisation
- Softmax output layer

---

# Evaluation Metrics

The models are evaluated using:

- Accuracy
- Classification Report
- Confusion Matrix

The project compares the performance of both architectures to determine which model performs better for the selected dataset.

---

# Installation

## Requirements

Install the required Python packages:

```bash
pip install tensorflow numpy matplotlib scikit-learn seaborn
```

---

# Running the Project

## Option 1 – Google Colab

1. Upload the dataset ZIP file.
2. Open `M420CQ.ipynb` in Google Colab.
3. Update the dataset path if required.
4. Run all notebook cells.

---

## Option 2 – Local Machine

Run the Python script:

```bash
python m420cq.py
```

Ensure the dataset path is correctly configured before execution.

---

# Results

The project demonstrates how transfer learning can significantly improve image classification performance while reducing training time.

Both MobileNetV2 and ResNet50 achieved strong results, with ResNet50 generally providing better feature extraction at the cost of increased computational complexity.

---

# Future Improvements

Possible future enhancements include:

- Increasing dataset size
- Fine-tuning additional layers
- Testing other CNN architectures
- Hyperparameter optimisation
- Real-time image classification deployment
- Web or mobile application integration

---

# Academic Context

This project was created for the CMP600 Dissertation module as part of the BSc (Hons) Computing programme.

---

# Author

**Ionut-Denis Voroneanu**

BSc (Hons) Computing

2026
