# Dog-Vision-Multi-class-Classifier
## 🐶 Dog Vision: Multi‑Class Image Classification
An end‑to‑end machine learning project for classifying dog breeds using deep learning and computer vision.


## 📌 Project Overview

This project builds a multi‑class image classifier capable of identifying dog breeds from images. It follows a complete ML workflow—from data ingestion and preprocessing to model training, evaluation, and deployment‑ready outputs.
The model leverages transfer learning with modern convolutional neural networks (CNNs) to achieve high accuracy even with limited training data.


## Dataset

* Kaggle Dog Breed Identification Dataset: https://www.kaggle.com/c/dog-breed-identification/overview
* Any custom dataset with labeled dog images
Each image should map to a breed label in a CSV or folder‑based structure.

## 🚀 Model Training Workflow

1. Load and preprocess data
* Resize images (e.g., 224×224)
* Normalize pixel values
* Turning data in batches

2. Build the model
* TensorFlow + Keras + ImageNetV2
* From TensorFlow Hub - "https://kaggle.com/models/google/mobilenet-v2/TensorFlow2/130-224-classification/1"

4. Train the model (TensorFlow)
* Using a 1000 images at first
* Use early stopping
* Save best weights
* Track accuracy/loss curves

4. Evaluate
* Overall accuracy
* Per‑class accuracy
* Confusion matrix
* Misclassified samples




## 🧠 Key Features
* Multi‑class classification (e.g., 120+ dog breeds)
* Transfer learning using pretrained CNNs (EfficientNet, ResNet, MobileNet)
* Data augmentation for improved generalization
* Training pipeline with checkpoints and early stopping
* Evaluation with accuracy, confusion matrix, and per‑class metrics
* Exportable model for inference (SavedModel / ONNX)


## 🛠️ Python Libraries Used
### Core ML & Deep Learning
* TensorFlow / Keras – model building, training
* PyTorch (optional alternative)
* scikit‑learn – metrics, preprocessing utilities


### Data Handling
* pandas – label and metadata management
* numpy – numerical operations


### Visualization
* matplotlib – training curves




## 📂 Project Structure

```
dog-vision/
│
├── data/
│   ├── train/
│   ├── test/
│   └── labels.csv
│
├── notebooks/
│   └── dog_vision_training.ipynb
│
├── src/
│   ├── data_loader.py
│   ├── model.py
│   ├── train.py
│   └── utils.py
│
├── requirements.txt
└── README.md
```

## Author
Created by Orangel Mendez email:omendez30@gmail.com
