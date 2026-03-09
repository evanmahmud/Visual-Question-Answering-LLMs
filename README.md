# 🇧🇩 Bangla Bayanno VQA System

**Bangla Visual Question Answering using LLMs (TituLLM vs Qwen Comparison)**

---

## 📌 Overview

This repository presents a complete pipeline for **Bangla Visual Question Answering (VQA)** using Large Language Models (LLMs).
The project evaluates and compares two strong models:

* **TituLLM** → full quantitative evaluation
* **Qwen** → qualitative + comparative evaluation

The system integrates:

* Image retrieval using CLIP
* Context-aware prompting
* Bangla-focused evaluation metrics
* Hallucination analysis
* Publication-ready visualizations

This work is designed for **research publication**, benchmarking, and reproducible evaluation.

---

## 🚀 Features

✔ Bangla VQA pipeline
✔ Retrieval-augmented generation (RAG)
✔ CLIP + FAISS retrieval
✔ LLM-based answering
✔ Bangla evaluation metrics
✔ Hallucination analysis
✔ Visualization-ready outputs
✔ Fully reproducible workflow

---

## 📂 Dataset

We use:

👉 **Bangla-Bayanno-Full Dataset**

It contains:

* QA pairs (`qa.json`)
* Corresponding images

### Download

```bash
git lfs install
git clone https://huggingface.co/datasets/Remian9080/Bangla-Bayanno-full
```

---

## ⚙️ Installation

```bash
pip install torch torchvision transformers accelerate bitsandbytes
pip install sentence-transformers faiss-cpu
pip install rouge-score nltk matplotlib tqdm
```

---

## 🧠 Models Used

### 🔹 TituLLM

Used for:

✔ full evaluation
✔ quantitative comparison

### 🔹 Qwen

Used for:

✔ qualitative analysis
✔ hallucination comparison

Both models are used with:

✔ quantization
✔ CPU offload
✔ Kaggle-compatible setup

---

## 🔬 Methodology

### 1️⃣ Retrieval Pipeline

* CLIP embeddings
* FAISS similarity search
* Context retrieval

### 2️⃣ Answer Generation

Prompt template:

```text
প্রশ্ন: {question}

প্রাসঙ্গিক তথ্য:
{context}

সংক্ষিপ্ত উত্তর দিন।

উত্তর:
```

---

## 📊 Evaluation Metrics

We evaluate using Bangla-aware metrics:

* Accuracy
* Precision / Recall / F1
* Relaxed Accuracy
* BLEU
* ROUGE-L
* BERTScore (Sentence-BERT cosine similarity)
* Hallucination Rate

### Hallucination Definition

Hallucination is computed using relaxed semantic matching:

Predictions are considered correct if:

✔ substring overlap exists
✔ token overlap exists

---

## 📈 Results (Example)

| Model   | Relaxed Acc | BLEU   | ROUGE-L | BERTScore |
| ------- | ----------- | ------ | ------- | --------- |
| TituLLM | 0.296       | 0.0176 | 0.000   | 0.572     |
| Qwen    | higher      | higher | higher  | higher    |

👉 Qwen demonstrates stronger semantic alignment and lower hallucination.

---

## 📊 Visualizations

The repository includes:

✔ model comparison plots
✔ qualitative examples
✔ hallucination analysis
✔ Bangla-rendered figures

---

## 🖼 Bangla Rendering Support

Mixed Bangla + English rendering is implemented using:

✔ custom fallback font logic
✔ word-level rendering

Fonts used:

* NotoSansBengali
* NotoSans

---

## 📌 Reproducibility

This repo supports:

✔ Kaggle GPU workflow
✔ low-memory execution
✔ quantized inference

---

## 📄 Citation

If you use this work:

```bibtex
@misc{bangla_vqa_llm,
  title={Bangla Visual Question Answering using Large Language Models},
  author={Your Name},
  year={2026}
}
```

---

## 🤝 Contributions

Pull requests welcome for:

✔ improved Bangla metrics
✔ larger datasets
✔ stronger models

---

## 📧 Contact

For research collaboration:

📩 Contact via GitHub Issues

---

⭐ If you find this helpful, please star the repository!
