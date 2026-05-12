# Legal Document Summarizer using T5 Transformer

A transformer-based legal document summarization system built using Python, HuggingFace Transformers, and a fine-tuned T5 model to generate concise summaries from lengthy legal documents.

The project also includes an interactive multilingual demo capable of translating generated summaries into regional languages using the Google Gemini API.

---

## Features

- Fine-tuned T5 transformer model for legal text summarization
- Preprocessing pipeline for handling lengthy legal documents
- Tokenization and dataset preparation using HuggingFace
- ROUGE score evaluation during training
- Interactive legal document summarization demo
- Multilingual translation support using Gemini API
- GPU-accelerated training and inference using Google Colab

---

## Tech Stack

- Python
- HuggingFace Transformers
- T5 Transformer
- PyTorch
- Google Colab
- Google Gemini API
- IN-ABS Legal Dataset

---

## Project Structure

```text
legal-document-summarizer/
│
├── legal_document_training.ipynb
├── legal_document_demo.ipynb
├── README.md
└── LICENSE
```

---

## Training Pipeline

The training notebook includes:

1. Library installation and environment setup
2. Dataset loading and preprocessing
3. Tokenization using T5 tokenizer
4. Fine-tuning the T5 model on legal text data
5. ROUGE score evaluation
6. Model saving and inference generation

### Training Output

The model was trained on the IN-ABS legal summarization dataset using GPU acceleration in Google Colab.

Evaluation metrics generated during training:

| Epoch | Training Loss | Validation Loss | ROUGE-1 | ROUGE-2 | ROUGE-L |
|-------|----------------|----------------|---------|---------|---------|
| 1 | 2.4550 | 2.2390 | 0.1579 | 0.0694 | 0.1434 |
| 2 | 2.3686 | 2.1903 | 0.1585 | 0.0698 | 0.1350 |
| 3 | 2.3332 | 2.1784 | 0.1586 | 0.0702 | 0.1349 |

---

## Interactive Demo

The demo notebook allows users to:

- Input lengthy legal documents
- Generate concise summaries
- Translate summaries into regional languages
- Interactively test the fine-tuned model

### Supported Translation

- Telugu
- Additional languages supported through Gemini API integration

---

## Sample Output

### Input Legal Document

A lengthy Indian legal case document containing court proceedings, judgments, and legal arguments.

### Generated Summary

> "The appellant who was Assistant Engineer in the Central Public Works Department was placed under suspension pending a departmental enquiry under rule 12(2) of the Central Civil Services Rules. After multiple proceedings and appeals, the appellant was eventually dismissed from service."

### Telugu Translation

> తెలుగు అనువాదం successfully generated using Gemini API integration.

---

## Running the Project

### Clone the Repository

```bash
git clone https://github.com/CP-TEJESWAR/legal-document-summarizer.git
```

### Install Dependencies

```bash
pip install transformers datasets torch rouge_score sentencepiece accelerate
```

### Run the Notebooks

Open the notebooks using:

- Google Colab
- Jupyter Notebook

---

## Future Improvements

- Deploy as a web application using Flask or FastAPI
- Add support for additional transformer architectures
- Improve ROUGE evaluation performance
- Add PDF upload support
- Build a React frontend for real-time summarization

---

## Author

**Tejeswar CP**

- VIT-AP University
- B.Tech CSE (AI & ML)

GitHub: https://github.com/CP-TEJESWAR

---
