# Malaria Diagnosis using Convolutional Neural Networks

## 📌 Project Overview

This project implements a **Convolutional Neural Network (CNN)** for automated malaria diagnosis using microscopic images of blood smears. Malaria is a life-threatening disease caused by *Plasmodium parasites*, and rapid, reliable diagnosis is critical for effective treatment.

Using **deep learning and transfer learning (VGG16, VGG19, ResNet50, InceptionV3)**, the model classifies cell images into two categories:

* **Infected Cells**
* **Uninfected Cells**

This project demonstrates how machine learning can aid healthcare professionals by providing an **automated, accurate, and scalable diagnostic tool**.

---

## 📂 Dataset

The dataset used is the **Malaria Cell Images Dataset** from the **National Institutes of Health (NIH)**.

* Images are divided into **Infected** and **Uninfected** categories.
* The dataset was split into **Training (80%)**, **Validation (10%)**, and **Testing (10%)** using the [`splitfolders`](https://pypi.org/project/split-folders/) library.

Example:

```
Malaria Cell Images/
│── Infected/
│── Uninfected/
```

---

## ⚙️ Features

* Preprocessing & Augmentation with **ImageDataGenerator**
* Balanced dataset using **class weights**
* Multiple CNN architectures tested:

  * VGG16
  * VGG19
  * ResNet50
  * InceptionV3
* Visualization of model architecture using **visualkeras**
* Performance evaluation on test data

---

## 🚀 Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/malaria-cnn-diagnosis.git
cd malaria-cnn-diagnosis
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Requirements

Main libraries used:

* `tensorflow` / `keras`
* `numpy`, `pandas`, `matplotlib`
* `opencv-python`
* `split-folders`
* `visualkeras`

---

## 🏗️ Model Architecture

The primary model used is **VGG19** with additional layers for classification.

* Convolutional + Pooling Layers (from VGG backbone)
* Flatten / Global Average Pooling
* Dense Layers with **Dropout**
* Softmax output layer (2 classes)

---

## 📊 Training

* **Optimizer:** Adam
* **Loss Function:** Binary Crossentropy
* **Evaluation Metrics:** Accuracy

Class imbalance was handled using **class weights**.

---

## 📈 Results & Evaluation

The trained CNN achieved high accuracy in distinguishing **infected vs uninfected** cells.

* Accuracy: \~95% (on validation & test sets)
* Loss & Accuracy plots were generated to track performance.

---

## 🔍 Visualizations

* Sample **Infected vs Uninfected** cell images
* Model architecture visualization using `visualkeras`
* Training/validation **accuracy & loss curves**

---

## 📜 How to Run

Run the Jupyter notebook:

```bash
jupyter notebook malaria-detector-checkpoint.ipynb
```

Or, for Google Colab:

1. Upload the notebook.
2. Mount dataset folder.
3. Run all cells.

---

## 📌 Future Work

* Deploy the model using **Flask/Django + Streamlit/Gradio**
* Integrate with **mobile diagnostic tools**
* Improve generalization with larger datasets

---

## 🤝 Contributing

Pull requests are welcome! If you’d like to improve this project (deployment, optimization, or documentation), feel free to fork and contribute.

---

## 📧 Contact

👩‍💻 **Akanksha Sawant**

* 📍 Pune, India
* 💼 [LinkedIn]([https://www.linkedin.com](https://www.linkedin.com/in/akanksha-sawant-29260226a/))
* 🖥️ [GitHub]([https://github.com/your-username](https://github.com/AkankshaASawant))
