# LLM Training, Fine-Tuning & Evaluation Pipeline

This repository provides an end-to-end workflow for training and fine-tuning a Causal Language Model (LLM) using Hugging Face `datasets` and `transformers`.  
It covers the complete process used in real LLM engineering projects: data preparation, tokenization, model training, and iterative evaluation.

The pipeline uses:

- **Dataset:** `lamini/lamini_docs`
- **Base Model:** `EleutherAI/pythia-70m` (lightweight, great for learning)
- **Frameworks:** Hugging Face `transformers`, `datasets`, and PyTorch

---

## 🚀 Project Highlights

- Clean workflow for LLM dataset preparation and prompt formatting  
- Tokenization using `AutoTokenizer` and Hugging Face `Dataset`  
- Fine-tuning a GPT-style model using `Trainer`  
- Saving and loading finetuned models  
- Qualitative evaluation comparing **base vs. finetuned** outputs  
- Iteration process for improving dataset quality and model performance  

---

## 📁 Project Structure

```text
.
├─ README.md
├─ requirements.txt
├─ .gitignore
│
├─ data/                    # local data folder (ignored in git)
│   └── lamini_docs.jsonl   # example dataset (not included)
│
├─ data_preparation.ipynb               # Data extraction, JSONL parsing & tokenization
├─ llm_finetuning_lamini_docs.ipynb     # Fine-tuning Pythia-70m on lamini_docs
└─ evaluation_iteration.ipynb           # Model evaluation & iterative refinement
