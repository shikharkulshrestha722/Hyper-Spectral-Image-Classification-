# Hyper-Spectral-Image-Classification-
# Hyperspectral Image Classification with Self-Attention

## Overview
This project implements a deep learning model for hyperspectral image classification using a CNN combined with self-attention. The model learns both spectral and spatial features to classify each pixel in a hyperspectral image.

## Dataset
- Indian Pines dataset (preprocessed as NumPy arrays)
- Shape: (145 × 145 × 220 bands)

## Methodology
- Applied PCA to reduce spectral dimensions (220 → 30)
- Extracted spatial patches (15×15) around each pixel
- Built a CNN + Self-Attention model
- Trained using CrossEntropy loss

## Results
- High classification accuracy (~99%*)
- Visual comparison of ground truth vs predictions

*Note: Accuracy may be inflated due to patch-based splitting.

## Tech Stack
- Python
- PyTorch
- NumPy
- Scikit-learn
- Matplotlib

## How to Run
1. Clone the repository
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
