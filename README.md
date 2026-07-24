# Plant Disease Detection Using Deep Learning

[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange.svg)](https://tensorflow.org/)
[![Keras](https://img.shields.io/badge/Keras-Deep%20Learning-red.svg)](https://keras.io/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Project Overview
This project focuses on classifying plant diseases using computer vision and deep learning techniques. The goal is to rigorously analyze model performance, generalization capabilities, and architectural efficiency to determine the optimal approach for automated agricultural disease detection.

The notebook benchmarks and compares the following architectures:
*   **Baseline CNN:** A custom foundational convolutional neural network.
*   **Improved CNN Architecture:** Enhanced layers and regularization strategies.
*   **Augmented CNN:** Training integrated with custom data augmentation pipelines to combat overfitting.
*   **Transfer Learning (MobileNetV2):** Utilizing a lightweight pre-trained backbone optimized for efficiency.
*   **Transfer Learning (EfficientNetB0):** Leveraging a state-of-the-art scalable architecture for superior feature extraction.

---

## Dataset
*   **Source:** Imported directly via `kagglehub` from the [Plant Disease Detection Dataset](https://www.kaggle.com/datasets/karagwaanntreasure/plant-disease-detection)[cite: 1].
*   **Exploratory Data Analysis (EDA):** Included initial checks for class distributions, sample image inspections, dimension verification, and handling data imbalance[cite: 1].

---

## Key Steps & Workflow
1.  **Data Ingestion & Setup:** Automated dataset downloading via Kaggle API and directory configurations using TensorFlow/Keras[cite: 1].
2.  **Exploratory Data Analysis:** Visualizing sample inputs, checking image resolutions, and quantifying class imbalances[cite: 1].
3.  **Preprocessing & Augmentation:** Image resizing, normalization, and scaling, alongside augmentation layers.
4.  **Model Training & Evaluation:** Compiling models with appropriate loss functions, tracking accuracy/loss metrics, and generating detailed classification reports (`scikit-learn`)[cite: 1].

---

## Results & Comparison
*(1) Global Average Pooling is superior to flattening for image classification tasks, significantly reducing overfitting; 
(2) inverse-frequency
class weights effectively handle severe class imbalance (21:1 ratio) without requiring data
resampling; 
(3) the marginal performance gain of EfficientNetB0 (0.03%) over the Improved CNN may not justify its 100× larger model size for edge-device deployment.*

---

## Tech Stack
*   **Language:** Python[cite: 1]
*   **Deep Learning Framework:** TensorFlow / Keras[cite: 1]
*   **Data Analysis & Visualization:** NumPy, Pandas, Matplotlib, Seaborn[cite: 1]
*   **Metrics:** Scikit-learn (`classification_report`)[cite: 1]
*   **Environment:** Google Colab / Kaggle Notebooks[cite: 1]


