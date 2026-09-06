# 🪖 Helmet Detection & Traffic Violation Monitoring System

An AI-powered **Helmet Detection and Traffic Violation Monitoring System** built using Machine Learning, Deep Learning, Computer Vision, and a lightweight database system.

The system detects whether a two-wheeler rider is wearing a helmet and identifies helmet violations. It also maintains violation records and applies a warning and fine mechanism for repeated violations.

## 🚀 Project Overview

Road safety is an important concern, and not wearing a helmet is one of the most common traffic violations among two-wheeler riders.

This project uses Computer Vision and Deep Learning techniques to classify riders into:

* 🟢 With Helmet
* 🔴 Without Helmet

The system processes rider images, performs helmet classification, records violations, and provides an interactive interface for making predictions.

## ✨ Features

* 📊 Dataset analysis and preprocessing
* 🧹 Data quality and cleaning checks
* 🖼️ Image preprocessing and rider crop extraction
* 🔍 HOG feature extraction
* 🤖 Machine Learning using SGD Classifier
* 🧠 Deep Learning using MobileNetV3-Small
* 🔬 DINOv2 feature extraction
* ⚙️ Hyperparameter tuning
* 🔄 Data augmentation using AutoAugment
* ⚖️ Class balancing
* 📈 Model evaluation
* 📋 Classification reports
* 🔲 Confusion matrix visualization
* ⚠️ Helmet violation detection
* 🗃️ SQLite database for violation records
* 🚨 Warning and fine mechanism
* 🖥️ Interactive Gradio interface

## 🔄 System Workflow

```text
Dataset
   ↓
Data Download
   ↓
Data Analysis & Cleaning
   ↓
Annotation Processing
   ↓
Rider/Image Crop Extraction
   ↓
Data Augmentation
   ↓
Feature Extraction
   ↓
Model Training
   ↓
Model Evaluation
   ↓
Helmet Classification
   ↓
Violation Detection
   ↓
Warning & Fine Logic
   ↓
SQLite Database
   ↓
Gradio Interface
```

## 🤖 Models Used

### 1. HOG + SGD Classifier

A traditional Machine Learning approach using Histogram of Oriented Gradients (HOG) features followed by an SGD Classifier.

### 2. MobileNetV3-Small

A lightweight Deep Learning architecture used for efficient image classification.

### 3. DINOv2

DINOv2 is used as a vision foundation model for extracting powerful image representations, which are then used for helmet classification.

## 📊 Model Evaluation

The models are evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix
* Classification Report

These metrics help compare the performance of traditional Machine Learning and modern Deep Learning approaches.

## ⚠️ Violation Management

The system identifies a helmet violation when a rider is classified as **Without Helmet**.

Violation records are maintained using SQLite.

A repeated-violation mechanism is implemented where consecutive violations can result in:

```text
Helmet Violation
       ↓
Violation Recorded
       ↓
Repeated Violations
       ↓
Warning
       ↓
Fine
```

## 🖥️ User Interface

A Gradio-based interface is included to provide an easy way to interact with the trained system.

Users can upload an image and receive the helmet classification result along with the corresponding violation status.

## 🛠️ Technologies Used

* Python
* PyTorch
* Torchvision
* Scikit-learn
* OpenCV
* PIL
* NumPy
* Pandas
* Matplotlib
* Seaborn
* KaggleHub
* SQLite
* Gradio
* OpenPyXL

## 📂 Project Structure

```text
Helmet-Detection-System/
│
├── CONS1.ipynb
└── README.md
```

The complete implementation is contained in the Jupyter/Google Colab notebook.

## ▶️ How to Run

### Option 1: Google Colab

1. Open the `.ipynb` notebook in Google Colab.
2. Install the required dependencies if prompted.
3. Configure your Kaggle credentials if required.
4. Run the notebook cells sequentially.
5. Upload an image when prompted by the Gradio interface.
6. View the helmet classification and violation result.

### Option 2: Jupyter Notebook

1. Clone or download this repository.
2. Install the required Python packages.
3. Open `CONS1.ipynb` using Jupyter Notebook or JupyterLab.
4. Execute the cells sequentially.
5. Provide the required dataset and credentials.
6. Run the Gradio interface for prediction.

## 📌 Dataset

The project uses a helmet detection dataset obtained through KaggleHub.

The dataset contains annotated images that are processed to extract rider/object regions for helmet classification.

## 🎯 Learning Outcomes

This project provided hands-on experience with:

* Computer Vision
* Machine Learning
* Deep Learning
* Image preprocessing
* Feature extraction
* Transfer learning
* Vision foundation models
* Data augmentation
* Hyperparameter tuning
* Model evaluation
* Database integration
* Frontend integration using Gradio
* Building an end-to-end AI application

## 🔮 Future Improvements

Possible future enhancements include:

* Real-time helmet detection using CCTV/video streams
* YOLO-based object detection
* Automatic number plate recognition
* Rider identification
* Cloud database integration
* Web-based monitoring dashboard
* Automated violation reports
* Real-time traffic monitoring
* Deployment as a complete web application
* Integration with traffic management systems

## 👩‍💻 Author

**Alisha Verma**

Built as an end-to-end AI/Computer Vision project to explore practical applications of Machine Learning and Deep Learning in road safety.

---

⭐ If you find this project useful or interesting, feel free to star the repository!
