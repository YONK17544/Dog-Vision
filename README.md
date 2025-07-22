# Dog-Vision
A Dog Breed Classifier Project made using TensorFlow

# 🐶 Dog Breed Classifier using TensorFlow & MobileNetV2

This project is a deep learning-based dog breed classifier built using TensorFlow and Keras. It uses transfer learning with a pre-trained MobileNetV2 model to identify the breed of a dog from an image. The dataset used includes over 100 dog breeds.

---

## 📂 Folder Structure
dog-breed-classifier/
├── dog_breed_classifier.ipynb # Main Colab notebook
├── README.md # Project overview and instructions
├── requirements.txt # List of dependencies
└── /images/ # (Optional) Folder for prediction outputs


---

## 📊 Dataset

- **Source**: Custom dataset with labeled images of dog breeds  
- **Link**: [Download the dataset](https://www.dropbox.com/scl/fi/pjrulzwpa2osmtcl34j5c/dog-breed-identification.zip?rlkey=illavzwa19vysrolwpgqov86a&e=1&dl=0)  
- Format: `train`, `test`, and `labels.csv`  
- Organized into `ImageDataGenerator` pipelines

---

## ⚙️ Model Architecture

- Base Model: [`MobileNetV2`](https://tfhub.dev/google/imagenet/mobilenet_v2_130_224/feature_vector/4)
- Custom classification head: 1 Dense layer
- Loss: `SparseCategoricalCrossentropy`
- Optimizer: `Adam`
- Metrics: `accuracy`
- Callbacks: TensorBoard & EarlyStopping

---

---

## 📦 Dataset

- Source: [Dropbox Dog Breed Dataset](https://www.dropbox.com/scl/fi/pjrulzwpa2osmtcl34j5c/dog-breed-identification.zip?rlkey=illavzwa19vysrolwpgqov86a&e=1&dl=0)
- The dataset contains dog images and a CSV file with breed labels.

> ⚠️ Note: You need to manually download and extract the dataset before training. Place it in your working directory or mount it in Google Colab.

---

## 🚀 Features

- ✅ Transfer learning using `MobileNetV2` feature extractor
- ✅ 120 dog breeds classification
- ✅ Early stopping & TensorBoard logging
- ✅ Easily customizable for new datasets

---

## 🧠 Model Summary

- **Backbone:** `MobileNetV2` (`imagenet/mobilenet_v2_130_224/feature_vector/4`)
- **Trainable Params:** ~200K
- **Input Shape:** (224, 224, 3)

✅ Project Status
✅ Model built and trained
✅ Accurate top-5 predictions
✅ Validation performance verified

🧠 Reflections
This project was a major learning experience in:

Understanding image classification pipelines.

Building and debugging deep learning models.

Managing heavy cognitive load and persevering through complexity.

Even though I did not memorize all syntax, I focused on true comprehension — and that's what matters most.

📷 Sample Prediction
Input Image: Golden Retriever
Top-5 Predictions:
1. golden_retriever (confidence: 0.91)
2. labrador_retriever (0.05)
3. kuvasz (0.02)
4. flat-coated_retriever (0.01)
5. great_pyrenees (0.01)




