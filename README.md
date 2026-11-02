<div align="center">

# 🩻 PNS Detection · YOLOv5

**Detect affected vs. normal regions in PNS X-ray images with a custom-trained YOLOv5s.**

<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"> <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" alt="PyTorch"> <img src="https://img.shields.io/badge/YOLO-111F68?style=for-the-badge" alt="YOLO"> <img src="https://img.shields.io/badge/Roboflow-6706CE?style=for-the-badge&logo=roboflow&logoColor=white" alt="Roboflow"> <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white" alt="Jupyter">

<a href="https://colab.research.google.com/github/KamranUmer/YoloV5_pns/blob/main/updated_1__YOLOv5_Tutorial.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab"></a>

</div>

<p align="center"><img src="https://github.com/KamranUmer/YoloV5_pns/assets/86089489/dd3c38a2-06c3-4b50-9773-75c76741754d" alt="PNS Detection · YOLOv5 screenshot" width="85%"></p>

## 📌 Overview

Trains YOLOv5s on a custom PNS dataset (from a Roboflow project) with two classes, **Effected** and **Normal**. Companion projects: a YOLO-NAS version in [yolo_nas](https://github.com/KamranUmer/yolo_nas) and a Streamlit app in [streamlitApp_for_Yolov5_pns](https://github.com/KamranUmer/streamlitApp_for_Yolov5_pns).

## 🔬 Pipeline

- Dataset pulled from Roboflow (`pns-detection`, version 4)
- YOLOv5s, 640 px images, batch 16, 100 epochs
- Results, confusion matrix and predictions saved to Google Drive

## 📊 Results

| Metric | Value |
|---|---|
| mAP@0.5 (all) | **0.914** |
| mAP@0.5:0.95 (all) | 0.401 |
| Precision / Recall | 0.895 / 0.891 |
| mAP@0.5 · Effected | 0.848 |
| mAP@0.5 · Normal | 0.980 |

> Validation set: 24 images, 48 labelled regions.

## 🚀 Getting Started

```bash
# Open the notebook in Google Colab (badge above), choose a GPU runtime,
# then run the cells from top to bottom.
# You need a Roboflow API key to download the dataset.
```

## ⚠️ Disclaimer

This project is for research and learning only. It is **not** a medical device and must not be used for diagnosis or treatment decisions.

## 🙏 Acknowledgements

- [YOLOv5](https://github.com/ultralytics/yolov5) by Ultralytics
- Dataset hosted on [Roboflow](https://roboflow.com)

---

<div align="center">

Built by <a href="https://github.com/KamranUmer"><b>Kamran Umer</b></a> · ⭐ Star the repo if you find it useful

</div>
