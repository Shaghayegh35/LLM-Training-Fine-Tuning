# LLM Data Tokenization & Finetuning Pipeline

Jupyter notebooks for preparing instruction–response datasets and finetuning
a causal language model using Hugging Face `datasets` and `transformers`.

The project uses the `lamini/lamini_docs` dataset and `EleutherAI/pythia-70m`
as a base model to demonstrate an end-to-end workflow:
data preparation → tokenization → training → saving a finetuned model.

- **evaluation_iteration.ipynb**  
  Contains steps for evaluating the finetuned model, comparing outputs from the base model vs. the trained model, and performing iterative improvements. Includes prompt testing, qualitative evaluation, and guideline suggestions for dataset refinement.


## Project structure

```text
.
LLM-data-tokenization-pipeline/
│
├── README.md
├── requirements.txt
├── .gitignore
│
├── data/
│   └── lamini_docs.jsonl   (ignored)
│
├── data_preparation.ipynb
├── llm_finetuning_lamini_docs.ipynb
└── evaluation_iteration.ipynb

