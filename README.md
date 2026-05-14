# RetailVision 🛒

End-to-end computer vision pipeline for retail product detection, OCR, and image similarity search.

Inspired by production CV systems built at scale — detecting products, reading labels, and matching items across hundreds of cameras in real time.

---

## 🎯 What This Project Does

- Detects retail products on shelves using YOLOv11
- Reads product labels using OCR (EasyOCR + CLAHE)
- Matches products to catalog using image similarity search
- Automatically retrains when model accuracy drops
- Serves predictions via REST API (FastAPI)
- Tracks all experiments with MLflow
- Monitors model health in real time

---

## 🏗️ Architecture
Input Image
↓

Preprocessing (CLAHE, resize, augmentation)
↓

YOLOv11 Detection (fine-tuned on retail data)
↓

OCR Module (EasyOCR)
↓

Embedding + Similarity Search (FAISS)
↓

FastAPI REST Endpoint
↓

MLflow Logging + Monitoring Dashboard

---

## 📁 Project Structure
retailvision/
│
├── data/
├── models/
├── ocr/
├── embeddings/
├── api/
├── monitoring/
├── experiments/
├── docker/
├── notebooks/
└── README.md

---

## 🛠️ Tech Stack

Python • PyTorch • YOLOv11 • EasyOCR • FAISS • FastAPI • MLflow • Docker • OpenCV

---

## 📊 Results

| Module | Metric | Result |
|--------|--------|--------|
| Detection | mAP | In progress |
| OCR | Accuracy | In progress |
| Similarity Search | Top-1 Accuracy | In progress |
| API | Inference Speed | In progress |

---

## 🚀 Roadmap

- [x] Project setup and structure
- [ ] Data preprocessing pipeline
- [ ] CNN classifier from scratch
- [ ] YOLOv11 fine-tuning
- [ ] OCR module
- [ ] Similarity search with FAISS
- [ ] FastAPI REST endpoint
- [ ] Auto-retraining pipeline
- [ ] Model monitoring dashboard
- [ ] Docker deployment
- [ ] Live demo on HuggingFace Spaces

---

## 👤 Author

Jaya Sravan Kala — Computer Vision Engineer  
[LinkedIn](https://www.linkedin.com/in/jaya-sravan-kala) • [Portfolio](https://jay1197-ui.github.io)
