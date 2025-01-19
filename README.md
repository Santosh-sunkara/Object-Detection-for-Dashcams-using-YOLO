📌 Object Detection for Dashcams Using YOLO 🚗💡
🔍 Overview
This project implements real-time object detection for dashcam footage using YOLO (You Only Look Once). It identifies and tracks objects such as cars, pedestrians, traffic signs, and other vehicles from BDD100K dataset images and videos.

📸 Sample Output
✅ Bounding boxes around detected objects
✅ Object labels and classifications
✅ Real-time inference on dashcam videos

📷 Example Detection on a Dashcam Image


📂 Project Structure
bash
Copy
Edit
Object-Detection-for-Dashcams-using-YOLO/
│── models/              # YOLOv8 pretrained model files
│── dataset/             # Training and validation dataset (BDD100K)
│── scripts/             # Helper Python scripts for data processing
│── detect.py            # Main object detection script
│── train.py             # Model training script
│── Welcome_To_Colab.ipynb  # Jupyter Notebook (Colab version)
│── README.md            # Project Documentation
│── requirements.txt      # Dependencies list
🛠️ Features
✔️ Real-time object detection on images & videos
✔️ Supports BDD100K dataset
✔️ Bounding box visualization with OpenCV
✔️ YOLO-based model for accurate detection
✔️ Training support for custom datasets

📥 Installation & Setup
1️⃣ Clone the Repository
sh
Copy
Edit
git clone https://github.com/Santosh-sunkara/Object-Detection-for-Dashcams-using-YOLO.git
cd Object-Detection-for-Dashcams-using-YOLO
2️⃣ Install Dependencies
sh
Copy
Edit
pip install -r requirements.txt
3️⃣ Download the Model
Download the YOLOv8 pretrained model from Ultralytics and place it inside the models/ directory.

sh
Copy
Edit
mkdir models
wget -O models/yolov8.pt https://github.com/ultralytics/yolov8/releases/download/v8.0.0/yolov8n.pt
🚀 Training the Model
If you want to train your own model, modify train.py and run:

sh
Copy
Edit
python train.py --data bdd100k.yaml --weights yolov8n.pt --epochs 50
🔍 Running Object Detection
To detect objects in a sample image, run:

sh
Copy
Edit
python detect.py --image data/sample.jpg --weights models/yolov8.pt
For video detection (e.g., dashcam footage):

sh
Copy
Edit
python detect.py --video data/dashcam.mp4 --weights models/yolov8.pt
🎯 YOLO Detection Implementation
The Jupyter Notebook (.ipynb) contains the following workflow:

1️⃣ Load the BDD100K dataset
2️⃣ Define image height & width
3️⃣ Read images & annotations
4️⃣ Draw bounding boxes & labels
5️⃣ Display results using Matplotlib

Code Highlights:

python
Copy
Edit
for i in range(n_samples):
    img = cv2.imread(train_sample[i])
    img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
    
    # Draw bounding boxes
    img = cv2.rectangle(img, pt1, pt2, color=(0,255,0), thickness=2)
    
    plt.imshow(img)
    plt.axis('off')
    plt.show()
