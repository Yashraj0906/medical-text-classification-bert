# Medical Text Classification using BERT

This project implements an end-to-end medical text classification pipeline using a fine-tuned BERT-based model. The objective is to classify medical research study titles into outcome-based categories using transfer learning with Hugging Face Transformers.

---

## 📌 Project Overview

Medical research generates thousands of studies with varying outcomes. Manually reviewing these studies is time-consuming. This project demonstrates how a pretrained transformer model can be fine-tuned to automatically classify medical study titles based on their reported results.

The project focuses on:
- Domain-specific NLP
- Fine-tuning pretrained language models
- Building an inference-ready pipeline

---

## 🧠 Model & Methodology

- **Model Used:** `distilbert-base-uncased`
- **Frameworks:** PyTorch, Hugging Face Transformers
- **Task Type:** Multi-class text classification
- **Training Approach:** Transfer learning using Hugging Face `Trainer`

### Target Classes
The model predicts one of the following outcome categories:
- **Positive**
- **Negative**
- **Inconclusive**
- **Needs_AI**

---

## 📊 Dataset

- ~12,000 medical research study titles
- Each title is labeled with an outcome category
- Dataset is **not included** in this repository due to size and licensing constraints

The notebook can be easily adapted to any similar labeled text dataset.

---

## 📈 Results

After fine-tuning the model for **3 epochs**, the following performance was achieved on the test set:

- **Accuracy:** ~70%
- **F1-score (weighted):** ~67%

These results indicate effective learning on real-world medical text data.

---

## 🧪 Sample Prediction

Example input:

📸 Refer to `sample_image.png` for an example inference output.

---

## 🗂️ Repository Structure

medical-text-classification-bert/
├── Medical_Text_Classification_BERT.ipynb
├── requirements.txt
├── sample_image.png
└── README.md


---

## 🛠️ How to Run the Project

1. Clone the repository:
```bash
git clone https://github.com/Yashraj0906/medical-text-classification-bert.git
cd medical-text-classification-bert 
```
2. Install dependencies:
```bash
pip install -r requirements.txt
```
3. Open the notebook:
```bash
Medical_Text_Classification_BERT.ipynb
```
