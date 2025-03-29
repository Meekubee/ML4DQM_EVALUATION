# ML4DQM_EVALUATION

This repository contains my submission for the **Evaluation Test: ML4DQM**.

## Project Overview
The project involves building and evaluating a **Vision Transformer (ViT) model** to classify images from a synthetic dataset generated at the Large Hadron Collider's (LHC) Compact Muon Solenoid (CMS) detector. The goal is to classify input images into the dataset(2) they originate from using a ViT approach.

---

## Model Architecture
- **Base Model:** Vision Transformer (ViT)
- **Input Shape:** 224x224x3
- **Number of Classes:** 2 (Binary Classification)
- **Layers:**
    - Multi-Head Self-Attention
    - Feed-Forward Network with L2 Regularization
    - Dropout for Regularization
    - Layer Normalization
- **Loss Function:** Binary Cross-Entropy
- **Optimizer:** Adam with learning rate 0.0001
- **Metrics:** Accuracy, AUC, and ROC

---

## Data Preprocessing
- **Normalization:** Pixel values scaled between 0 and 1
- **Train/Validation/Test Split:** 70:15:15
- **Augmentation Techniques:**
    - Random Flip
    - Random Rotation
    - Random Zoom

---

## Performance Evaluation
- **Metrics Used:**
    - Classification Report (Precision, Recall, F1-score)
    - Confusion Matrix
    - ROC AUC Score
- **Results:**
    - Accuracy: ~99.3%
    - ROC AUC: ~0.9934

---


## How to Run
1. Clone the repository:
```bash
git clone https://github.com/Meekubee/ML4DQM_EVALUATION.git
```
2. Install Dependencies:
```bash
pip install -r requirements.txt
```
