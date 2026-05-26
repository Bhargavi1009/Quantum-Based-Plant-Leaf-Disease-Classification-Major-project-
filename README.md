# 🌿 Quantum-Based Plant Leaf Disease Classification

## 📌 Abstract

This project presents a hybrid quantum-classical framework for plant leaf disease classification using image data. The approach combines classical preprocessing and feature extraction with quantum feature mapping circuits and a variational quantum classifier (VQC). The study explores the applicability of quantum machine learning techniques in solving real-world agricultural classification problems.

---

## 📖 Reference Paper

This work is implemented based on the methodology described in the following conference paper:

> *“Quantum Machine Learning for Image Classification using Variational Quantum Circuits”*
> (Conference Paper – adapted implementation)


---

## 🎯 Objectives

* To classify plant leaf images into healthy and diseased categories
* To implement quantum feature encoding using parameterized circuits
* To design and train a variational quantum classifier
* To evaluate classification performance using hybrid quantum models

---

## 📂 Dataset

Dataset used: **PlantDoc Dataset**

🔗 [https://www.kaggle.com/datasets/vipoooool/new-plant-diseases-dataset]

### Dataset Features:

* Multiple plant species (Tomato, Potato, Pepper, etc.)
* Healthy and diseased leaf images
* Multi-class classification problem

---

## ⚙️ Technologies Used

* Python
* Qiskit (Quantum Machine Learning)
* TensorFlow / Keras
* OpenCV
* NumPy, Matplotlib
* Scikit-learn

---

## 🧠 Methodology

### 🔹 1. Data Preprocessing

* Image resizing (64 × 64)
* Pixel normalization
* Data loading using ImageDataGenerator

---

### 🔹 2. Feature Extraction

* Conversion of images into numerical feature vectors
* Dimensionality reduction to match qubit constraints

---

### 🔹 3. Quantum Feature Mapping

* Implemented using **ZZFeatureMap**
* Encodes classical features into quantum states

---

### 🔹 4. Variational Quantum Classifier

* Implemented using **TwoLocal ansatz**
* Rotation gates: Ry
* Entanglement: CZ
* Optimizer: COBYLA

---

### 🔹 5. Model Training

* Hybrid classical–quantum pipeline
* Training performed on reduced feature set
* Limited by number of qubits

---

### 🔹 6. Model Evaluation

* Accuracy score used for evaluation
* Predictions compared against true labels
* Train-test split applied to avoid overfitting

---

## 🏗️ System Architecture

```text id="h8xmbg"
Input Image
     ↓
Image Preprocessing
     ↓
Feature Extraction
     ↓
Quantum Feature Mapping (ZZFeatureMap)
     ↓
Variational Quantum Circuit (TwoLocal)
     ↓
Measurement
     ↓
Predicted Class Label
```

---

## 📊 Results

* Achieved moderate classification accuracy
* Observed higher accuracy when evaluated on training data (overfitting)
* Improved evaluation using train-test split

---

## ⚠️ Limitations

* Limited number of qubits restricts feature size
* Training performed on small data samples
* Quantum simulation increases computational cost

---

## 🚀 Future Work

* Integrate CNN-based feature extraction
* Increase number of qubits for higher dimensional data
* Train on full dataset instead of batches
* Deploy model as a web-based application

---

## 📜 Conclusion

This project demonstrates the feasibility of applying quantum machine learning to plant leaf disease classification. Although constrained by current quantum hardware limitations, the hybrid approach shows promising potential for future research in agriculture and quantum computing.

---

## 📎 Notes

* Dataset is not included due to size limitations
* Download dataset from the provided Kaggle link
* Code implementation available in this repository

---
