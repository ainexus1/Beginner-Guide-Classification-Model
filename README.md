# Beginner Guide: Classification Model

This repository provides a beginner-friendly guide to building and training a binary classification model using TensorFlow and scikit-learn. The project uses a dataset of height and weight to classify gender and demonstrates preprocessing, model building, and visualization.

---

## Table of Contents
1. [Dataset](#)
2. [Requirements](#)
3. [Installation](#)
4. [Usage](#)
5. [Results](#)
6. [Acknowledgements](#)

---

## Dataset

The dataset used in this project is a collection of height and weight data categorized by gender. It is available on Kaggle:  
[Male-Female-Height-and-Weight](https://www.kaggle.com/datasets/saranpannasuriyaporn/male-female-height-and-weight).  

Download the dataset using the `kagglehub` library directly in the script or manually from the link above.

---

## Requirements

Make sure you have the following libraries installed:

- `numpy`
- `pandas`
- `matplotlib`
- `scikit-learn`
- `tensorflow`
- `kagglehub`

To install these libraries, run:
```bash
pip install numpy pandas matplotlib scikit-learn tensorflow kagglehub
```

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/ainexus1/Beginner-Guide-Classification-Model.git
   cd Beginner-Guide-Classification-Model
   ```

2. Ensure you have the required libraries installed. (See the [Requirements](#) section).

3. Run the script:
   ```bash
   python classification_model.py
   ```

---

## Usage

### 1. Dataset Preprocessing
- The dataset is downloaded using `kagglehub`.
- Categorical labels (Male/Female) are converted to numerical values (1/0).
- The data is split into training and testing sets using `train_test_split`.
- MinMaxScaler is applied for normalization.

### 2. Model Building
- A neural network is built using TensorFlow's `Sequential` API.
- The model consists of:
  - Dense layers with ReLU activation.
  - Batch normalization layers.
  - Dropout layers for regularization.
  - A sigmoid-activated output layer for binary classification.

### 3. Training
- The model is trained for 20 epochs with a batch size of 32.

### 4. Visualization
- Scatter plots visualize the dataset.
- Training history is plotted using `matplotlib`.

---

## Results

The model demonstrates how to classify binary data based on height and weight. Accuracy and loss metrics are logged, and training progress is visualized.

---

## Acknowledgements

- **Kaggle** for the dataset: [Male-Female-Height-and-Weight](https://www.kaggle.com/datasets/saranpannasuriyaporn/male-female-height-and-weight)
- TensorFlow and scikit-learn communities for documentation and tools.

---
