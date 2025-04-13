# Pneumonia_detection
# 🫁 Pneumonia Detection from Chest X-Ray Images
Classify chest X-ray images into Pneumonia or Normal using Deep Learning and MobileNetV2.
## 📄 Overview
This project uses a deep learning model (MobileNetV2) to detect pneumonia in chest X-ray images. The goal is to assist in early diagnosis and reduce diagnostic errors.
## 📂 Dataset
- Dataset: [Chest X-ray Images (Pneumonia)](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)
- Classes: NORMAL, PNEUMONIA
- Total Images: ~5,000+
## 🧠 Model
- Base: MobileNetV2 (pretrained on ImageNet)
- Layers added:
  - GlobalAveragePooling2D
  - Dense(128, activation='relu')
  - Dropout(0.5)
  - Dense(1, activation='sigmoid')
## 📈 Results

| Dataset       | Accuracy |
|---------------|----------|
| Training      | 94.86%   |
| Validation    | 81.25%   |
| Test          | 88.00%   |
