# 🚁 Drone Detection System 

## 📝 Overview

This project detects drones in aerial images and videos using the YOLOv5 object detection model. It is designed to run seamlessly on **Google Colab** and supports detection on both **images and videos**, with visualized outputs.

---
## 🧰 Features

  YOLOv5 trained on custom drone data
  
  Real-time image/video detection
  
  Results visualized & saved in Colab
  
  Supports pretrained weights & fine-tuning
  
  FFmpeg used for video output
  
  Google Drive integration for storage

---
## 🚀 Setup in Google Colab

### 🔁 Clone the YOLOv5 repo

```bash
!git clone https://github.com/ultralytics/yolov5
%cd yolov5
!pip install -r requirements.txt

```

## 🧪 Train YOLOv5 on Drone Dataset
```
!python train.py --img 640 --batch 8 --epochs 30 --data drone_dataset.yaml --weights yolov5s.pt --cache

```

## 🖼️ Test Image Detection
```
!python detect.py --weights runs/train/exp/weights/best.pt --img 640 --conf 0.5 --source /content/drive/MyDrive/drone_test/sample.jpg

```

## 🎥 Test Video Detection
```
!python detect.py --weights runs/train/exp/weights/best.pt --img 640 --conf 0.5 --source /content/drive/MyDrive/drone_test/drone_video.mp4

```
## 📊 Results
Drone Detection Image Output Frame:

![Drone Detection Result](https://i.postimg.cc/sfQt8T45/Screenshot-596.png)

Drone Detection Video Output Frame:

▶️ [Click to watch drone detection video demo](https://streamable.com/qcerl9)

## 🔗 Repository

```
git clone https://github.com/AishwariyaRaj/Object_Detection_DroneSystem.git

```

## 📜 License

This project is open-sourced for educational and research purposes. Please ensure proper attribution when using the dataset and model outputs.



