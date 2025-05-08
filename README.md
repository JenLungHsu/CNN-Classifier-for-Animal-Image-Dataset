# CNN Classifier for Animal Image Dataset

[![Semester](https://img.shields.io/badge/Semester-Spring%202024-blue)]() [![Project](https://img.shields.io/badge/Project-Multimedia%20Content%20Analysis%20Project%203-orange)]()

🚀 check out the [report](./CNN%20classifier.pdf) for more detail.

---

## Overview
This project focuses on building a **Convolutional Neural Network (CNN)** to classify images of three different animals: **Dog**, **Cat**, and **Panda**. The implementation explores two different CNN architectures:
- **SimpleCNN**: A basic convolutional network with fewer layers.
- **DeeperCNN**: An extended version with more convolutional layers and a dropout layer to enhance generalization.

Data augmentation techniques were applied to improve model robustness, including:
- Random Cropping
- Horizontal and Vertical Flipping
- Perspective Transformations
- Rotation

---

## Dataset
- **Dataset:** [Kaggle - Animal Image Dataset (Dog, Cat, Panda)](https://www.kaggle.com/datasets/ashishsaxena2209/animal-image-datasetdog-cat-and-panda)
- **Description:** The dataset contains images of three animal species: Dog, Cat, and Panda, with balanced class distributions.

---

## Project Structure
```
├── CNN classifier.ipynb       # Jupyter Notebook with full model training and evaluation
├── CNN classifier.pdf         # Report of the analysis and findings
├── requirements.txt           # Dependencies for running the notebook
└── README.md                  # Project documentation
```

---

## Methodology
1. **Data Preparation:**
   - Loaded and preprocessed images from the dataset.
   - Split into **Training**, **Validation**, and **Test** sets.
   - Applied data augmentation for improved generalization.

2. **Model Architectures:**
   - **SimpleCNN**: Basic architecture with three convolutional layers.
   - **DeeperCNN**: Extended architecture with five convolutional layers and dropout regularization.

3. **Training Process:**
   - Loss function: Cross Entropy Loss
   - Optimizer: Adam with learning rate decay
   - Early stopping based on validation accuracy

4. **Evaluation:**
   - Accuracy and loss plots
   - Confusion matrix visualization
   - Class-wise performance metrics

---

## Results
The best performance was achieved with:
- **Model:** DeeperCNN
- **Test Accuracy:** 72.17%

<img src='image/Confusion Matrix.png' alt='Confusion Matrix' width='545'/>

The confusion matrix showed that misclassifications primarily occurred between **dog** and **cat** images, while **panda** was generally classified correctly due to its distinct features.

---

## Usage
To execute the notebook:
```bash
pip install -r requirements.txt
jupyter notebook 'CNN classifier.ipynb'
```

Before running the notebook, download the dataset from [Kaggle](https://www.kaggle.com/datasets/ashishsaxena2209/animal-image-datasetdog-cat-and-panda) and extract it into the project folder.

---

## Contact
- **Author:** Jen Lung Hsu
- **Email:** RE6121011@gs.ncku.edu.tw
- **Institute:** National Cheng Kung University, Institute of Data Science
