# SkinSense

SkinSense is a deep learning-based skin disease detection system that classifies skin lesion images into 7 categories using a Convolutional Neural Network (CNN). Built as a multi-semester project, this is the Sem 1 deliverable: a trained classifier with a live demo interface.

## Problem Statement
Early detection of skin conditions — especially melanoma — significantly improves treatment outcomes. SkinSense aims to provide a fast, accessible first-look screening tool using image classification.

## Dataset
[HAM10000 (Human Against Machine)](https://www.kaggle.com/datasets/kmader/skin-cancer-mnist-ham10000) — 10,000+ dermatoscopic images across 7 skin lesion classes.

## Classes Detected
- Actinic keratoses (akiec)
- Basal cell carcinoma (bcc)
- Benign keratosis (bkl)
- Dermatofibroma (df)
- Melanoma (mel)
- Melanocytic nevi (nv)
- Vascular lesions (vasc)

## Tech Stack
- **Model:** CNN (TensorFlow/Keras)
- **Preprocessing:** NumPy, Pandas, scikit-learn
- **Demo Interface:** Gradio
- **Environment:** Google Colab (GPU-accelerated)

## Model Architecture
3 convolutional blocks (Conv2D + BatchNorm + MaxPooling) followed by dense layers with dropout, trained with class-weighted loss to handle dataset imbalance.

## How to Run
1. Clone this repo
2. Open `SkinSense.ipynb` in Google Colab
3. Run all cells (dataset auto-loads from provided CSVs)
4. Launch the Gradio demo cell to test with your own images

## Results
- Trained on 28x28 RGB images with class-weighted balancing
- Evaluated using precision, recall, and confusion matrix across all 7 classes

## Roadmap (Multi-Semester Plan)
- **Sem 1 (Current):** CNN classifier + Gradio demo ✅
- **Sem 2:** Severity scoring + treatment/precaution suggestions
- **Sem 3:** Doctor dashboard + patient history tracking
- **Sem 4:** Multi-condition detection (skin, nail, hair) + confidence-based doctor referral system

## Author
Ashwini Vindravath — B.Tech Data Science, Malla Reddy Engineering College for Women
