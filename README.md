
🧠 PVSegmentationForParkinsonsDisease
Parkinson's Disease Detection Using Brain MRI Segmentation and Deep Learning

This project presents a deep learning-based framework for the automated detection of Parkinson's Disease (PD) from brain MRI scans. The approach combines medical image preprocessing, segmentation, and classification techniques to identify patterns associated with Parkinson's Disease and distinguish them from healthy subjects.

📌 Project Overview

Parkinson's Disease is a progressive neurological disorder that affects movement and cognitive functions. Early diagnosis is crucial for effective treatment and management.

This project leverages:

Brain MRI images
Segmentation masks
Deep Learning models
Medical image preprocessing techniques

to develop an automated Parkinson's Disease prediction system.

🎯 Objectives
Preprocess brain MRI scans for analysis.
Utilize segmentation masks to focus on relevant brain regions.
Extract meaningful features from MRI images.
Train a deep learning model for Parkinson's Disease classification.
Evaluate model performance using standard medical imaging metrics.
📂 Dataset

The dataset consists of:

Brain MRI images (.nii / .nii.gz)
Corresponding segmentation masks
Binary labels:
Parkinson's Disease (PD)
Healthy Control (HC)
Dataset Structure
dataset/
│
├── images/
│   ├── patient_001.nii.gz
│   ├── patient_002.nii.gz
│   └── ...
│
├── masks/
│   ├── patient_001_mask.nii.gz
│   ├── patient_002_mask.nii.gz
│   └── ...
│
└── labels.csv
🏗️ Project Architecture
MRI Images
     │
     ▼
Preprocessing
     │
     ▼
Mask Application
     │
     ▼
Data Augmentation
     │
     ▼
Deep Learning Model
     │
     ▼
Classification
(PD / Healthy)
⚙️ Methodology
1. Data Preprocessing
MRI volume loading using NiBabel
Intensity normalization
Slice extraction
Resizing
Mask alignment
2. Segmentation
Application of provided segmentation masks
Extraction of disease-relevant regions
3. Data Augmentation
Rotation
Horizontal flipping
Zooming
Brightness adjustments
4. Model Training

The model learns disease-specific features from segmented MRI scans.

Typical architecture components:

Convolutional Layers
Batch Normalization
ReLU Activation
Max Pooling
Dropout
Fully Connected Layers
🧪 Training Pipeline
Load Dataset
      ↓
Preprocess MRI Scans
      ↓
Apply Segmentation Masks
      ↓
Train Deep Learning Model
      ↓
Validate Performance
      ↓
Evaluate on Test Set
📊 Evaluation Metrics

The model is evaluated using:

Accuracy
Precision
Recall (Sensitivity)
Specificity
F1 Score
ROC-AUC Score
Confusion Matrix
Metric Definitions
Metric	Description
Accuracy	Overall prediction correctness
Precision	How many predicted PD cases are actually PD
Recall	How many actual PD cases were detected
Specificity	Ability to identify healthy subjects
F1 Score	Balance between precision and recall
ROC-AUC	Overall classification capability
🛠️ Technologies Used
Python
PyTorch / TensorFlow
NumPy
Pandas
OpenCV
NiBabel
Scikit-Learn
Matplotlib
Seaborn
📁 Repository Structure
PVSegmentationForParkinsonsDisease/
│
├── data/
├── notebooks/
├── models/
├── results/
├── images/
│
├── train.py
├── evaluate.py
├── predict.py
├── requirements.txt
├── README.md
│
└── utils/
🚀 Installation

Clone the repository:

git clone https://github.com/HIMANSHI549/PVSegmentationForParkinson.git

cd PVSegmentationForParkinson

Install dependencies:

pip install -r requirements.txt
▶️ Usage

Train the model:

python train.py

Evaluate the model:

python evaluate.py

Run prediction:

python predict.py
📈 Results

Example performance metrics:

Metric	Score
Accuracy	XX%
Precision	XX%
Recall	XX%
F1 Score	XX%
ROC-AUC	XX%

Replace these values with your actual experimental results.

🔬 Future Improvements
3D CNN architectures
Transformer-based medical imaging models
Multi-modal MRI analysis
Explainable AI (Grad-CAM)
Clinical deployment pipeline
👩‍💻 Author

Himanshi

B.Tech (Hons.) Artificial Intelligence & Data Science
Malaviya National Institute of Technology Jaipur
