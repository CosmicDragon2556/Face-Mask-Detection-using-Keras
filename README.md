# 😷 Real-Time Face Mask Detection  

A real-time face mask detection system that classifies three categories:  
- 😷 With Mask  
- 😶 Without Mask  
- ⚠️ Mask Worn Incorrectly  

Built with TensorFlow/Keras for model training and OpenCV for real-time inference.  


## 📌 Table of Contents  
- Features  
- Installation  
- Usage  
- Dataset  
- Model Architecture  
- Training  
- Results  
- Contributing  
- License  
- Contact  


## 🚀 Features  
- Real-time webcam/video stream detection  
- MobileNetV2-based CNN model  
- Handles class imbalance using data augmentation & class weights  
- Ready for Flask/Streamlit deployment(yet to do)
- Multi-class support (3 categories)  
- FPS optimization for real-time performance(yet to do)



## ⚙️ Installation  

### 🔧 Requirements  
- Python 3.8+  
- TensorFlow 2.x  
- OpenCV-Python  
- NumPy  
- Matplotlib  

### 🔹 Setup  
1. Clone the repository  
2. Navigate into the project folder  
3. Install dependencies using pip  


## ▶️ Usage  

### 📷 Real-Time Detection  
Run the detection script with the trained model (Yet to implement)

### 🖼️ Test Single Image  
Provide an image path to test mask classification.  

### 🎯 Training  
Train the model using the dataset and specify the number of epochs.  

## 📂 Dataset  

### 🔹 Structure  
- dataset_cnn/  
  - with_mask/ (3232 images)  
  - without_mask/ (717 images)  
  - mask_weared_incorrect/ (123 images)  

### 📊 Class Distribution  
| Class                   | Count |  
|-------------------------|-------|  
| 😷 With Mask           | 3232  |  
| 😶 Without Mask     | 717   |  
| ⚠️ Mask Worn Incorrect | 123   |  


## 🏗️ Model Architecture  

- Base Model: MobileNetV2 (pretrained on ImageNet)  
- Custom Head:  
  - GlobalAveragePooling2D  
  - Dense(256, activation='relu')  
  - Dropout(0.5)  
  - Dense(3, activation='softmax')  
- Optimizer: Adam (learning rate 0.0001)  
- Loss Function: Categorical Crossentropy  

## 📊 Training  

Model trained for 20 epochs:  
- Initial accuracy ~83%  
- Final validation accuracy ~93.2%  


## 🏆 Results  

- Accuracy: 93.2%  
- Inference Speed: 15 FPS (Tested on NVIDIA GTX 1660 Ti)  
- Model Size: 14 MB  


## 🤝 Contributing  

1. Fork the repository  
2. Create a feature branch  
3. Commit your changes  
4. Push to branch  
5. Open a Pull Request  

