# Facial Emotion Recognition with YOLOv11  

This project implements **Facial Emotion Recognition** using the **YOLOv11** object detection model, trained on a custom dataset hosted on **Roboflow**.  
It demonstrates **fine-tuning** and **transfer learning** approaches, then compares their training performance.  

---

## 😃 Recognized Emotions  
- 😠 Angry  
- 🙂 Happy  
- 😢 Sad  
- 😲 Surprised  

---

## 🚀 Features  
- 📥 One-line dataset download from **Roboflow**  
- 🔥 Train YOLOv11 with **fine-tuning** and **transfer learning**  
- 📊 Side-by-side comparison of training results  
- 🧩 Easy to adapt for other custom datasets  

---

## 📦 Setup  

Run this in **Google Colab** (recommended):  

```bash
!pip install roboflow ultralytics opencv-python matplotlib

from roboflow import Roboflow
rf = Roboflow(api_key="YOUR_API_KEY")
project = rf.workspace("youssef-elsheikh-pqoup").project("facial-emotion-recognition-hnujs")
version = project.version(1)
dataset = version.download("yolov11")

Facial-emotion-recognition-1/
│── train/
│── valid/
│── test/
│── data.yaml
