# AIDL_Project--A5
# 🧠 Brain Tumor Classification Using Deep Learning Models on MRI Images

## 📌 Project Overview

Brain Tumor Classification is an Artificial Intelligence and Deep Learning project that uses **MRI (Magnetic Resonance Imaging) images** to classify brain scans into four different categories.

This project uses Convolutional Neural Networks (CNN) and Transfer Learning techniques to identify brain tumor categories from MRI images.

Four deep learning models are implemented and compared:
- Simple CNN
- MobileNetV2
- EfficientNetB0
- ResNet50V2

The main objective is to evaluate different deep learning architectures and identify the model with the best classification accuracy.

## 🎯 Project Objectives

- Develop a deep learning model for brain MRI image classification.
- Preprocess and augment MRI images.
- Implement a baseline CNN model.
- Apply transfer learning using pretrained models.
- Evaluate model performance using test data.
- Compare the accuracy of different models.

## 📂 Dataset Information

**Dataset Name:** Brain Tumor MRI Dataset

**Dataset Source:** Kaggle

**Dataset Link:** https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset

**Dataset ID:** `masoudnickparvar/brain-tumor-mri-dataset`

The dataset contains four categories:

| Class | Description |
|---|---|
| Glioma | Glioma tumor category |
| Meningioma | Meningioma tumor category |
| No Tumor | MRI images without tumor |
| Pituitary | Pituitary tumor category |

### Dataset Distribution

| Dataset | Number of Images |
|---|---:|
| Training | 4,760 |
| Validation | 840 |
| Testing | 1,600 |
| **Total** | **7,200** |

## 🛠️ Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- KaggleHub
- Google Colab
- Streamlit

## ⚙️ Methodology

The project follows these steps:

1. **Dataset Collection:** Download the Brain Tumor MRI dataset using KaggleHub.
2. **Image Preprocessing:** Resize images to 224 × 224 pixels.
3. **Data Augmentation:** Apply rotation, width and height shifts, zoom, and horizontal flipping to training images.
4. **Model Building:** Implement CNN and pretrained deep learning architectures.
5. **Model Training:** Train models using the Adam optimizer and categorical cross-entropy loss.
6. **Fine-Tuning:** Fine-tune selected layers of pretrained models.
7. **Model Evaluation:** Evaluate performance using test accuracy, precision, recall, F1-score, and confusion matrices where reported.

## 🧠 Deep Learning Models

### 1. Simple CNN
A baseline Convolutional Neural Network with three convolutional blocks containing 32, 64, and 128 filters.

### 2. MobileNetV2
A pretrained lightweight CNN architecture using ImageNet weights and fine-tuning.

### 3. EfficientNetB0
A transfer-learning architecture that uses pretrained ImageNet weights and class-weighted training.

### 4. ResNet50V2
A pretrained residual neural network used for brain MRI image classification.

## 📊 Model Performance Comparison

The following table shows the test results recorded in the project notebook and report.

| Model | Test Accuracy |
|---|---:|
| Simple CNN | 67.44% |
| MobileNetV2 | 90.56% |
| EfficientNetB0 | 84.25% |
| ResNet50V2 | **94.63%** |

### 🏆 Best Performing Model

**ResNet50V2 achieved the highest test accuracy of 94.63%.**

The results indicate that transfer learning performed better than the baseline CNN in this experiment.

Note: The model pipelines use different preprocessing and validation settings, so the comparison is not a perfectly controlled experiment.

## 📈 Evaluation Techniques

The project uses the following evaluation methods:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Training and Validation Accuracy
- Training and Validation Loss

## 🚀 How to Run the Project

### Step 1: Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### Step 2: Open the Notebook

Open the Jupyter Notebook:

`Brain Tumor Classification from MRI Images using MobileNetV2.ipynb`

You can run it using Google Colab.

### Step 3: Install Required Libraries

```python
!pip install tensorflow kagglehub numpy matplotlib seaborn scikit-learn
```

### Step 4: Download the Dataset

```python
import kagglehub

DATA_ROOT = kagglehub.dataset_download(
    "masoudnickparvar/brain-tumor-mri-dataset"
)

print(DATA_ROOT)
```

### Step 5: Run the Notebook

Execute the notebook cells in order to:
- Load the dataset.
- Preprocess MRI images.
- Train the deep learning models.
- Evaluate model performance.
- Generate accuracy graphs and confusion matrices.

## 🌐 Project Demo

**Live Streamlit Application:**

https://brain-tumor-detection-nxlg2uxca2mb64ajmjfg4b.streamlit.app/

## 🔮 Future Enhancements

- Improve classification performance.
- Evaluate all models using identical data splits and preprocessing.
- Add complete class-wise evaluation metrics.
- Implement Grad-CAM for model explainability.
- Perform external dataset validation.
- Improve the web application interface.

## ⚠️ Disclaimer

This project is developed for academic and educational purposes only. It is an experimental image-classification system and should not be used as a replacement for professional medical diagnosis.

## 👨‍🎓 Project Details

**Project Title:** Brain Tumor Classification Using Deep Learning Models on MRI Images

**Student Name:** A. ASHISH

**Roll Number:** 2403A510A5

**Course:** Artificial Intelligence and Deep Learning (24CS312PC310)

**University:** SR University, Warangal, Telangana, India

**Academic Year:** 2026–2027

**Project Guide:** Anurodh Kumar

---

Brain-Tumor-Classification/
│
├── README.md
├── Brain Tumor Classification from MRI Images using MobileNetV2.ipynb
├── A5_Brain_Tumor_Project_Report.docx
├── Brain_Tumor_Classification_Project_Presentation.pptx
└── screenshots/
