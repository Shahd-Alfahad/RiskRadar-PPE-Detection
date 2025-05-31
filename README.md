
# RiskRadar – PPE Detection on Construction Sites 🦺👷‍♀️

RiskRadar is a machine learning-based system designed to **detect Personal Protective Equipment (PPE)** in real-time using image data from construction sites. The system supports safety enforcement by automatically identifying whether workers are wearing essential gear such as helmets, gloves, safety vests, and masks.

## 📌 Project Overview

Construction sites remain some of the most dangerous workplaces globally. RiskRadar leverages **computer vision and deep learning** to monitor PPE compliance and reduce safety risks. It was developed as part of a senior project at **King Saud University**.

> 🏗️ **Goal:** Improve site safety through automated visual detection of PPE.

## 🧠 Methods Used

### 1. Support Vector Machine (SVM)
- **Approach:** Feature extraction using HOG (Histogram of Oriented Gradients).
- **Purpose:** Baseline classification of safety gear presence.
- **Accuracy:** ~41% with linear kernel (best class F1-score: 59%).

### 2. YOLOv11 Object Detection
- **Approach:** Real-time detection of multiple PPE classes.
- **Baseline:** Trained on 10 epochs (Precision: 84.49%, Recall: 60.59%).
- **Tuned Model:** 100 epochs + batch size 64 (Precision: 92.13%, Recall: 74.12%).

> 📈 Metrics: Precision, Recall, mAP@50, mAP@50-95, Fitness Score

## 📊 Dataset

- Source: Roboflow (Construction Site Safety Dataset)  
- Format: YOLO annotation (.txt)  
- Size: 2,605 training images, 114 validation, 82 test  
- Classes: Helmet, No-Helmet, Mask, No-Mask, Gloves, Safety Vest, etc.


## 🛠️ Technologies

- Python, OpenCV, NumPy, scikit-learn, PyTorch, Ultralytics YOLO
- Jupyter Notebook, Roboflow, Matplotlib, Seaborn



> King Saud University — IT 461-ML Course, 1446H*
