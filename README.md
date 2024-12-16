# Internship Task: Human Activity Recognition (HAR) using UCI Dataset
The [Human Activity Recognition (HAR) dataset](http://archive.ics.uci.edu/dataset/240/human+activity+recognition+using+smartphones) from the University of California, Irvine (UCI)
contains two types of data:
1. **Featurized data**: Pre-extracted features representing activities.
2. **Raw inertial sensor data**: Accelerometer and gyroscope readings from the sensors.

### Activity Labels
The experiments have been carried out with a group of 30 volunteers within an age bracket of 19-48 years. Each person performed six activities as follows

| labels | activity |
|---|------------|
| 1 | WALKING|
| 2 | WALKING_UPSTAIRS|
| 3 | WALKING_DOWNSTAIRS|
| 4 | SITTING|
| 5 | STANDING|
| 6 | LAYING|

<hr>

### Task 1: Demonstrate Bias-Variance Tradeoff

- Use the **featurized dataset** for this task.
- Train a **Decision Tree classifier**, varying the tree's depth to demonstrate the
**Bias-Variance** Tradeoff.
- Visualize and explain how performance changes with depth to highlight overfitting and
underfitting.

<hr>

### Task 2: Train and Compare Classic ML Models
- Use the **featurized dataset** to train the following models:
    - Random Forest classifier
    - Decision Tree classifier
    - Logistic Regression
    - AdaBoost classifier
- Evaluate these models using:
    - **K-Fold Cross-Validation (K-Fold CV)**
    - **Leave-One-Subject-Out Cross-Validation (LOSO-CV)**
- Compare the performance of the models using the following metrics:
    - Accuracy
    - Precision
    - Recall
    - F1 Score

<hr>

### Task 3: Dimensionality Reduction
- Identify **correlated features** in the **featurized dataset** and remove redundant features
to reduce dimensionality. Retrain the models from Task 2 on the reduced dataset and
report performance metrics again.
- Apply **Principal Component Analysis (PCA)** for dimensionality reduction. Retrain the
models using PCA-transformed features and compare the metrics with those from the
original and reduced datasets.

<hr>

### Task 4: Deep Learning on Raw Inertial Sensor Data
- Use the **raw inertial sensor data** to train the following deep learning models:
    - 1D Convolutional Neural Network (1D-CNN)
    - Multi-Layer Perceptron (MLP)
    - Long Short-Term Memory Network (LSTM)
- Evaluate the models using:
    - **K-Fold CV**
    - **Leave-One-Subject-Out CV**
- Report the performance of these models using:
    - Accuracy
    - Precision
    - Recall
    - F1 Score