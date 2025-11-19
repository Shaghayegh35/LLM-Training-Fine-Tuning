# LLM Training, Fine-Tuning & Evaluation Pipeline

This repository provides an end-to-end workflow for training, fine-tuning, and evaluating  
a Causal Language Model (LLM) using Hugging Face `transformers`, `datasets`, PyTorch,  
and parameter-efficient fine-tuning (LoRA).

It includes everything needed to understand how modern LLM pipelines work—  
from raw data → tokenization → full fine-tuning → LoRA → evaluation → iteration.

The pipeline uses:

- **Dataset:** `lamini/lamini_docs`
- **Base Model:** `EleutherAI/pythia-70m` (lightweight, ideal for learning)
- **Fine-Tuning Methods:** Full training + LoRA
- **Frameworks:** Hugging Face `transformers`, `datasets`, `peft`, `accelerate`

---

## 🚀 Project Highlights

- Build instruction–response datasets from JSONL or Hugging Face datasets  
- Tokenize data and prepare training splits  
- Fine-tune GPT-style models using Hugging Face `Trainer`  
- Apply **LoRA (Low-Rank Adaptation)** for parameter-efficient training  
- Save and load trained models  
- Evaluate base vs. finetuned models  
- Iteratively refine prompts and dataset quality  
- Lightweight notebooks ideal for students & job portfolios  

---

## 📁 Project Structure

```text
.
├─ README.md
├─ requirements.txt
├─ .gitignore
│
├─ data/                    
│   └── lamini_docs.jsonl   # (ignored) example dataset
│
├─ data_preparation.ipynb               # Build & tokenize instruction dataset
├─ llm_finetuning_lamini_docs.ipynb     # Full fine-tuning of Pythia-70M
├─ evaluation_iteration.ipynb           # Evaluation & comparison of models
└─ fine_tune_with_LoRA.ipynb            # NEW: LoRA fine-tuning workflow
