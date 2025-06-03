# Lung-Cancer-Classification
A deep learning project to classify lung cancer subtypes using histopathology images from the LungHist700 dataset. Three models — ViT, ResNet50, and EfficientNet — were compared after applying data augmentation and class balancing. EfficientNet achieved the highest accuracy (70–75%), proving more suitable for small medical image datasets.

# 🧬 Lung Cancer Classification using Deep Learning

This project focuses on classifying **7 histopathological lung cancer subtypes** using three deep learning models: **ViT, ResNet50, and EfficientNet**. It uses the publicly available **LungHist700 dataset**.

---

## 📂 Dataset

- **Source**: [LungHist700 Kaggle Dataset](https://www.kaggle.com/datasets/yasserh/lunghist)
- **Classes**:
  - `nor` – Normal tissue
  - `aca_bd`, `aca_md`, `aca_pd` – Adenocarcinoma (borderline/moderate/poor)
  - `scc_bd`, `scc_md`, `scc_pd` – Squamous Cell Carcinoma (borderline/moderate/poor)

---

## 🛠️ Methodology

- Applied **data augmentation** and **class balancing**
- Used PyTorch, Timm models, and `WeightedRandomSampler`
- Evaluated using **per-class accuracy** and **confusion matrix**

---

## 🧪 Models & Accuracy

| Model        | Accuracy     |
|--------------|--------------|
| Vision Transformer (ViT) | 47–55% |
| ResNet50     | 55–60%       |
| EfficientNet | 70–75% ✅     |

- ✅ EfficientNet performed best due to small dataset + balanced training
- ❌ ViT performed worst due to high data requirement

---

## 📊 Results

- Included: Per-class accuracy, confusion matrix
- Predicts image class from test data

---

## 🔧 Installation

```bash
git clone https://github.com/yourusername/lung-cancer-classification.git
cd lung-cancer-classification
pip install -r requirements.txt
