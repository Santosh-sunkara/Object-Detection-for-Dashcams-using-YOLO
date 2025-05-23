# 📌 Object Detection for Dashcams Using YOLO 🚗💡

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1gqPvlw8nLLsS4xlrBxd6etvCll946joN?usp=sharing)

## 🔍 Overview
This project implements real-time object detection for dashcam footage using YOLO (You Only Look Once). It identifies and tracks objects such as cars, pedestrians, traffic signs, and other vehicles from BDD100K dataset images and videos.

---

## 📸 Sample Output
- ✅ Bounding boxes around detected objects  
- ✅ Object labels and classifications  
- ✅ Real-time inference on dashcam videos

---

## 📷 Example Detection on a Dashcam Image

![Detection Image 1](https://drive.google.com/uc?export=view&id=1vJT4O1XgBkWNSoVqueyx5ulYUm9-yufk)  
*Example 1*

![Detection Image 2](https://drive.google.com/uc?export=view&id=1pkhIg8Trj5SqEcydAAr-MMHK3eacvAnW)  
*Example 2*

---
## 🏅 Publication Certificate

[![Certificate](https://drive.google.com/thumbnail?id=18s9M4jGLMF3R4yCchVtRvWMiZ6NZdnUa)](https://drive.google.com/file/d/18s9M4jGLMF3R4yCchVtRvWMiZ6NZdnUa/view?usp=sharing)


## 📂 Project Structure
Object-Detection-for-Dashcams-using-YOLO/
│
├── models/                  # Pretrained YOLOv8 model weights (.pt files)
├── dataset/                 # BDD100K dataset (images and labels)
├── scripts/                 # Helper Python scripts for data preprocessing, visualization, etc.
│
├── detect.py                # Script to perform object detection on images/videos
├── train.py                 # Script to train YOLO model on BDD100K or custom dataset
├── Welcome_To_Colab.ipynb   # Jupyter Notebook for running project on Google Colab
│
├── requirements.txt         # Python dependencies list
├── README.md                # Project documentation file
└── utils.py                 # (Optional) Utility functions used in training or detection


---

## 🛠️ Features
- ✔️ Real-time object detection on images & videos  
- ✔️ Supports BDD100K dataset  
- ✔️ Bounding box visualization with OpenCV  
- ✔️ YOLO-based model for accurate detection  
- ✔️ Training support for custom datasets

---

## 📥 Installation & Setup

### 1️⃣ Clone the Repository

git clone https://github.com/Santosh-sunkara/Object-Detection-for-Dashcams-using-YOLO/blob/main/Source_Code
pip install -r requirements.txt


