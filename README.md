# 😷 Face Mask Detection

## 📌 Dataset
- **Source:** Custom dataset with images and XML annotations.
- **Structure:** Images with bounding box annotations in XML format.

## 🔄 Preprocessing Steps
- Extracted images and annotations from a ZIP file.
- Parsed XML annotation files to retrieve bounding box details.
- Loaded and resized images for model training.

## 🏗️ Model Architecture
- Convolutional Neural Network (CNN) using Keras.
- Activation Functions: ReLU, Softmax.
- Optimizer: Adam.
- Loss Function: Categorical Crossentropy.

## 🎯 Training Process
- Used preprocessed images and annotations.
- Applied **data augmentation** for better generalization.
- Evaluated model performance using accuracy and loss metrics.

## 📊 Results
- Achieved **high accuracy** in detecting face masks.
- Works well in **varied lighting conditions** and **different angles**.

## 🚀 Future Enhancements
- Implement **real-time detection** using OpenCV.
- Improve **model accuracy** with more training data.
- Deploy as a **web or mobile application**.

## 🙌 Acknowledgments
- Dataset sourced from **publicly available datasets**.
- Inspired by **CNN-based object detection architectures**.
