
##Decoder-Only (GPT-2 / LLaMA) — Pseudo-code to Code Generation
#Problem Statement
The goal of this task is to develop a model that can generate executable Python code from structured pseudo-code instructions. Using a decoder-only architecture such as GPT-2 or LLaMA, the system learns to translate pseudo-code into syntactically and semantically correct Python programs.
# Dataset
We use the SPOC Dataset, which contains aligned pairs of pseudo-code and corresponding Python code.
This dataset provides a diverse range of algorithmic tasks suitable for training and evaluating code generation models.
# Objective
Fine-tune decoder-only models (e.g., GPT-2 or LLaMA) for pseudo-code → Python translation.
Ensure the generated outputs are syntactically valid and semantically executable.
# Key Steps
Data Preprocessing – Clean and align pseudo-code/code pairs, normalize formatting.
Tokenization – Apply GPT-2 or LLaMA tokenizer to both pseudo-code and Python targets.
Fine-tuning – Train using a causal language modeling (CLM) objective on the paired dataset.
Evaluation – Assess model quality using:
BLEU (text similarity)
CodeBLEU (code-aware metric)
Human Evaluation (readability and correctness)
Deployment – Build an interactive Streamlit or Gradio interface for real-time pseudo-code to code generation.
# Deliverables
Preprocessed dataset and tokenized training corpus
Fine-tuned GPT-2 / LLaMA model
Evaluation metrics and analysis results
Web interface for live demonstrations
