# Alzhiemer-Disease-using-ResNet
Alzheimer’s Disease Prediction using Deep Learning (ResNet50)

Overview

This project focuses on the early diagnosis of Alzheimer’s Disease (AD) using Deep Learning, particularly ResNet50, a Convolutional Neural Network (CNN). The model classifies MRI scans into four categories: Demented, Non-Demented, Mild Demented, and Very Mild Demented. Early detection is critical for better disease management, and deep learning significantly enhances prediction accuracy compared to traditional diagnostic methods.

Dataset

The dataset is sourced from Kaggle, containing MRI images of patients categorized into:

Demented

Non-Demented

Mild Demented

Very Mild Demented

Data Statistics:

Training Images: 5120

Test Images: 1280

Image Resolution: 224x224 pixels (resized during preprocessing)

Methodology

Data Collection

Kaggle dataset of MRI scans.

Data pre-processing: resizing, normalization, and augmentation.

Deep Learning Model (ResNet50)

Pretrained ResNet50 model applied using Transfer Learning.

Layers fine-tuned to improve performance on AD classification.

Training & Optimization

Dataset split: Training (80%), Validation (10%), Testing (10%).

Loss function: Categorical Cross-Entropy.

Optimizer: Adam.

Batch Size: 32.

Evaluation Metrics

Accuracy: Ratio of correctly predicted samples.

Precision: TP / (TP + FP).

Recall: TP / (TP + FN).

F1 Score: Harmonic mean of precision and recall.

Model Performance

Achieved 80-90% accuracy on test data.

Avoided overfitting using dropout layers.

Performance visualized using accuracy/loss validation graphs.

Steps to Run:

Clone the Repository

git clone https://github.com/your-repo/alzheimer-prediction-resnet50.git cd alzheimer-prediction-resnet50

Install Dependencies

pip install -r requirements.txt

Run the Model

python train.py

Test the Model

python predict.py --image path/to/image.jpg

Results & Discussion

The ResNet50-based model demonstrates high accuracy in predicting Alzheimer’s at early stages. The use of Transfer Learning significantly improves classification performance, ensuring robust predictions. The study shows deep learning’s potential in revolutionizing AD diagnosis, reducing diagnosis time and human error.
