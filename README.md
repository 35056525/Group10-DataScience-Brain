# Group10-DataScience-Brain

# Title :
# EXPLAINABLE DEEP LEARNING FOR BRAIN TUMOUR CLASSIFICATION IN MRI IMAGES USING GRAD-CAM

# Project Overview

This project presents an explainable deep learning system for classifying brain tumors from MRI images. The model uses transfer learning with InceptionV3 to classify MRI scans into four categories:

Glioma
Meningioma
Pituitary Tumor
No Tumor

Grad-CAM is used to generate visual explanations, highlighting important regions in MRI images to improve interpretability and trust in predictions.

# Team Details

Group 10 Members:

Balu Krishna Gade
Role: Project Lead and GitHub Coordinator
Student ID: 35056225
Molla Ganja Shaida
Role: Data Engineer
Student ID: 35054237
Vijayagayathri Guntupalli
Role: Model Developer and Evaluation Lead
Student ID: 35054417
Venkata Naga Suresh Kumar
Role: XAI and Presentation Lead
Student ID: 35054355
Mounika Chinta
Role: Documentation Lead
Student ID: 35054164
Dataset

# Dataset used: Brain Tumor MRI Dataset
Link: https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset

# Description:

Total images: 8000
Classes: 4
Balanced using augmentation techniques
Pre-trained Model

The trained model file is large and not included directly in this repository.

Model size: More than 150 MB

Download the trained model from:
# https://drive.google.com/file/d/11t5VMiyZ9LGvHrHrp4q_nHgR8T4WyWlx/view?usp=drive_link

After downloading, place the model file in the following directory:

project_root/
models/
InceptionV3_Brain_Tumor_MRI.h5

# Project Structure

The project includes:

Training code (Jupyter Notebook)
Demo script for prediction
Trained model (external download)
Documentation and reports

Main files:

Full training notebook

Demo code for running predictions

# Environment Setup

Step 1: Clone the repository
git clone https://github.com/35056525/Group10-DataScience-Brain

cd Group10-DataScience-Brain

Step 2: Install required dependencies

# Create a requirements.txt file with the following:

tensorflow
numpy
matplotlib
pandas
scikit-learn
opencv-python
Pillow
tqdm
seaborn
scikit-image
kagglehub

Install using:
pip install -r requirements.txt

How to Run the Project
1. Training the Model

Open and run the notebook:

Brain_Tumor_Group10_Full_Code.ipynb

This will:

Load dataset
Perform preprocessing
Train the model
Evaluate performance
2. Running the Demo

Run the demo script:

python brain_tumor_demo_code.py

This will:

Load trained model
Predict tumor class
Display confidence scores
Show results for test images
Model Details
Base Model: InceptionV3 (pretrained on ImageNet)
Technique: Transfer Learning and Fine-tuning
Input Size: 224 x 224
Optimizer: Adam / AdamW
Loss Function: Categorical Crossentropy
Explainability

Grad-CAM is used to:

Highlight important regions in MRI images
Visualize model decision-making
Improve trust and interpretability
Performance Metrics

# Overall Performance:

Test Accuracy: 0.9737
Macro Precision: 0.9741
Macro Recall: 0.9738
Macro F1-score: 0.9738

# Class-wise Performance:

Glioma: F1-score ~ 0.96
Meningioma: F1-score ~ 0.96
No Tumor: F1-score ~ 0.98
Pituitary: F1-score ~ 0.99
Key Features
High accuracy model
Balanced dataset using augmentation
Explainable AI with Grad-CAM
Real-time prediction capability
Ethical Considerations
Model should assist clinicians, not replace them
Dataset bias may affect results
Requires validation before clinical use
# Conclusion

This project demonstrates an effective combination of deep learning and explainable AI for brain tumor classification. The use of Grad-CAM enhances transparency, making the system more reliable and suitable for real-world healthcare applications.
