# 🎬 BERT Sentiment Analysis on IMDb

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)
![Transformers](https://img.shields.io/badge/Transformers-FF8C00?style=for-the-badge)
![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)

**Fine-tuning BERT-base-uncased for Binary Sentiment Classification on the IMDb Movie Reviews Dataset using Hugging Face Transformers.**

---

## ✨ Features

- ✅ **State-of-the-art** BERT model fine-tuning
- ✅ Hugging Face `transformers` + `datasets` library
- ✅ Efficient tokenization with padding & truncation
- ✅ Full training with `Trainer` API
- ✅ Model evaluation & custom inference
- ✅ GPU accelerated (CUDA support)
- ✅ Clean, well-structured Jupyter Notebook

---

## 📊 Results

| Metric                | Value          |
|-----------------------|----------------|
| **Model**             | `bert-base-uncased` |
| **Dataset**           | IMDb (25k train, 25k test) |
| **Epochs**            | 2              |
| **Training Loss**     | 0.430          |
| **Validation Loss**   | 0.595          |
| **Max Sequence Length**| 256 tokens    |

---

## 🛠️ Technologies Used

- **Hugging Face Transformers**
- **Hugging Face Datasets**
- **PyTorch**
- **BERT-base-uncased**
- **Python 3.12 + CUDA**

---

## 📁 Project Structure

```bash
BERT-IMDb-Sentiment-Analysis/
├── project-03-bert-fine-tuning.ipynb    # Main Notebook
├── README.md
└── results/                             # Training outputs (auto-generated)
