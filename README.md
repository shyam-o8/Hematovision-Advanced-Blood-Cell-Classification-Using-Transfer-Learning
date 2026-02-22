# 🩸 HematoVision – Advanced Blood Cell Classification Using Transfer Learning

**AICTE Internship Project**  
**Team ID:** LTVIP2026TMIDS65951  
**Team Size:** 4  

---

## 👥 Team Details

**Team Leader:** Mekala Vishnu Vardhan  

**Team Members:**  
- Nizampatnam Shyam Prasad  
- Orsu Naga Yashaswini  
- Pulimi Jaswitha  

---

## 📌 Project Overview

HematoVision is a deep learning-based image classification system that classifies microscopic blood cell images into four categories:

- Eosinophil  
- Lymphocyte  
- Monocyte  
- Neutrophil  

The project uses Transfer Learning with the MobileNetV2 architecture to achieve high accuracy.  
It includes a model training pipeline and a Flask-based web application for real-time predictions.

---

## 🛠️ Technologies Used

- Python  
- TensorFlow / Keras  
- MobileNetV2 (Transfer Learning)  
- Flask  
- HTML / CSS  

---

## 📂 Dataset

This project uses the Blood Cell Images Dataset from Kaggle.

### Dataset Setup

1. Download the dataset from Kaggle.  
2. Extract the files.  
3. Create a folder named `dataset` inside the **Project files** directory.  
4. Organize the folders as shown below:

```
Project files/
│
├── dataset/
│   ├── TRAIN/
│   │   ├── EOSINOPHIL/
│   │   ├── LYMPHOCYTE/
│   │   ├── MONOCYTE/
│   │   └── NEUTROPHIL/
│   │
│   └── TEST/
│       ├── EOSINOPHIL/
│       ├── LYMPHOCYTE/
│       ├── MONOCYTE/
│       └── NEUTROPHIL/
│
├── app.py
├── web_app.py
├── requirements.txt
└── blood_cell_classifier_mobilenetv2.h5
```

---

## ⚙️ Installation

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/HematoVision-Advanced-Blood-Cell-Classification-Using-Transfer-Learning.git
cd HematoVision-Advanced-Blood-Cell-Classification-Using-Transfer-Learning
```

### 2️⃣ Install Dependencies

```bash
pip install -r "Project files/requirements.txt"
```

---

## 🚀 Usage

### 🔹 1. Train the Model

Run the following command to train the model:

```bash
cd "Project files"
python app.py
```

After training, the model file will be generated:

```
blood_cell_classifier_mobilenetv2.h5
```

---

### 🔹 2. Run the Web Application

Start the Flask server:

```bash
cd "Project files"
python web_app.py
```

Open your browser and go to:

```
http://127.0.0.1:5000
```

Upload a blood cell image to get the predicted result.

---

## 🧠 Model Details

- Base Model: MobileNetV2  
- Pretrained on ImageNet  
- Custom classification head  
- Softmax activation (4 output classes)  
- Fine-tuned for improved performance  

---

## 📊 Output Classes

The model classifies images into:

1. Eosinophil  
2. Lymphocyte  
3. Monocyte  
4. Neutrophil  

---

## 📜 License

This project was developed as part of the AICTE Internship Program for academic and educational purposes.
