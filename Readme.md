# 🌙 Fine-Tuning an LLM for the Damascene Arabic Dialect

> Fine-tuning a large language model on **Shami (Damascene/Levantine) Arabic**.

---

## 📖 Overview

The **Damascene dialect** (Shami Arabic / اللهجة الشامية) is widely spoken across Syria and the Levant, yet remains severely underrepresented in NLP research.

---

## ✨ Features

- Fine-tuned **Qwen** base model on Damascene (Shami) Arabic dialect data
- Custom dataset curated specifically for colloquial Damascene expressions, vocabulary, and grammar
- Full training pipeline implemented as reproducible Jupyter notebooks
- Saved model weights ready for inference

---

## 🗂️ Repository Structure

```
Fine-Tuning-LLM-for-Damscene-Dialect/
│
├── data/                        # Training and evaluation datasets
│   └── ...                      # Damascene dialect text samples
│
├── notebooks/                   # Jupyter notebooks for training & evaluation
│   └── ...                      # Step-by-step fine-tuning pipeline
│
├── model/
│   └── shami-qwen-final/        # Final fine-tuned model weights & config
│
├── .gitattributes
└── .gitignore
```

---

## 🚀 Getting Started

### Prerequisites

```bash
pip install torch transformers datasets peft accelerate bitsandbytes
```

A CUDA-capable GPU is recommended (16GB+ VRAM). Training can also be run on Google Colab with a T4/A100 instance.

### Clone the Repository

```bash
git clone https://github.com/philipnakhleh/Fine-Tuning-LLM-for-Damscene-Dialect.git
cd Fine-Tuning-LLM-for-Damscene-Dialect
```

### Run the Notebooks

Open the notebooks in order inside the `notebooks/` directory. They walk through:

1. **Data preparation** — loading and formatting the Damascene dialect dataset
2. **Model fine-tuning** — applying LoRA/QLoRA adapters to the Qwen base model
3. **Evaluation** — testing the fine-tuned model against baseline outputs
4. **Inference** — generating responses in Shami Arabic


## 🛠️ Tech Stack

| Component | Technology |
|-----------|-----------|
| Base Model | Qwen (multilingual LLM) |
| Fine-tuning Method | LoRA (PEFT) |
| Training Framework | Hugging Face `transformers` + `trl` |
| Notebooks | Jupyter |
| Prompt Templates | Jinja2 |

---

## 🌍 Why Damascene Arabic?

The Damascene dialect is spoken by millions across Syria and the diaspora. Despite this, NLP tools for Shami Arabic remain scarce. This project is a step toward:

- More inclusive Arabic NLP research
- Better dialect-aware chatbots and assistants
- Preserving and digitizing spoken Levantine Arabic

---

## 🤝 Contributing

Contributions are welcome! If you have Damascene dialect data, improvements to the training pipeline, or evaluation benchmarks, feel free to open an issue or submit a pull request.

---

## 📄 License

This project is open source. Please refer to the repository for licensing details.
