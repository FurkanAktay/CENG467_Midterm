# CENG 467 — Natural Language Understanding and Generation

**Take-Home Midterm Examination**
Izmir Institute of Technology — Department of Computer Engineering
Instructor: Prof. Dr. Aytuğ Onan

## Overview

This repository contains the implementation, experiments, and analysis for the CENG 467 take-home midterm. The midterm covers five core NLP tasks, each implemented as an independent, reproducible Colab notebook.

| # | Task | Notebook | Models |
|---|------|----------|--------|
| Q1 | Text Classification | `Q1_Text_Classification.ipynb` | TF-IDF + Logistic Regression, BiLSTM, DistilBERT |
| Q2 | Named Entity Recognition | `Q2_Named_Entity_Recognition.ipynb` | BiLSTM-CRF, DistilBERT-NER |
| Q3 | Text Summarization | `Q3_Text_Summarization.ipynb` | LexRank (extractive), BART-CNN (abstractive) |
| Q4 | Machine Translation | `Q4_Machine_Translation.ipynb` | Seq2Seq + Attention, OPUS-MT (Transformer) |
| Q5 | Language Modeling | `Q5_Language_Modeling.ipynb` | Trigram (Kneser-Ney), LSTM-LM |

## Reproducibility

All experiments use a fixed random seed (`SEED = 42`) and are runnable on Google Colab Free (T4 GPU, 15 GB VRAM).
Each notebook is self-contained: it installs its own dependencies, downloads the dataset, and writes results to `/results`.

### Environment

- Python 3.11 (Colab default)
- PyTorch 2.x + CUDA (Colab default)
- See per-notebook `pip install` cell for exact package versions.

### Running the Notebooks

1. Open the notebook in Google Colab.
2. Set runtime to **GPU (T4)**.
3. Run all cells (`Runtime → Run all`).
4. Final results table and qualitative examples are printed in the last cells.

## Repository Structure

```
CENG467_Midterm/
├── README.md
├── Q1_Text_Classification.ipynb
├── Q2_Named_Entity_Recognition.ipynb
├── Q3_Text_Summarization.ipynb
├── Q4_Machine_Translation.ipynb
├── Q5_Language_Modeling.ipynb
├── results/                  # Output JSON/CSV per notebook
└── reports/
    └── CENG467_Midterm_Report.pdf
```

## Author

Yusuf Furkan Aktay — Student ID: `<333078005>`
