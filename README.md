# 🚀 HHO-Based Fusion of YOLOv5 & YOLOv8 for Enhanced Locust Detection
🔍 A deep learning–based object detection model for locust identification using an HHO-optimized fusion of YOLOv5 and YOLOv8.

## 📌 Project Overview
This is the official repository for my research work:

"HHO-Based Fusion of YOLOv5 and YOLOv8 for Enhanced Locust Detection" (DOI: 10.5281/zenodo.14996737)

This study proposes a Harris Hawks Optimization (HHO)–based fusion framework that combines the strengths of YOLOv5 and YOLOv8 for accurate and efficient locust identification.
The dataset has been curated, annotated, and augmented specifically for this task.
This repository presents the implementation, fusion process, and performance evaluation of the proposed HHO-based fused YOLOv5–YOLOv8 model for real-world locust identification in smart farming applications. The study was conducted on:

1️⃣ A curated dataset specifically prepared for locust detection.

2️⃣ An augmented version of the dataset, where various augmentation techniques were applied to enhance model robustness.

3️⃣ Labels are in YOLO format.

## 🔥 Key Findings:
◆ The HHO-based fused model achieved a higher Mean IoU and better detection accuracy compared to individual YOLO models.

◆ The fusion reduced false positives and improved overall model robustness under varied lighting and environmental conditions.

◆ The fusion strategy effectively leveraged YOLOv5’s localization precision and YOLOv8’s generalization capability.

## ✅ Features
★ YOLOv5 + YOLOv8 fusion using Harris Hawks Optimization (HHO)

★ Curated and augmented dataset for locust detection

★ Training and inference scripts included

★ Fusion and evaluation scripts for HHO-based ensemble

★ Supports Google Colab for easy execution

## 📁 Dataset & Model Files
🔹 Code includes:

YOLOv5 and YOLOv8 base training scripts

HHO-based fusion implementation (fusion_hho.ipynb)

Inference and visualization utilities


🔹 Dataset is structured like this
```
locust_detection
├── images
│ ├── train
│ │ ├── img_001.jpg
│ │ ├── img_002.jpg
│ │ └── ...
│ ├── val
│ │ ├── img_101.jpg
│ │ ├── img_102.jpg
│ │ └── ...
└── labels
├── train
│ ├── img_001.txt
│ ├── img_002.txt
│ └── ...
├── val
│ ├── img_101.txt
│ ├── img_102.txt
│ └── ...
```
## 🎯 Augmentation Techniques Applied

The following augmentation techniques were applied to improve model diversity and robustness:

🔹 Horizontal & Vertical Flip

🔹 Brightness and Contrast Adjustment

🔹 Rotation and Scaling

🔹 Gaussian Blur

🔹 HSV Modification

🔹 Color Shifting

🔹 Cropping

💡 Augmentation script: augmentation.ipynb

### **Applied Augmentation Techniques**
![Augmentation](Results/augmentation.jpg)

## 🚀 Installation & Setup


1️⃣ Clone the Repository

git clone https://github.com/yourusername/locust-fusion-hho.git  
cd locust-fusion-hho


2️⃣ Install Dependencies

pip install -r requirements.txt

👉 If using Google Colab, run:

!pip install -r requirements.txt


3️⃣ Download the Dataset
Since the dataset is hosted on Zenodo, download it manually from:
🔗 Dataset DOI: 10.5281/zenodo.14964987

Unzip and place it in the correct directory (datasets/).

4️⃣ Mount Google Drive (if using Colab)
from google.colab import drive
drive.mount('/content/drive')



## 🔧 Training 

We trained and evaluated:

◆ YOLOv5 baseline

◆ YOLOv8 baseline

◆ Proposed HHO-based Fusion model

## ⚡ Training Commands

✔ Train YOLOv5

!python train.py --img 640 --batch 16 --epochs 60 --data dataset.yaml --weights yolov5s.pt

✔ Train YOLOv8

results = model.train(
    data='dataset.yaml',
    epochs=60,
    batch=16,
    imgsz=640
)

✔ Perform HHO-Based Fusion


🏆 Results & Evaluation

◆ The fused YOLOv5–YOLOv8 model achieved Mean IoU: 0.614 with the lowest False Detection Rate among all models.

◆ The HHO optimization balanced model outputs to enhance reliability across test samples.

Performance Comparison

| Model                       | Mean IoU  | Precision | Recall   | F1 Score |
| --------------------------- | --------- | --------- | -------- | -------- |
| YOLOv5                      | 0.589     | 0.82      | 0.78     | 0.80     |
| YOLOv8                      | 0.607     | 0.84      | 0.81     | 0.82     |
| **HHO-Fused YOLOv5+YOLOv8** | **0.614** | **0.86**  | **0.84** | **0.85** |




## ⚡ Results showed that YOLOv8 outperformed YOLOv5 in detection accuracy especially after augmentation.



## 📸 Visual Comparison of Results
Below are performance results:


📸 Sample Output

![Fused, Yolov8, Yolov5 Output](Results/detection.jpg)

📜 Citation

If you use this dataset or model, please cite the following:

🔗 Dataset DOI: 10.5281/zenodo.14964987

🔗 Fusion Model DOI: 10.5281/zenodo.14996737

## 📜 Citation

If you use this dataset, please cite the Zenodo DOI:  
🔗 DOI: [10.5281/zenodo.14964987](https://doi.org/10.5281/zenodo.14964987)  

```bibtex
@misc{vajpayee2025locust,
  author    = {Pooja Vajpayee and Kuldeep Kr. Yogi},
  title     = {Locust Images Dataset},
  year      = {2025},
  publisher = {Zenodo},
  doi       = {10.5281/zenodo.14964987},
  url       = {https://doi.org/10.5281/zenodo.14964987}
}
```



## 📄 License
🔹 This project is licensed under the MIT License.

## 🤝 Acknowledgments
Special thanks to Ultralytics for YOLO development.

## 📬 Contact

For questions, reach out via poojavjpy@gmail.com or https://www.researchgate.net/profile/Pooja-Vajpayee-2/research

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.14996738.svg)](https://doi.org/10.5281/zenodo.14996738)


