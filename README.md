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

![Example Detection](https://drive.google.com/uc?export=view&id=1KNcn3QI3m8X5XgLc8U9xaH6ZcA2MbXD8)

---

## 📂 Project Structure


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
```bash
git clone https://github.com/Santosh-sunkara/Object-Detection-for-Dashcams-using-YOLO.git
cd Object-Detection-for-Dashcams-using-YOLO

pip install -r requirements.txt
mkdir models
wget -O models/yolov8.pt https://github.com/ultralytics/yolov8/releases/download/v8.0.0/yolov8n.pt
python train.py --data bdd100k.yaml --weights yolov8n.pt --epochs 50
python detect.py --image data/sample.jpg --weights models/yolov8.pt
python detect.py --video data/dashcam.mp4 --weights models/yolov8.pt

for i in range(n_samples):
    img = cv2.imread(train_sample[i])
    img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)

    # Draw bounding boxes
    img = cv2.rectangle(img, pt1, pt2, color=(0,255,0), thickness=2)

    plt.imshow(img)
    plt.axis('off')
    plt.show()
