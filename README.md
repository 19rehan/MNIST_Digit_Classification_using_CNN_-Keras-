# 🔢 MNIST Digit Classification using CNN (Keras)


## 📝 Project Overview
The goal is to classify handwritten digits (0-9) from the MNIST Dataset. By implementing a **Convolutional Neural Network (CNN)**, the model learns to recognize spatial patterns, achieving an accuracy of **98.34%**.

---

## 🏗️ The Logic & Architecture

### 1. Preprocessing (Data Cleaning)
* **Normalization:** Scaled pixel values from `[0, 255]` to `[0, 1]` for faster convergence.
* **Reshaping:** Converted images to `(28, 28, 1)` to define the grayscale channel for CNN layers.
* **One-Hot Encoding:** Used `to_categorical` to transform labels into 10-class probability vectors.

### 2. Model Layers (The Blueprint)
* **Conv2D Layer:** The "Eyes" of the model; 32 filters to detect edges and curves.
* **MaxPooling2D:** Downsampling to keep only the most important features and reduce computation.
* **Flatten:** The bridge that converts 2D feature maps into a 1D vector for the Dense layers.
* **Dense (Hidden):** 64 neurons to understand complex relationships between extracted features.
* **Output Layer:** 10 neurons with **Softmax** activation to give the final probability (%) for each digit.

---

## 📊 Performance Summary
| Metric | Value | Logic |
| :--- | :--- | :--- |
| **Test Accuracy** | **98.34%** | Highly reliable for handwritten text. |
| **Loss Function** | `categorical_crossentropy` | Ideal for multi-class labeling. |
| **Optimizer** | `adam` | Adaptive learning rate for efficient training. |

---

## 🛠️ Tech Stack
* **Language:** Python
* **Library:** TensorFlow / Keras
* **Environment:** Google Colab / Jupyter Notebook
* **Visualization:** Matplotlib / NumPy
---

## 🚀 Future Goals
Moving forward, I will apply this logic to **CIFAR-10** (Color Images) to handle 3-channel (RGB) data and more complex object recognition.
