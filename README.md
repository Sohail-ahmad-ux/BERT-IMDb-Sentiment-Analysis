# 🎬 BERT Sentiment Analysis on IMDb

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)
![Transformers](https://img.shields.io/badge/Transformers-FF8C00?style=for-the-badge)
![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)

**Fine-tuning `bert-base-uncased` for Binary Sentiment Classification on the IMDb Movie Reviews Dataset using Hugging Face Transformers.**

---

## ✨ Project Highlights

- ✅ **Pretrained Model**: `bert-base-uncased` (110M parameters)
- ✅ Full fine-tuning using Hugging Face `Trainer` API
- ✅ Proper tokenization with padding and truncation
- ✅ GPU-accelerated training (NVIDIA Tesla T4)
- ✅ Custom inference on new movie reviews
- ✅ Clean, reproducible Jupyter Notebook

---

## 📊 Results

| Metric                  | Value              |
|-------------------------|--------------------|
| **Model**               | `bert-base-uncased` |
| **Dataset**             | IMDb (25k train / 25k test) |
| **Epochs**              | 2                  |
| **Training Loss**       | 0.430              |
| **Validation Loss**     | 0.595              |
| **Max Sequence Length** | 256 tokens         |
| **Batch Size**          | 8                  |
| **Learning Rate**       | 2e-5               |

---

## 🧠 Model Used

- **Base Model**: [`bert-base-uncased`](https://huggingface.co/bert-base-uncased)
- **Architecture**: BERT (Bidirectional Encoder Representations from Transformers)
- **Parameters**: 110 million
- **Hidden Size**: 768
- **Attention Heads**: 12
- **Layers**: 12
- **Task**: Sequence Classification (2 labels: Positive / Negative)
- **Tokenizer**: BERT WordPiece tokenizer

---

## ⚙️ Training Details

- **Framework**: Hugging Face `transformers` + `Trainer` API
- **Optimizer**: AdamW (with weight decay = 0.01)
- **Loss Function**: Cross Entropy Loss
- **Mixed Precision**: Not used (default FP32)
- **Hardware**: NVIDIA Tesla T4 GPU
- **Training Time**: ~34 minutes for 2 epochs

### Hyperparameters

yaml
**learning_rate: 2e-5
**per_device_train_batch_size: 8
**per_device_eval_batch_size: 8
**num_train_epochs: 2
**weight_decay: 0.01
**max_length: 256
**eval_strategy: epoch
**save_strategy: epoch

### 📋 Workflow

**Load IMDb Dataset
**Tokenize reviews (max_length=256)
**Load Pretrained BERT with classification head
**Fine-tune using Trainer API
**Evaluate on test set
**Perform inference on custom text
