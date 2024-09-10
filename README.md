# AI-Powered Grading Assistant

## Overview

This project is an AI-powered grading assistant designed to help professors evaluate student answers based on a given PDF book. The system uses the T5 model from Hugging Face to generate questions from the book, evaluates student answers for these questions, and saves the results in an Excel file.

## Features

- **Text Extraction**: Extracts text from a PDF book.
- **Question Generation**: Generates three questions based on the extracted text.
- **Answer Evaluation**: Evaluates student answers against the book text using TF-IDF and cosine similarity.
- **Result Saving**: Saves student scores and details in an Excel file.

## Requirements

- Python 3.7+
- `transformers` library
- `PyPDF2` library
- `gradio` library
- `scikit-learn` library
- `pandas` library
- `openpyxl` library (for Excel file operations)

You can install the required libraries using pip:

```bash
pip install transformers PyPDF2 gradio scikit-learn pandas openpyxl
