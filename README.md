# 🚦 Traffic Signs Detection using YOLOv8

A computer vision portfolio project by **Ayesha Javaid** — custom training YOLOv8 on the German Traffic Sign Recognition dataset to detect and classify traffic signs in real time.

---

## 📌 Project Overview

This project demonstrates how to fine-tune a state-of-the-art object detection model (YOLOv8) on a custom dataset for autonomous driving use cases. Traffic sign detection is a core module in self-driving systems alongside lane detection and obstacle avoidance.

| Detail | Info |
|---|---|
| **Model** | YOLOv8s (Ultralytics) |
| **Dataset** | German Traffic Sign Recognition (Roboflow) |
| **Task** | Object Detection |
| **Framework** | PyTorch + Ultralytics |
| **Platform** | Google Colab (T4 GPU) |
| **Epochs** | 25 |
| **Image Size** | 640×640 |

---

## 🗂️ Repository Structure

```
traffic-signs-yolov8/
│
├── Ayesha_Javaid_Portfolio_Project_CV_DS8.ipynb   # Main Colab notebook
├── README.md                                       # Project documentation
├── requirements.txt                                # Python dependencies
├── .gitignore                                      # Files to exclude from git

```

---

## 🧠 Problem Statement

In autonomous vehicle systems, traffic sign detection is critical for safe navigation. This project focuses on:

- Downloading and preparing a real-world German traffic sign dataset
- Running baseline inference using a pretrained YOLOv8 model
- Fine-tuning (custom training) YOLOv8 on the traffic signs dataset
- Evaluating performance using mAP, Precision-Recall curves, Confusion Matrix, and F1 curves

---

## ⚙️ Setup & Usage

### 1. Open in Google Colab

Click the badge below to open the notebook directly in Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AyeshaJavaid676/Computer-Vision/blob/main/Ayesha_Javaid_Portfolio_Project_CV_DS8.ipynb)

> ⚠️ Make sure to set the **runtime to T4 GPU** before running: `Runtime → Change runtime type → T4 GPU`

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Dataset

The dataset is downloaded automatically via the Roboflow API inside the notebook:

- **Source:** [German Traffic Sign Recognition on Roboflow](https://universe.roboflow.com/trafficsignrecognition/german-traffic-sign-recognition)
- **Version:** 5
- **Format:** YOLOv8

---

## 🔄 Workflow

```
1. Install libraries (Ultralytics, Roboflow, OpenCV, etc.)
      ↓
2. Download German Traffic Sign dataset via Roboflow API
      ↓
3. Visualize sample training images (3×3 grid)
      ↓
4. Run inference with pretrained YOLOv8n (baseline)
      ↓
5. Fine-tune YOLOv8s on custom dataset (25 epochs, batch=16, imgsz=640)
      ↓
6. Evaluate with mAP, Precision-Recall, Confusion Matrix, F1 Curve
      ↓
7. Batch inference on 5 random test images
```

---

## 📊 Evaluation Metrics

After training, the model is evaluated using:

- **mAP (Mean Average Precision)** — overall detection accuracy
- **Precision-Recall Curve** — trade-off between precision and recall
- **Confusion Matrix** — per-class classification results
- **F1 Curve** — balance between precision and recall at various thresholds

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| [Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics) | Object detection model |
| [Roboflow](https://roboflow.com/) | Dataset management & download |
| [OpenCV](https://opencv.org/) | Image processing |
| [Matplotlib](https://matplotlib.org/) | Visualization |
| [PyTorch](https://pytorch.org/) | Deep learning backend |
| Google Colab | Cloud GPU training |

---

## 📚 Key Learnings

1. How to fine-tune a SOTA model (YOLOv8) for a custom task
2. Working with real-world annotated datasets from Roboflow
3. Using API keys to programmatically download datasets in Colab
4. Evaluating object detection models with industry-standard metrics

---

## 📎 References

- [YOLOv8 Documentation](https://docs.ultralytics.com/)
- [German Traffic Sign Dataset on Roboflow](https://universe.roboflow.com/search?q=german%2520traffic%2520sign)
---

## 👩‍💻 Author

**Ayesha Javaid**  
Computer Vision Portfolio Project | DS8  

---

## 📄 License

This project is for educational and portfolio purposes.
