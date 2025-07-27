# 🩺 Pneumonia Detection from Pediatric Chest X-Rays Using Deep Learning

This repository presents a deep learning approach to detect **pneumonia** from pediatric chest X-ray images using a pre-trained **EfficientNetV2L** model. The model is trained to classify X-ray images into **Normal**, **Bacterial Pneumonia**, and **Viral Pneumonia** categories.

---

## 📖 Project Overview

This work is inspired by **Figure S6** in the [Cell publication](http://www.cell.com/cell/fulltext/S0092-8674(18)30154-5), which illustrates:

- **Normal**: Clear lungs without abnormal opacification.
- **Bacterial Pneumonia**: Focal lobar consolidation (e.g., right upper lobe).
- **Viral Pneumonia**: Diffuse interstitial patterns across both lungs.

The model learns to identify these patterns from X-ray images using transfer learning techniques.

---

## 📁 Dataset

- **Source**: Guangzhou Women and Children’s Medical Center
- **Images**: 5,863 chest X-rays (AP view) of children aged 1–5 years
- **Classes**: `PNEUMONIA/` and `NORMAL/`
- **Split**: `train/`, `val/`, and `test/` folders

All radiographs underwent quality control and were labeled by two expert physicians, with evaluation samples reviewed by a third expert.

🔗 **Dataset Link**: [Chest X-Ray Images (Pneumonia) on Kaggle](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)

---

## 🔍 Features

- Image preprocessing and augmentation
- Deep learning classification using TensorFlow & Keras
- Evaluation via precision, recall, F1-score, confusion matrix
- Stratified K-Fold cross-validation
- Clean training loops with `tqdm` progress bars
- Visualization with Matplotlib and Seaborn

---

## 🧰 Libraries Used

- `TensorFlow`, `Keras`, `EfficientNetV2L`
- `OpenCV`, `NumPy`, `Pandas`
- `Matplotlib`, `Seaborn`, `TQDM`
- `Scikit-learn` (metrics & cross-validation)

---

## 📌 Citation

> Kermany, D.S. et al. (2018). *Identifying Medical Diagnoses and Treatable Diseases by Image-Based Deep Learning*. [Cell, 172(5), 1122–1131.e9](http://www.cell.com/cell/fulltext/S0092-8674(18)30154-5)

---

## 🚀 Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/dimpaldm/pneumonia-xray-detection.git
   cd pneumonia-xray-detection
