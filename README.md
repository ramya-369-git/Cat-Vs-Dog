# 🐱🐶 Cat vs Dog Classification using CNN

This project implements a **Convolutional Neural Network (CNN)** to classify images as either **cats** or **dogs**. Using a dataset of labeled images, the model learns to distinguish features unique to each class and achieves strong accuracy with minimal preprocessing.

---

## 📌 Project Overview

Image classification is one of the most well-known applications of deep learning. In this project, we use a CNN built with **TensorFlow/Keras** to automatically learn visual patterns and classify images into one of two categories: **Cat** or **Dog**.

---

## 🧾 Dataset

- **Structure**:
  ```
  dataset/
  ├── cats/
  │   ├── cat001.jpg
  ├── dogs/
  │   ├── dog001.jpg
  ```
- **Source**: [Kaggle – Dogs vs Cats](https://www.kaggle.com/competitions/dogs-vs-cats/data)
- **Classes**:  
  - `0` = Cat  
  - `1` = Dog

> ⚠️ Note: The dataset is not included in this repo due to size limits. Download it from Kaggle and place it inside the `dataset/` folder.

---

## 🧠 Model Architecture (CNN)

Built using **Keras Sequential API**:

- Input Layer (resized RGB image: 150x150)
- 2–3 Convolutional layers with ReLU
- MaxPooling layers
- Dropout layer
- Dense (fully connected) layer
- Output layer with sigmoid activation (binary)

---

## 📊 Training Details

- **Loss**: Binary Crossentropy  
- **Optimizer**: Adam  
- **Metrics**: Accuracy  
- **Epochs**: 20  
- **Validation Split**: 20%

---

## 🖼️ Sample Predictions

| Image      | Prediction |
|------------|------------|
| `img1.jpeg`| Cat        |
| `img2.jpg` | Dog        |

---

## 📦 Dependencies

- Python 3.x  
- TensorFlow / Keras  
- NumPy  
- Matplotlib  
- OpenCV (optional for preprocessing)

Install using:
```bash
pip install -r requirements.txt
```

---

## 🚀 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/ramya-369-git/cat-vs-dog.git
   cd cat-vs-dog
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Add dataset to the `dataset/` folder

4. Run the notebook:
   ```bash
   jupyter notebook code.ipynb
   ```
