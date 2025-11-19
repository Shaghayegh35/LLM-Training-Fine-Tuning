# LLM Data Tokenization & Finetuning Pipeline

Jupyter notebooks for preparing instruction–response datasets and finetuning
a causal language model using Hugging Face `datasets` and `transformers`.

The project uses the `lamini/lamini_docs` dataset and `EleutherAI/pythia-70m`
as a base model to demonstrate an end-to-end workflow:
data preparation → tokenization → training → saving a finetuned model.

## Project structure

```text
.
├─ README.md
├─ requirements.txt
├─ .gitignore
├─ data/
│  └─ lamini_docs.jsonl        # optional local data (not in repo)
├─ data_preparation.ipynb
└─ llm_finetuning_lamini_docs.ipynb
