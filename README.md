# 🐶🐱 Dogs vs Cats Image Classification using Deep Learning

## 📌 Project Overview
This project focuses on building an efficient **image classification model** to distinguish between images of **dogs and cats** using Deep Learning techniques. The model leverages **Transfer Learning** with a pretrained architecture to achieve high accuracy with optimized training time.

The implementation is done using **TensorFlow and Keras**, and the model is trained on a labeled dataset of dog and cat images.

---

## 🎯 Project Objective
The primary goal of this project is to:

- Classify images into two categories: **Dog 🐶** or **Cat 🐱**
- Use **Transfer Learning** to improve performance and reduce training time
- Apply **Data Augmentation** to enhance model generalization
- Achieve high accuracy on validation data

---

## 📂 Dataset Details

### 📌 Source:
The dataset used in this project is publicly available on Kaggle:

🔗 https://www.kaggle.com/datasets/biaiscience/dogs-vs-cats/data


---

### 📊 Dataset Structure (Original):
The dataset initially contained all images in a single folder:

train/
cat.0.jpg
dog.1.jpg

---

### 🔧 Preprocessing Applied:
To make the dataset compatible with `flow_from_directory()`, the images were reorganized into class-wise folders:

data/train/
cat/
dog/

---

## ⚙️ Technologies Used

- **Programming Language:** Python 🐍  
- **Libraries & Frameworks:**
  - TensorFlow / Keras
  - NumPy
  - Matplotlib
  - OS & Shutil (for file handling)

---

## 🧠 Model Architecture

This project uses **Transfer Learning** with:

- **Base Model:** MobileNetV2 (pretrained on ImageNet)
- **Custom Layers Added:**
  - Global Average Pooling Layer
  - Dense Layer (128 neurons, ReLU activation)
  - Dropout Layer (0.5) to prevent overfitting
  - Output Layer (Sigmoid activation for binary classification)

---

## 🔄 Data Preprocessing & Augmentation

The following techniques were applied:

- Rescaling pixel values (0–255 → 0–1)
- Random rotation
- Zoom augmentation
- Horizontal flipping
- Validation split (20%)

These steps help improve model robustness and reduce overfitting.

---

## 🚀 Model Training

- **Batch Size:** 32  
- **Image Size:** 224 × 224  
- **Epochs:** 10  
- **Loss Function:** Binary Crossentropy  
- **Optimizer:** Adam  

The model was trained using training data and validated using a validation split.

---

## 📊 Model Performance

### ✅ Training Results:
157/157 ━━━━━━━━━━━━━━━━━━━━ 52s 332ms/step - accuracy: 0.9762 - loss: 0.0602


---

## 📈 Performance Analysis

- The model achieved **~97.7% validation accuracy**, indicating strong performance.
- High accuracy with low loss suggests effective learning.
- Data augmentation helped reduce overfitting.
- Transfer learning significantly improved training efficiency.

---

## 🔮 Prediction

The model takes an input image and predicts:

- **Dog 🐶** (if probability > 0.5)  
- **Cat 🐱** (if probability < 0.5)  

---

## 💡 Key Features of the Project

- Uses **Transfer Learning (MobileNetV2)**  
- Handles **real-world image variations** using augmentation  
- Efficient and fast training  
- High accuracy (~97%)  
- Clean and scalable pipeline  

---

## 🧪 Future Improvements

- Fine-tuning the pretrained model layers for even better accuracy  
- Adding more classes (multi-class classification)  
- Deploying the model using Flask or Streamlit  
- Integrating with a web or mobile application  

---

## 📌 Conclusion

This project demonstrates how deep learning and transfer learning can be effectively used for image classification tasks. By leveraging pretrained models and proper data preprocessing techniques, high accuracy can be achieved even with limited computational resources.

---
## 👩‍💻 Author

**Shreyasi Rawat**
